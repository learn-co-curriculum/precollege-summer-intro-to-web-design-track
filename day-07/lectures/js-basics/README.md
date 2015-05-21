#DAY-07 JavaScript Basics

_A full lecture is available [here](LECTURE.md)_

##SWBATs

***Students will be able understand the fundamentals of JavaScript***
+ Display text in the console
+ Perform math with JS
+ Declare JavaScript variables
+ Declare JS constants
+ Understand JS datatypes
+ Execute string concatenate
+ Utilize string methods
+ Execute string concatenate
+ Understand datatype conversion and why/when to use it
+ Use different types of dialogue boxes like alert and prompt
+ Understand comparison and logic operators
+ Use conditional statements to control program flow (if/else and switch)

##Motivation
We've seen how we can use jQuery to manipulate the elements of a website. Now we are going to learn about the technology that jQuery is built upon, JavaScript. JavaScript is a coding language that is supported by every browser and allows developers to write code that can do amazing things on any platform.

##Lesson Plan

### Variables

+ A variable is like a bucket that we can store some data inside and then later change the data it stores.
+ You need to declare variables explicitly in JavaScript with the `var` keyword
+ Naming variables: start with letter a-z A-Z remaining 0-9 a-z A-Z, you can also use `_ `never use spaces ' ' or or illegal characters (! % ?)
+ For variable names consisting of multiple words you should use camelCase or snake_case (camelCase is generally what JS developers use by convention and is called that becauseTheLettersMakeHumpsInTheName)
+ I can refer directly to a variable and change its value using `=` symbol
+ We can also declare and assign a value simultaneously using comma separation.

### Math

+ JavaScript supports the basic math operators you would expect (`+`, `-`, `*`, `/`, `%`)

### Constants

+ A constant is like a bucket (variable) with a lid that is glued shut, and once you store a value inside it, you cannot change that value again.
+ Just like `var`, `const` is a keyword that declares a constant
+ `const` variables are often named with ALL_CAPS so that developers know not to try and change them

### JavaScript data types

+ Numbers: integers (whole numbers) like 2, floats (decimals) like 3.56789
+ Strings: (text) like 'hello' or "hello", anything within quotes
+ Boolean: true or false
+ null (empty)
+ undefined (not yet defined)

### Concatenation

+ JavaScript uses `+` symbol for math when surrounded by numbers, but when any content is a string, it will concatenate the text

### String Methods:

+ String methods can be called on a string to modify the string in some way. Usually you can figure out what a method is doing to do just based on its name.
+ Method Chaining is also possible with the output of one statement feeds into the next one.

### Data Type Conversion
	+ Concatenating empty string changes number to a string.
	+ `parseInt` changes a string to a whole number.
	+ Converting text to a number returns NaN (Not a Number)
	+ Converting text to a float returns the string as a number
	+ `parseInt` stops at whole number and ignores characters that are not numbers where as `parseFloat` maintains decimal values.

### Dialog Boxes and JS Console
	+ alerts (Outputs a string)
	+ confirm (Boolean values)
	+ prompt
	+ Log - reports the age they entered into the JS Console located in the developer tool window.

### Doing math with JavaScript: 
	+ Arithmetic Operators

### Shorthand Operators

| shortcut  | original  | 
|---|---|
| x += y  | x = x + y  | 
| x -= y  |  x = x - y | 
|  x *= y  | x = x * y  |
|	x *= y	| x = x * y|
| x /= y | x = x / y |
|	x %= y | x = x % y | 

### Conditional Statements
+ If-then statements are conditional statements
+ A conditional statement is a set of commands that executes *if* a specified condition is `true`. 
+ JavaScript supports two conditional statements: `if-else` and `switch`.
+ Use the `if` statement to execute a statement if a logical condition is `true`. Use the optional `else` clause to execute a statement if the condition is `false`. An `if` statement looks as follows:

+ You can see that there are a few syntax details that you’ll need to pay attention to. What is syntax? Syntax is like the grammar of a programming language. There are certain conventions that you need to follow in order for your program to run properly.
	+ **almost** every line of JS ends with a `;`

### Comparison Operators

+ You can also see that we have a funny looking triple equals `===`. This is how we compare the values of two things. One equal to assign value, triple equals to compare values. 

### Complex Conditionals

+ We can add additional branches to a conditional statement with the `else if` keywords like this:
+ We can also make more complex conditional statements with logical operators, like this:

### Logical Operators 

+Give a list of logical operators from LECTURE-NOTES

### Linking to HTML and websites

+ What do I do with my JavaScript. You write out your JS in a `.js` file and require it in your html files like this:
	+ `<script src="js/myScript.js"></script>`







