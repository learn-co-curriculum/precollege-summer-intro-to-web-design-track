### Objective

Create a brand new HTML page from scratch using HTML5

### SWABTS

+ Structure an html page using `doctype`, `html`, `head` and `body` tags
+ Explain what goes into the head of the document
+ Add text to a page using `p` and `h1` tags
+ Add images using `img` tag
+ Add links using `a` tags and understand the difference between relative and absolute paths
+ Create multiple pages and link them
+ Create an ordered list using `ul` and `ol` tags
+ Include comments
+ Understand HTML elements that are deprecated and why they shouldn't be used
+ Create and understand when to use tables
+ Understand how to use HTML5 `audio` and `video` tags

### Motivation / Why Should You Care?

HTML is the foundational technology for the Internet, every one of your favorite websites is HTML at its core. 

Yesterday you used a prepared template to create personal pages for our student directory. Today you are going to learn how to create an HTML site from scratch, create your own styles for the page and deploy it to the world wide web with GitHub.

### Lesson Plan

#### Setup

*Students should be able to follow along with this demo*
+ In Nitrous terminal/command line from inside `development` directory make a directory (`mkdir`) called `my_website`
+ `cd` into that directory and make a `css` directory and an `index.html` file.
  * In terminal enter: `touch index.html`
  * In terminal enter: `mkdir css`
+ Add this HTML to `index.html`:

```HTML
<!doctype html> 
<html></html>
<head></head>
<body></body>
```

You are now have a blank HTML page that's ready to turn into anything!

#### Ideation

People make websites about all sorts of stuff:
+ [Corgis?](http://corgiaddict.com/) 
+ [Bacon?](http://www.royalbaconsociety.com/)
+ [Sanwiches?](http://fortheloveofsandwich.tumblr.com/) 
+ [Norwegian Olympic Curling Team’s pants?](https://www.facebook.com/NOCTP)

*Ask the students for some website ideas about things they love.*

#### Tag syntax
Every HTML tag has an opening and closing tag with its content in the middle. The tag names are contained within angle brackets, and a closing tag has a `/` before the tag name, like so:

```HTML
<tag>
    .... CONTENT GOES HERE ....
</tag>
```

Tags can also have attributes applied to them. These can be thought of as modifying or providing additional information to a tag. If `teacher` was a tag, it might have an attribute `subject` or `personality`.  A tag can have any number of attributes. These are placed in the opening tag like so:

```HTML
<tag attribute="attribute value" attribute2="2nd attribute">
    .... CONTENT GOES HERE ....
</tag>
```
Or with fictional `teacher` tag it would look like

```HTML
<teacher subject="coding" personality="super strict">
    .... CONTENT GOES HERE ....
</teacher>
```

#### Tag Nesting and Whitespace

Most tags can contain other tags inside of them. When we do this it is customary to indent the nested tags and their content by 2 or 4 spaces. This is to make it easier to read for humans. Computers only care that you close the tags.

*Bad indentation*

```HTML
<html><head><title>The end of the world as we know it</title>
</head><body><p>
Some text about things</p></body>
```
This is not only confusing but can also make it harder to find errors. *Can you spot the missing tag?*

*Good indentation*
```HTML
<html>
  <head>
    <title>
      The end of the world as we know it
    </title>
  </head>
  <body>
    <p>
      Some text about things
    </p>
  </body>
```
Using whitespace allows us to much more easily see at-a-glance how the HTML is structured.  *Can you spot the missing tag now that they all line up?* (closing `</html>` tag is missing.)

However, be careful to close (`</tag>`) the nested tag before closing it's parent tag. Let's show a bad example first:

*Bad closing order*
```HTML
<head>
  <body>
</head>
</body
```

This is wrong because we should close tags in the reverse order that we opened them. In our case we opened `<head>` then `<body>`, so we need to close them with `</body>` then `</head>`.

*Good closing order*
```HTML
<head>
  <body>
  </body>
</head>
```
Notice that when you do it right, the indentation/whitespace makes sense.

#### Headers

One important type of tag is a header. Headers tell your visitors what your site is about. Usually, the main title of pages uses the `<h1>` tag. 
 * Google looks for `h1` tags to figure out what a page is about. 
+ We also have subheaders we can use - our header tags range from `<h1>` through `<h6>`, which range from largest to smallest.

Netflix might use headers like this: 

```HTML
<!DOCTYPE html>
<body>
  <h1>Netflix</h1>
  <h2>Top Picks For You</h2>
  <!-- your top picks would be here! -->
  <h3>TV Shows</h3>
  <!-- TV Shows would be here! -->
  <h3>Comedies</h3>
  <!-- Comedies here! -->
  <h3>Horror</h3>
  <!-- Horror Movies here! -->
</body>
```

#### Other Tags

+ `<p>` tags, delineate paragraph text.
+ `<b>` will make any text contained within bold.
+ `<i>` ... Can you guess?

Lists
+ Bullet point lists start with `<ul>` for *unordered list*
+ Numbered lists (computer will automatically count up from 1) start with `<ol>` for *ordered list*
+ The actual list items go between `<li>` tags for, you guessed it, *list items*

```HTML
<ul>
  <li>item with bullet point</li>
  <li>2nd item with bullet point</li>
  <li>another list item</li>
</ul>

<ol>
  <li>Numbered item</li>
  <li>List item #2</li>
  <li>Third list item</li>
</ol>
```

Links
+ Links use an `<a>` tag, which stands for *anchor*. If you wanted a link to Google it would look like this:
```HTML
<a href="http://www.google.com">Super secret link</a>
```
Notice that the `<a>` tag has an `href=""` attribute! href stands for *hypertext reference*. This is where the link will tell the browser to go when clicked. The text between the opening and closing tags are what the user will see, "Super secret link" in this case.






+ Add the following to your page for each of the three reasons you love your topic:
  * a subheader for the top (using h2-h6 tags)
  * a `p` tag with a short descriptive paragraph
  * an image that goes along with the thing 
  * a link to somewhere on the web where I can find more information about the topic. 
+ Adding pages to your site: create three separate html files 
+ Inside of those files set up your html file structure
+ To link to pages in the same site, use a tag.
  * If site has `index.html` and `pig_facts.html` and theyre in the same directory, having a link from `index.html` to `pig_facts.html` looks like this: `<a href="pig_facts.html">click here for pig facts</a>`
+ Put links in an unordered list using `ul` and `li` tags
  * will style next class as a nav bar
+ HTML5 makes it super easy to embed video and audio into your website with these tags:
+ Audio:
  ```html
    <audio>
        <source src="audio.mp3" type="audio/mp3">
        <source src="audio.ogg" type="audio/ogg”> 
        <!-– fallback content here -->
    </audio>
  ```
+ Video
  ```html
    <video>
        <source src="movie.mp4" type="video/mp4">
        <source src="movie.ogv" type="video/ogg">
        <source src="movie.webm" type="video/webm”>
        <!-– fall back content here -->
      </video>
  ```
+ The fallback content is important because there are still old browsers out there that are not good at handling HTML5 audio and video elements.
+ Check out this great [resource](http://caniuse.com/) for checking out HTML5 compatibility
+ You can also embed YouTube video's really easily. Just go to the YouTube site for a video you like. Follow these steps:

<img src="https://s3.amazonaws.com/after-school-assets/YouTube-embed.png">

+ *Try adding an audio or video to your personal website.*


### Conclusion / So What?
HTML allows us to define and label the content of our page. Across browsers, there isn't a specification about how text without tags should be rendered. You have no control over how it's displayed, and in future versions of a browser, your code might not be displayed.

### Hints and Hurdles
+ An HTML element is composed of an opening tag, content, and a closing tag
+ Students should have their HTML files in both the browser and in the text editor. 
+ iTune encrypts audio files so they won't be able to be played with the audio tags. Students have to use legally acquired mp3 files - You can download Girl Talk's album for free [here](http://illegalart.net/girltalk/shop/)
