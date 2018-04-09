##### How did you determine which rules should be placed in each new CSS file?

* The most basic rules that apply most broadly I tried to put in the base.css. 

  * Such As:   * items, body background and basic positioning of nav, article, aside, an dfooter section. 

* For layout.css I tried to pin point items that will reoccur on every page with child selectors
  
  * Such As: Logo,  hr, recipe block, and aside positioning

* For modules.css I tried to pinpoint items that I was specifically diving into in order to more specifically select
  * Such As: the nav in the header, the h2, p, date, and print inside of the article tag, and image, h3, and p inside of the aside tag

---

##### Did you do any refactoring of the existing CSS? If so, briefly explain what you did and why.

* I erased the 'input' styling because this styling is rendundant because the styling of class 'recipe' already applies to the input text

* I refactored 'h2' to be a 'h2' and an 'article h2' because I assume the we want the h2s to look the same but we may not want the same spacing if there is an h2 outside of the article tag

* Refactored 'main p' to 'article p' to isolate the description of the recipe in case we want to add other p tags in the main that's not related to the recipe

* Added a 'article .date' and 'article .print' selector because I imagine we may wnat to use theses classes again to produce a consistent look to these elements but may not not want to maintain the spacing that is used inside of the article tag

* Added 'header nav ul' and 'header nav li' rather than 'nav ul' and 'nav li' because we may want to add navigation into another part of the page and not keep the header navigation spacing but we want our header navigation to be consistent across pages