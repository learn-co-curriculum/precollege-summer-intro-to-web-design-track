###SWBATS
***Students will be able to understand the fundamentals of jQuery and incorporate them into their projects***

+ DOM - Explain what the document object model is and how we can interact with it
+ DOM - Understand the tree-like structure of the DOM
+ jQuery - Use proper syntax
+ jQuery - Use selectors and methods together to manipulate the DOM
+ jQuery - Use jQuery selectors - they are essentially the same as CSS selectors
+ jQuery - Understand what jQuery is - a library that helps us interact with the DOM
+ jQuery - Set up a document with jQuery

### Motivation/ Why Should You Care
jQuery is a powerful JavaScript library that controls all the magic you see on your page, from sliding menus to animations. [Beyonce](beyonce.com) has some amazing jQuery on her page.

### Lesson  Plan

+ The DOM, stands for document object model and it is a structural representation of our HTML in tree form. Like this:

<img src="https://s3.amazonaws.com/after-school-assets/jquery4.png">

+ This model enables us to modify the content and visual presentation on our HTML document with scripting languages such as JavaScript.
+ What kind of things can we do with JS + DOM.
  + Add/remove/hide/show HTML elements in the page.
  + Add/remove/change HTML attributes.
  + Add/remove/change  CSS styles.
  + Listen for key presses or mouse events upon Elements
  + Create events in the page.

<img src="https://s3.amazonaws.com/after-school-assets/tumblr_mo32apssfq1r8lg7to1_500.jpg">

+ We can select elements on the page like this:
  ```js
  // using “plain old vanilla” JavaScript
  document.getElementsByTagName("p");

  // using jQuery
  $("p");
  ```
+ And manipulate content like this:
  ```js
  // using “plain old” JavaScript
  document.getElementById("foo").innerHTML("hello world");

  // using jQuery
  $("#foo").text("hello world");
  ```
+ You can probably already see how jQuery is going to help simplify your life. Let’s dive right in to learning more about it.
+ So what is jQuery?
  + jQuery is a JavaScript library
+ What is a library?
  + A library is a  collection of code that extends the abilities and features of a core programming language, offering additional methods and often simplifying the process to build in that native language.
+ Why use jQuery?
  + It just works everywhere! jQuery has been written to solve many cross browser issues that exist in core JavaScript.
  + Terse code. You can often write fewer lines of code than you would in using core JavaScript to accomplish the same thing. Hence jQuery’s slogan “Write Less Do More”.
  + Popularity. jQuery is currently at the time of writing this by far the most popular JavaScript framework. That means more forums, more code sharing, and more plugins.
  + Easy extending methods. Coders can create and share their own custom plugins easily.
  + Familiar DOM selectors. If you already know CSS you’re a step ahead as jQuery uses all our familiar CSS selector statements.
+ Are their other JS libraries out there?
  + Yes, there are a lot each with their strengths and weaknesses and some are broad, while others suit specific purposes.
  + At the time of writing this, here are some other popular JS libraries and frameworks:
  + MooTools, YUI, Prototype, Backbone, Cappuccino, Sammy, Angular, Ext JS, Knockout, Dojo, MochiKit, The M Project, Embed JS, MobilizeJS…etc
+ To setup a document to run jQuery we must link to the jQuery core library first, just like linking your HTML and CSS! Imagine that JavaScript is like a pet dog. On it’s own it knows how to eat, sleep, and play. Loading jQuery is like teaching the dog new tricks such as roll over, fetch, etc… Imagine what would happen if we gave the command for our dog to fetch before we had taught it this trick (linked to jQuery). Therefore, we always link to the jQuery core library first.
+ Inside your `<head></head>`, remote link: 
`<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.8.2/jquery.min.js"></script>`
+ Inside your `<head></head>`, local link (downloaded from jquery.com):
`<script src=”js/jquery-1.8.2.min.js"></script>`
+ Inside your `<head></head>`, both using local as fallback solution:
```html
  <script src="https://ajax.googleapis.com/ajax/libs/jquery/1.8.2/jquery.min.js"></script>
  <script>window.jQuery || document.write('<script src="js/jquery-1.8.2.min.js"> <\/script>')</script>
  ```
+ jQuery syntax 
+ Here is an example of the syntax for using a jQuery method
  + `$(selector).method(parameters);`
  + `$` refers to the jQuery object.
+ `selector` asks jQuery to go out into the DOM (Document Object Model) web page and select an element(s). In jQuery we can use all of the familiar selectors we use in CSS yay!
+ `.method` these are various actions and commands attached to the jQuery object that allow us to do things like fade elements in an out or change the content of the DOM and much much more
+ `parameters` are options we can set for each method.
+ An example of real code:
  + `$('h1').css({'background':'yellow'});`
  + `$` refers to the jQuery object.
  + `h1` asks jQuery to go out into the DOM (Document Object Model) web page and select all `<h1>`.
  + `css` method applies some CSS upon the selected element(s).
  + `{'background':'yellow'}` changes the background color to yellow.
+ A few more examples of jQuery selectors:
  + Select Elements
    + `$('h1')`
  + Select ID
    + `$('#nav')`
  + Select Class
    + `$('.celeb')`
  + Select Attribute
    + `$('a[href^=http://]')`
  + Select Descendent(s)
    + `$('#nav li')`
  + Select Child(ren)
    + `$('#nav > li')`
  + Select Sibling(s)
    + `$('h3 + p')`
  + Select by position
  + `$('li:eq(1)')` //selects the second list item
+ A few examples of jQuery methods
  + Effects
    + animate(`, `fadeTo()`, show(), hide(),  slideToggle()
  + Events
    + click(), hover(), focus(), blur(), keypress()
  + Manipulation
    + addClass(), clone(), empty(), attr(), val()
  + Traversing
    + eq(), each(), has(), closest(), find()
+ If you want to do something to your DOM jQuery probably has a method for it. 
+ YOU DO NOT HAVE TO MEMORIZE ALL OF THE METHODS
+ Having an idea of what possibilities are available is useful, and familiarizing yourself with some that you will use from day to day is useful, unless you’re a jQuery guru you probably will not memorize every method. Fortunately we can look them up and see their usage at sites like:
  + [API](http://api.jquery.com/)
  + [Documentation](http://docs.jquery.com/)
  + Or nifty [cheatsheets](http://oscarotero.com/jquery/)
  + [and](http://overapi.com/jquery)
+ How will I know when to use jQuery versus core JavaScript?
  + Firstly, jQuery is written in JavaScript so you can think of them as variations of the same thing instead of two separate things. To help answer this, jQuery methods are useful for many things; however there are certain fundamental parts of JavaScript that we still need in order to make flexible web applications. For example jQuery on its own does not have method for declaring variables, functions, if statements, or doing math…
  + This means that we can get a lot more mileage by integrating jQuery with core JavaScript.
+ An example of JS and jQuery working together:
  ```js
  var x = 12, 
  y = 5,
  total = x + y;

  If (total === 17) {
    $(’p').text('Correct!');
  } else {
    $(’p').text('Incorrect.');
  }
  ```
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
+ You’ll notice that here we are calling the ready method on the `$(document)` object and that ready function takes an argument that is another function. This happens a lot in jQuery. One jQuery method that you will probably be using a lot is the `.click()` method.
+ The `.click()` method also takes a function as an argument - a function that describes what should be done when that particular part of the dom is clicked. Here is an example (demo this in jsFiddle):
  HTML:
  ```html
  <button id="alert">Push to Alert</button>
  ```
  JS:
  ```js
  $(document).ready(function(){
    $('#alert').click(function(){
      alert('hello there');
    });
  });
  ```
+ You can see that we have a button in our dom and when we click that button the .click method performs the action within the function that we’ve given as an argument.
+ We can get even fancier and include jQuery methods within the function. 
+ For instance - what if we want to add some text to our page every time the button is clicked? 
+ We can use a very handy jQuery append method. The append method will add HTML to any piece of the DOM indicated. 
  + For example if I add `<div id="alert-tracker"></div> `to my dom I can append “alert clicked!” every time the button is pushed and keep track of how many times the alert button has been pushed like this:
  HTML:
  ``html
  <button id="alert">Push to Alert</button>
  ```
  JS:
  ```js
  $(document).ready(function(){
    $('#alert').click(function(){
      alert('hello there');
      $('#alert-tracker').append("<p>alert clicked!</p>");
    });
  });
+ Pretty cool, huh! 
+ Now go get some practice with the labs on Learn.co!

### Conclusion
jQuery is magic.

### Hints and Hurdles
+ The `$` is like saying "hey jQuery, wake up. It's time for you to get to work"
