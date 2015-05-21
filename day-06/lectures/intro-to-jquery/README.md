##DAY-06 Intro to jQuery

_A full lecture is available [here](LECTURE.md)_

### SWBATs

***Students will be able to understand the fundamentals of jQuery and incorporate them into their projects***

+ DOM - Explain what the document object model is and how we can interact with it
+ DOM - Understand the tree-like structure of the DOM
+ jQuery - Understand what jQuery is - a library that helps us interact with the DOM
+ jQuery - Set up a document with jQuery
+ jQuery - Use proper syntax
+ jQuery - Use jQuery selectors - they are essentially the same as CSS selectors
+ jQuery - Use selectors and methods together to manipulate the DOM

### Motivation/ Why Should You Care

jQuery is a powerful JavaScript library that controls all the magic you see on your page, from sliding menus to animations. [Beyonce](beyonce.com) has some amazing jQuery on her page. Using Javascript and jQuery makes our pages interactive and awesome. 

### Lesson  Plan

#### Intro

+ So far, we've used HTML and CSS to structure and style our pages and present information to our users. However, it doesn't let our users interact with our page. 
+ We can do this with Javascript, a programming language built to run in a web browser, and jQuery, a Javascript library that gives us some awesome functionality for manipulating the DOM. 

#### The DOM

+ The DOM, stands for document object model and it is a structural representation of our HTML in tree form.
+ This model enables us to modify the content and visual presentation on our HTML document with scripting languages such as JavaScript.

#### jQuery Intro

+ We can use vanilla Javascript to manipulate the DOM, but it's a lot easier to use jQuery. 
+ jQuery is a JavaScript library
+ A library is a collection of code that extends the abilities and features of a core programming language, offering additional methods and often simplifying the process to build in that native language.
+ Why use jQuery?
  + It just works everywhere and it's much shorter to write than vanilla Javascript!

#### Setup

+ To setup a document to run jQuery we must link to the jQuery core library first, just like linking your HTML and CSS!
+ Inside your `<head></head>`, remote link: 
`<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.8.2/jquery.min.js"></script>`
+ Inside your `<head></head>`, local link (downloaded from jquery.com):
`<script src=”js/jquery-1.8.2.min.js"></script>`
+ Inside your `<head></head>`, both using local as fallback solution:

#### Syntax, Selectors, and Methods

+ jQuery syntax 
  + `$("selector").method(parameters);`
  + `$` refers to the jQuery object.
+ `selector` asks jQuery to go out into the DOM (Document Object Model) web page and select an element(s)
+ `.method` these are various actions and commands attached to the jQuery object that allow us to do things like fade elements in an out or change the content of the DOM and much much more
+ `parameters` are options we can set for each method.
+ **Write examples on the board from FULL-LECTURE and have students guess what they select**
+ **Write examples of jQuery Methods the board from FULL-LECTURE**
  + Note that to execute a method, you put `()` after it. That means, "hey, run this method now!"

#### Using jQuery and Javascript

+ How will I know when to use jQuery versus core JavaScript?
  + Remember, jQuery is written in Javascript - it's just an extension of the basic Javascript 
+ Set up steps for using jQuery in your websites:
  +  Include link to jQuery core library:
   `<script src="http://ajax.googleapis.com/ajax/libs/jquery/1.10.1/jquery.min.js"></script>`
  + Link to your custom js file
  `<script src=”./js/app.js"></script>`
  + Start your `app.js` with document ready command:
    ```js
    $(document).ready(function() {
       // your app code goes here.
    });
    ```
#### Events

##### Document Ready
+ You’ll notice that here we are calling the ready method on the `$(document)` object and that ready function takes an argument that is another function. This happens a lot in jQuery. 
+ Our javascript files often get loaded before any other elements on our page. 
+ That means we apply jQuery selectors before any selectors have loaded on our page, so nothing happens.

##### Click
+ One jQuery method that you will probably be using a lot is the `.click()` method.
+ The `.click()` method also takes a function as an argument - a function that describes what should be done when that particular part of the dom is clicked. 
+ We can get even fancier and include jQuery methods within the function. 
+ For instance - We can use a very handy jQuery append method. The append method will add HTML to any piece of the DOM indicated. 

### Conclusion
jQuery is magic - it lets users interactive with our pages in awesome ways.

### Hints and Hurdles
+ The `$` is like saying "hey jQuery, wake up. It's time for you to get to work"
