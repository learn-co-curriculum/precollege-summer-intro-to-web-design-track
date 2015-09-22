# CSS Selectors - Full Lecture

## SWBATs

### CSS

+ Use descendant selectors (Descendent,  sibling, precendent )
+ Use pseudo selectors
+ Use the universal selector
+ Use attribute selectors
+ Use compound selectors

## Motivation

We're starting to make some complex HTML pages and sometimes you need to get really specific about the element you are styling. Today we are going to go into more depth about how to use selectors to be very specific about styling elements on the page and keep our CSS stylesheets nice and clean.

## Lesson Plan

+ We've already learned how to use selectors. What are selectors? They are how we identify and apply styles to our HTML elements, such as `<p>`,`<h1>`, etc. We can also use selectors to target classes and IDs, such as `#nav` and `.button-default`

+ We can target elements on our page by specifying where one selector is in relation to another with a few different selector - today we'll talk about two:
  + Descendent Selectors
    + `nav li`
  + Child 
    + `#list > li {…}`
  + Sibling
    + `h3 + p {…}`
  + Preceded
    + `.styleafter ~ h2 {…}`
  + Pseudo Selectors
    + `a:hover`

### Special Selectors

#### Descendant Selectors

+ A descendent selector targets the last selector listed (li in the example above), using the previously listed selectors to narrow its scope. 

Given this HTML:
```html
<nav>
  <ul>
    <li>Home</li>
    <li>About</li>
    <li>Home</li>
  </ul>
</nav>
<ol> Favorites
  <li>Cheese</li>
  <li>Chocolate</li>
  <li>Cheetos</li>
<ol>
```

```css
nav li {
  color: purple
}
```

This CSS selector, `nav li` is saying is that we should target only those `li`'s that are nested within the `nav`. Any `li` element outside of the element with the `#nav` id would be unaffected. Based on that, we should only see the `nav` items text changed to purple, not our list of "Favorites".

+ To select descendents, your selection should list the 'parent' element and then the child(ren) that you're looking to select. For example, an `<a>` tag (child) inside of `<div id="pop">` (parent):

```html
  <div id="pop">
    <a href="google.com"> GOOGLE</a>
  </div>
```
 would be written as as:

```css
#pop a {
 /* styling here*/
}
``` OR 

```css 
div#pop a {
  /* styling here*/
}
```

+ The space in between the two selectors indicates descendence.

+ If we have a list within a list like this:

```html
  <ul id="nav">
    <li>child
     <ul><li>grandchild</li></ul>
     </li>
  </ul>
```

```css
#nav li {
  color: red;
}
```
+ Remember, because of cascading `#nav li` will target not only the child `<li>`, but it will also affect grandchildren, etc. That means both the text "child" and "grandchild" will 
appear in red text.

+ If you want to be more specific and only target direct descendants (just the child) - `child selector` in the example above, the text "child", you can use the child selector:

```css
#list > li {
  color: red;
}
```. 

+If you do this the grandchildren will not be affected by any CSS you specify here, they will show up in black text.

#### Sibling Selector

+ The `sibling selector` is very specific - like the child selector - but it does not depend on nested elements. It targets the next element that comes after. 
```html
<h3>An h3 Element</h3>
<p>I'm a p directly after an h3 element.</p>
<p>Not selected</p>
```

```css
h3 + p {
  color: green;
}
```
In this example, only the `p` element directly following the h3 element will be styled - the text "I'm a p directly after an h3 element." will appear in green.

#### Precedent Selector

+ The more general sibling selector is called the `precedent selector`. It will target all the siblings following an indicated selector - not just the one immediately following the selector. It does NOT affect siblings that are nested within another element though. Here is an example that all the text following the first line of text will show up in red color

 ```html
  <p class="pre">I’m the pre div.</p>
  <h2>I'm an h2 positioned after the pre div</h2>
  <h2>Me too!</h2>
  <div>`
    <h2>I’m nested within another element so I won’t be affected by the precedent style</h2>
  </div>
```

```css
.pre ~ h2 { 
  color:red;
}
```


#### Universal Selector

+ Universal selector will affect everything on the page. This helpful if you want to remove default margin and padding from HTML elements so that you can have granular control over layout.

```css
* {
  margin: 0px;
  padding: 0px;
}
``` 


### Attribute Selectors

+ The attribute selector will look for tags that have a certain attribute. In the example below, we're looking for `a` tags with the `target` attribute set as `_blank`. This way we can style links differently that open in a new window versus the same window (thats what `target="_blank"`, opens a link in a new window). We'll see the text "Google" in green.

HTML:
```html
<a href="www.google.com" target="_blank">Google</a>
<a href="www.facebook.com">Facebook</a>
<a href="www.twitter.com">Twitter</a>
```

CSS:
```css
a[target="_blank"] { 
  color: green
}
```

The attribute selector can really help you target elements in unique ways. Examples:

<img src="https://s3.amazonaws.com/after-school-assets/css-selector1.png">

### Pseudo Selectors

+ Pseudo class selectors are especially helpful in styling links, especially when you want to style an element when a user mouses over it or style visited and unvisited links differently.

HTML:
```html
<a href="https://www.google.com/"> Google</a>
```

CSS:
```css
/* first time load link on page */
a:link {
    color: #FF0000;
}

/* visited link */
a:visited {
    color: #00FF00;
}

/* mouse over link */
a:hover {
    color: #FF00FF;
}

/* selected link */
a:active {
    color: #0000FF;
}
```
+ Other examples:
<img src= "https://s3.amazonaws.com/after-school-assets/css-selector2.png">

### Compound Selectors:

+ Cleaning up and streamlining your CSS stylesheet is another way to make it easier to keep track of which elements you are styling and make sure you are targeting the right elements. If there are several things on the page that you want styled in a similar fashion you can use compound selectors. For example, if I want all my h2 and h3 tags to be purple I can indicate that like this:

HTML:
```html
  <h1> I Love Flatiron</h1>
  <h2> Flatiron School Is Amazing</h2>
  <h3> 11 Broadway, NYC</h3>
```
CSS:
```css
h2, h3 {
  color: purple;
}
```

### Inheritance

+ One last important bit of CSS are the rules around authority and inheritance.
+ If you use conflicting styles on the same element, ID overrules class which overrules type which overrules * (universal). 
  + Generally the more specific a selector, the more authority it has. If a more specific selector is not defined for an element it will inherit styles from a previously defined general selector statement.
+ If multiple Classes are applied to the same element(ie `<div class="btn btn-blue btn-green">` which has the classes `btn` `btn-blue`, and `button-green`), the Class listed furthest to the right overrules its neighbors to the left. For the example above, the `btn-green` styling would overrule `btn-blue` and `btn`. 
+ Uses “last man” rule. When conflicts with equal authority arise, CSS will listen to the last style it was told to apply. 
+ Now you know everything you need to get started with CSS! *Time for some practice!*


### Labs

+ [Graffiti Override](https://github.com/learn-co-curriculum/Css-Graffiti-Override)
+ [Pseudo Selector Blocks](To do) - use this as base: http://jsfiddle.net/webtiki/MpXYr/2/light/

