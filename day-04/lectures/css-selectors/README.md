#DAY-04 CSS Selectors

_A full lecture is available [here](LECTURE.md)_

## SWBATs

### CSS

+ Understand how to use descendant selectors
+ Use pseudo selectors
+ Use display-state property to show/hide elements
+ Use scaling elements - px and %
+ Understand and use border property for box styling, including border radius and box shadow

## Motivation

We’re starting to make some complex HTML pages and sometimes you need to get really specific about the element you are styling. Today we are going to go into more depth about how to use selectors to be very specific about styling elements on the page and keep our CSS stylesheets nice and clean.

## Lesson Plan

+ We’ve already learned how to use selectors. What are selectors?
+ We can target elements on our page by specifying where one selector is in relation to another with a few different selector
  + Descendent Selectors
  + Child 
  + Sibling
  + Preceded
  + Pseudo Selectors

### Special Selectors

+ A descendent selector targets the last selector listed (li in the example above), using the previously listed selectors to narrow its scope
+ To select descendents, your selection should list the 'parent' element and then the child(ren) 
+ Remember, because of cascading `#nav li` will target not only the child `<li>`, but it will also affect grandchildren, etc.

+ If you want to be more specific and only target direct descendants (just the child)above you can use the child selector `#list > li {…}`. If you do this the grandchildren will not be affected by any CSS you specify here.
+ The sibling selector is very specific - like the child selector - but it does not depend on nested elements. It targets the next element that comes after.
+ The more general sibling selector is called the precedent selector. It will target all the siblings following an indicated selector - not just the one immediately following the selector. It does NOT affect siblings that are nested within another element though.

+ There are a few other helpful selectors that we can use: Universal `* {…}`, Attribute `img[alt="Cat"] {…}` and Pseudo selectors `li:first-child {…}`, `a:link {…}`
+ The universal selector will affect every element on the page. 

### Attribute Selectors

+ The attribute selector will look for tags that have a certain attribute

### Pseudo Selectors

+ Pseudo class selectors are especially helpful in styling links

+ Cleaning up and streamlining your CSS stylesheet is another way to make it easier to keep track of which elements you are styling and make sure you are targeting the right elements. If there are several things on the page that you want styled in a similar fashion you can use compound selectors.

### Inheritance

+ One last important bit of CSS are the rules around authority and inheritance.
+ If you use conflicting styles on the same element, ID overrules class which overrules type which overrules * (universal). 
+ If multiple Classes are applied to the same element(ie `<div class="btn btn-blue btn-green">`), the Class listed furthest to the right overrules its neighbors to the left.
+ Uses “last man” rule. When conflicts with equal authority arise, CSS will listen to the last style it was told to apply. 
