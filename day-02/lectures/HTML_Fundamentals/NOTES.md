# HTML Fundamentals

## Objective

Create a brand new HTML page from scratch using HTML5

## SWBATS

+ Structure an html page using `doctype`, `html`, `head` and `body` tags
+ Explain what goes into the head of the document
+ Add text to a page using `p` and `h1` tags
+ Add images using `img` tag
+ Add links using `a` tags and understand the difference between relative and absolute paths
+ Create multiple pages and link them
+ Create an ordered list using `ul` and `ol` tags

## Motivation / Why Should You Care?

HTML is the foundational technology for the Internet, every one of your favorite websites is HTML at its core. 

Yesterday you used a prepared template to create personal pages for our student directory. Today you are going to learn how to create an HTML site from scratch, create your own styles for the page and deploy it to the world wide web with GitHub.

## Lesson Plan

### Setup

*Students should be able to follow along with this demo*
+ In Nitrous terminal/command line from inside `development` directory make a directory (`mkdir`) called `my_website`
+ `cd` into that directory and make a `css` directory and an `index.html` file.
+ Add this HTML to `index.html`:

```html
<!doctype html> 
<html></html>
<head></head>
<body></body>
```
### Ideation

People make websites about all sorts of stuff
*Ask the students for some website ideas about things they love.*

### Tag syntax
Every HTML tag has an opening and closing tag with its content in the middle. The tag names are contained within angle brackets, and a closing tag has a `/` before the tag name.

Tags can also have attributes applied to them. These can be thought of as modifying or providing additional information to a tag. A tag can have any number of attributes. These are placed in the opening tag.

### Tag Nesting and Whitespace

Most tags can contain other tags inside of them. When we do this it is customary to indent the nested tags and their content by 2 or 4 spaces. This is to make it easier to read for humans. Using whitespace allows us to much more easily see at-a-glance how the HTML is structured.

However, be careful to close (`</tag>`) the nested tag before closing it's parent tag.

### Headers

One important type of tag is a header. Headers tell your visitors what your site is about. 
+ We also have subheaders we can use - our header tags range from `<h1>` through `<h6>`, which range from largest to smallest.

### Other Tags
+ `<p>` tags, delineate paragraph text
+ `<strong>` will make any text contained within bold
+ `<em>` will italicize text or add *emphasis* 

#### Lists
+ Bullet point lists start with `<ul>` for *unordered list*
+ Numbered lists (computer will automatically count up from 1) start with `<ol>` for *ordered list*
+ The actual list items go between `<li>` tags for, you guessed it, *list items*

#### Links
Links use an `<a>` tag, which stands for *anchor*. If you wanted a link to Google it would look like this:
```html
<a href="http://www.google.com">Super secret link</a>
```
Notice that the `<a>` tag has an `href=""` attribute! href stands for *hypertext reference*. This is where the link will tell the browser to go when clicked. The text between the opening and closing tags are what the user will see.

#### Images
Images use an `<img>` tag to embed an image in a webpage.
```html
<img src="your_image_location">
```
The `src` attribute can be a URL of an image from the Internet or a relative link to an asset on your computer.

## Practice

### Adding sections
For your new website about a thing you love, create three sections describing why you love that thing using the following format:
+ a subheader for the top (using h2-h6 tags)
+ a `p` tag with a short descriptive paragraph
+ an image that goes along with the thing 
+ a link to somewhere on the web where I can find more information about the topic. 

### Adding pages
Add pages to your site by creating three separate html files 
+ Start each page with the proper HTML tag structure (`html`, `body`, `title`, ...)
+ To link to pages in the same site, use an `<a>` tag.
+ Put links in an unordered list using `ul` and `li` tags

## Conclusion / So What?
HTML allows us to define and label the content of our page. Across browsers, there isn't a specification about how text without tags should be rendered. You have no control over how it's displayed, and in future versions of a browser, your code might not be displayed.

## Hints and Hurdles
+ An HTML element is composed of an opening tag, content, and a closing tag
+ Students should have their HTML files in both the browser and in the text editor. 

