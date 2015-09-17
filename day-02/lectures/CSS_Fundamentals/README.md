#DAY-02 CSS Fundamentals

_A full lecture is available [here](LECTURE.md)_

## Overview

Create a brand new HTML page and style it with CSS

## SWBATs

+ Explain the purpose of CSS
+ Use selectors
+ Write CSS Syntax
+ Link a CSS stylesheet to an HTML page
+ Adjust basic properties of text: `font-size`, `font-family`, `text-align`, `font-color`
+ Adjust basic properties of images: `height`, `width`
+ Adjust backgrounds elements
+ Use hexadecimal, rgba, and rgb color values
+ Use classes and IDs to style specific HTML elements

## Motivation / Why Should You Care?

Have Beyonce’s twitter page up with all stylesheets unlinked (with dev tools can just delete all the link tags). Explain that this is what her twitter looks like with JUST HTML. It’s a lot like what our sites look like with just HTML.

Have students point out things that look different, from what it normally looks like -- all the styling.
So far, all we’ve been able to do is put content on a page with HTML to make some ugly looking websites. So how do we actually make our sites stuff look good? CSS!
CSS stands for Cascading Style Sheets. We write CSS in separate files, so that each file of our web site does one job and one job only. Single purpose files.

*Ask your students what they would want to style about their website? Or the one you have shown.*

## Lesson Plan

### Intro - Selectors and Linking our Stylesheet

+ We write our CSS in a separate file - style is a different job than structure. 
+ Using the `my_website` project we started earlier with HTML, make a `style.css` file inside the `css` directory
+ In `style.css`, let's make our `<h1>`s a different color. 
+ Property and value go between curly braces with colons and semi-colons 
+ Refresh your browser: won't see change because we haven't linked our stylesheet. 
+ Add `<link rel="stylesheet" type="text/css" href="css/style.css">` inside head tag in `index.html`
+ Other styling to play around with:text size, image size, centering text, background color, background image and have them style their page (see code snippets [here](./code_snippet1.md))
+ Put three paragraphs on the page and make the first one have a font color of red by using and ID
+ Then use a class to make the first and last paragraph font color red

### Colors

+ RGB vs Hexadecimal color 
  * RGB- stands for Red, Green, Blue. RGB color model is the ways of getting different colors through adding different amounts of Red, Green, and Blue count up from 0 amounts of each to 255 of each
  * Hexademical is a different notation for the amount of Red, Green, and Blue that gets added to your color.
    * count: 0, 1, 2, 3, 4, 5, 6, 7, ,8, 9, a, b, c, d, e, f (6 values: two red, two green, two blue)
  * [Color Picker](http://www.w3schools.com/tags/ref_colorpicker.asp) is a great resource to find other color tones

### Fonts

+ Google fonts (http://www.google.com/fonts) 
  * Browsers can only display whatever fonts are downloaded on that computer. 
  * Scroll down the page till you see this and make sure `import` is selected: <img src="https://s3.amazonaws.com/after-school-assets/google-font-import.png"> and copy and paste into the top of the CSS file

+ If you haven't already added three pages to your site: create three separate html files and put links to your other pages in an unordered list using ul and li tags

### Conclusion / So What?
CSS allows us to add styling to our page. Together, HTML and CSS give us the web as we know it. 

### Hints and Hurdles
+ Test all your CSS examples first and know how you're going to live code them
