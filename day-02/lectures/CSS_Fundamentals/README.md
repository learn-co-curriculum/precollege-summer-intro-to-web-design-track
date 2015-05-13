### Overview

Create a brand new HTML page and style it with CSS

###SWBATs

+ Use selectors
+ Write CSS Syntax
+ link a CSS stylesheet to an HTML page
+ explain the purpose of CSS
+ adjust basic properties of text: `font-size`, `font-family`, `text-align`, `font-color`
+ adjust basic properties of images: `height`, `width`
+ Adjust backgrounds elements
+ Use hexadecimal, rgba, and rgb color values

### Motivation / Why Should You Care?

Have Justin Bieber’s twitter page up with all stylesheets unlinked (with dev tools can just delete all the link tags). Explain that this is what his twitter looks like with JUST HTML. It’s a lot like what our sites look like with just HTML.
Have students point out things that look different, from what it normally looks like -- all the styling.
So far, all we’ve been able to do is put content on a page with HTML to make some ugly looking websites. So how do we actually make our sites stuff look good? CSS!
CSS stands for Cascading Style Sheets. We write CSS in separate files, so that each file of our web site does one job and one job only. Single purpose files. 


### Lesson Plan
+ CSS: 
  * write in a separate file - separation of concerns, easier to debug
  * Using the `my_website` project we started earlier with HTML, make a `style.css` file inside the `css` directory
+ In `style.css` to make h1 font color red: `h1 { color: red; }`
  * h1 is CSS selector
  * property and value go between curly braces
  * colons and semi-colons are important
  * refresh browser: won't see change because not linked
+ `<link rel="stylesheet" type="text/css" href="css/style.css">` inside head tag in `index.html`
  * `rel` attribute: relationship of file being linking
  * `type` attribute: the type of file being linked
  * `href` attribute: where to find the file being linked
    * have to tell our `index.html` how to find `style.css`, so it needs to go inside css directory first
+ Other styling:text size, image size, centering text, background color, background image and have them style their page.
  * see code snippets [here](https://github.com/flatiron-school-curriculum/hs-intro-web-design-teachers-guide-code-snippet-1)
+ RGB vs Hexadecimal color 
  * There are a few ways to get more specific with color value other than just writing "red". There are many tones of red
  * RGB- stands for Red, Green, Blue. RGB color model is the ways of getting different colors through adding different amounts of Red, Green, and Blue.
    * Count up from 0 amounts of each to 255 of each
    * `rgb(0,0,0)` gives you black
    * `rgb(255,255,255)` gives you white
  * Hexademical is a different notation for the amount of Red, Green, and Blue that gets added to your color.
    * count: 0, 1, 2, 3, 4, 5, 6, 7, ,8, 9, a, b, c, d, e, f
    * 6 values: two red, two green, two blue
    * `#000000` is black
    * `#ffffff` is white
    * `#0000FF` is blue (zero amounts of red and green)
  * [Color Picker](http://www.w3schools.com/tags/ref_colorpicker.asp) is a great resource to find other color tones
+ Google fonts 
  * Browsers can only display whatever fonts are downloaded on that computer. 
  * If a web application is using some random font that my computer doesn't have, I won't be able to see it
  * [Google fonts](http://www.google.com/fonts) is a great resource
  * Click the quick view button <img src="https://s3.amazonaws.com/after-school-assets/google-font-quick-view.png" height="30px">
  * Scroll down the page till you see this and make sure `import` is selected: <img src="https://s3.amazonaws.com/after-school-assets/google-font-import.png">
  * Copy that the `@import`... text and paste it at the top of your CSS file
  * Step 4 shows you how to use the font: <img src="https://s3.amazonaws.com/after-school-assets/google-font-usage.png">
    * They chose to style the `font-weight` property as well, you can ignore that
  ```css
    h1 {
      font-family: 'Metrophobic', Arial, serif;
    }
  ```
+ Adding pages to your site: create three separate html files 
+ Inside of those files set up your html file structure
+ Put links in an unordered list using ul and li tags
  * will style next class as a nav bar

### Conclusion / So What?
CSS allows us to add styling to our page. Together, HTML and CSS give us the web as we know it. 

### Hints and Hurdles
+ Test all your CSS examples first and know how you're going to live code them. It's easy to make mistakes here that are hard to get out of on the spot. 