#JavaScript Basics - Full Lecture

##SWBATs

***Students will be able understand the fundamentals of JavaScript***
+ Display text in the console
+ Perform math with JS
+ Declare JavaScript variables
+ Explain the different between the JS datatypes
+ Execute string concatenation
+ Utilize string methods
+ Understand datatype conversion and why/when to use it
+ Use different types of dialogue boxes like alert and prompt

##Motivation
Now that we know how to design clear, clear and beautiful websites, it's time to start adding some pizazz. Have you ever been to a website that had a lot of animations going on? [Beyonce's website](www.beyonce.com) has some great examples of that -- the sliding menu and the image changing colors etc. All of this is achieved through a programming language called JavaScript. JavasScript is a really powerful language that can be used on the frontend for animations. In order to learn how to add those cool features to our website, we need to learn the JavaScript basics.

##Lesson Plan
+ We write JavaScript in a separate file - just like HTML gets it's own files and CSS in it's own files, JavaScript gets it's own - with the file extension `.js`. 
+ To practice JS, we're going to type our code in the Nitrous text editor, and then run it in the browser console so we can see the output of our code immediately. Have students follow the steps to open the JS Console:
	+ Go to any website in the chrome browser, and right click. Select `inspect element`. Once the Chrome Developer Tools are open, click `console`. You now have a live JavaScript console where you can type code and see the results. Think of this as a playground. Once you close the Developer Tools, you will lose all your work.

### JavaScript data types

+ All websites are made up of pieces of data. You can think of every piece of text or image on your website as a piece of data. We direct JavaScript to do different things with those pieces of data to create the animations. You can classify data in a few different categories, or datatypes:

+ Integers (whole numbers) like 2, 
+ Floats (decimals) like 3.56789
+ Strings: (text) like 'hello' or "hello", anything within quotes
+ Boolean: true or false
+ null (empty)
+ undefined (not yet defined)

Checking the data type:
+ `typeof` is a keyword that allows us to check the data type.
```js

typeof 1; //reports type of number 
typeof 'Yumm'; //reports type of string
```

### Variables

+ A variable is like a bucket that we can store some data inside and then later change the data it stores.
	+ The bucket has a name that is arbitrary but should make it easy for a developer to understand what goes inside
+ You need to declare variables explicitly in JavaScript with the `var` keyword like this:
	+ `var x;` 
	+ `var` is a keyword that declares a variable
+ Naming variables: start with letter a-z A-Z remaining 0-9 a-z A-Z, you can also use `_ `never use spaces ' ' or or illegal characters (! % ?)
+ For variable names consisting of multiple words you should use camelCase or snake_case (camelCase is generally what JS developers use by convention and is called that becauseTheLettersMakeHumpsInTheName)
+ Let's assign a value in x (remember we said var x; previously)
	+ `x = 10;`
+ I can refer directly to x and change its value using `=` symbol
+ We can also declare and assign a value simultaneously.
	+ `var y = 20;`
+ Declare and assign multiple variables at once using comma separation.
	```js
	var a = 1,
	b = 'heyy ke$ha', 
	c = 3;
	```

### Math

+ JavaScript supports the basic math operators you would expect (`+`, `-`, `*`, `/`, `%`) and can work with integers and floats
+ Anytime we see an equation in code JS will try to run the equations
	+ So `10*3` becomes `30` to the computer running your code.  
+ Perform math on variables
	```js
	var x = 10, 
	y = 20,
	myMath = x + y;
	//What does myMath equal? (30)

	x = 5;
	myMath = x + y;
	//What does myMath equal now? (25)
```

### Concatenation

+ JavaScript uses `+` symbol for math when surrounded by numbers, but what happens if we did this (adding an integer and a string together)

```js
var combine = '10' + 5;` 
combine; //returns "105"
// adding a string and an integer gives you a string
```

+ It seems like adding the string `'10'` plus the integer `5` gives us 105. When doing addition with one string, it will concatenate the pieces of data. 
```js
 "hey" + "danny"
  //returns "heydanny"
  "hey " + "danny"
  //returns "hey danny"
  '10' + '100'
  //returns 10100
```
If Boolean and a number: `true = 1` and `false = 0`. So `true + 2 = 3`… weird huh? This can produce unexpected results unless we are careful how we use `+` symbol. It's also good idea to be aware what data types are involved.

```js
true + "10"
//returns 110

false + "100"
//returns 0100
```

**Have students do `Interactive Practice: Variables`**

### String Methods:
+ So we've learned that we can add strings together - what else can we do with strings?
+ A method is prewritten set of instructions that our computer knows hows how to listen to and obey. 
+ We use methods that JavaScript gives us to manipulate and modify strings.
+ String methods can be called on a string to modify the string in some way. Usually you can figure out what a method is doing to do just based on its name. Some examples:
```js
//toUpperCase
	"Foobar”.toUpperCase(); //returns "FOOBAR"
//toLowerCase
	"Foobar".toLowerCase(); //returns "foobar"
//replace
	"Foobar".replace("bar", "baz"); //returns "Foobaz"
	"Foobar".replace(/o/g, "x"); //returns "Fxxbar
	//charAt
	"character".charAt(1); // returns "h"
	"character".charAt(7); // returns "e"
```
+ Method Chaining is also possible with the output of one statement feeds into the next one.
	+ `"Foobar".replace(/o/g, "x").toUpperCase(); //returns "FXXBAR"`

**Have students do `Interactive Practice: Strings`**

### Data Type Conversion
+ We already saw the weird things that happen when we try to add different datatypes together. There might be instances where 
+ `parseInt` changes a string to a whole number.
	```js
		combineStuff = parseInt('10') + 5;
		combineStuff; //prints 15
	```
+ What the heck happens if I try converting text to a number?
	```js
		var userName = parseInt('bob'); //returns NaN
		//NaN stands for Not a Number
	```
+ What if I want to convert to a floating number instead of an integer?
	```js
		var gallonsGas = parseFloat('10.25');
		gallonsGas; //reports 10.25 as number
	```
+ `parseInt` stops at whole number and ignores characters that are not numbers. 10xffffff same as 10.12345 becomes 10. Where as `parseFloat` maintains decimal values.

### Dialog Boxes and JS Console
+ alerts (Outputs a string)
	+ `alert('warning do not attempt to cook food using this website!');`
+ confirm (Boolean values)
	+ `var delete = confirm('Are you sure you want to delete this?');` //true or false
+ prompt
	+ `var age = prompt('Please enter your age: ');` //captures the value inserted.
+ Log
	+ `console.log(age);` 
	+ reports the age they entered into the JS Console located in the developer tool window.
	+ *ProTip: This can be a great way to show output of code as you're working. [JSbin](http://jsbin.com/?js,console) or similar editors usually have a console window

### Hints and Hurdles
+ Alerts don't work in Nitrous







