#JavaScript Basics - Full Lecture

##SWBATs
+ Understand comparison and logic operators
+ Use conditional statements to control program flow (if/else and switch)


## Motivation
Let's say we want our code to be event based so that an input triggers one flow and one specific output, as opposed to a different input, so that we're not always manually calling all of our methods. For example, when the time is 12am, we get tired and go to bed. When the time is 10am, we're awake.

What if we wanted to set an alert to have our computer wake up up every morning at 7:30am. The way you would tell your computer is that __if__ it's 730am then send an alert, otherwise do nothing.

##Lesson Plan

### Conditional Statements
+ Who here has done if-then statements in math class? This is a conditional statements
+ A conditional statement is a set of commands that executes *if* a specified condition is `true`. 
+ JavaScript supports two conditional statements: `if-else` and `switch`.
+ Use the `if` statement to execute a statement if a logical condition is `true`. Use the optional `else` clause to execute a statement if the condition is `false`. An `if` statement looks as follows:

```
if (condition)
  statement_1
[else
  statement_2]
```

+ Example:
```js
var gasTank = 34; //gallons of gas

if (gasTank === 34) {
   console.log('Tank is full');
} else {
    console.log('Tank is not full');
}
```

+ You can see that there are a few syntax details that you'll need to pay attention to. What is syntax? Syntax is like the grammar of a programming language. There are certain conventions that you need to follow in order for your program to run properly.
  + JS requires that the conditions in your `if` statement be surrounded by `()`
  + You’ll need to encapsulate your conditional statement with `{}
  + **almost** every line of JS ends with a `;`


### Comparison Operators

+ You can also see that we have a funny looking triple equals `===`. This is how we compare the values of two things. One equal to assign value, triple equals to compare values. We're checking if they're equal in value and datatype.
+ Here is a list of all of JS comparison values and what they do

<img src="https://s3.amazonaws.com/after-school-assets/jquery2.png">

### Complex Conditionals

+ We can add additional branches to a conditional statement with the `else if` keywords like this:
```js
  if (gasTank === 34) {
     console.log('Tank is full.');
   } else if (gasTank > 34) {
      console.log('Oops, tank is overfilled!');
   } else {
      console.log(’Tank refill mandatory!');
   }
```
+ We can also make more complex conditional statements with logical operators, like this:
```js
  if (gasTank === 34) {
      console.log('Tank is full.');
   } else if (gasTank > 34) {
      console.log('Oops, tank is overfilled!');
   } else if (gasTank < 34 && gasTank > 5) {
      console.log(’Tank refill suggested.');
   } else {
     console.log(’Tank refill mandatory!');
   }
```

### Logical Operators 

+ Here is a list of all the Logical Operators and what they do:

<img src="https://s3.amazonaws.com/after-school-assets/jquery3.png">

### Linking to HTML and websites

+ What do I do with my JavaScript. You write out your JS in a `.js` file and require it in your HTML files like this:
  + `<script src="js/myScript.js"></script>`
+ *Go to Learn.co and get some practice using JS with the Donut App lab.*



##Conclusion
Conditional statements let us control the flow of our programs. It let's us trigger different outcomes based on certain inputs from a user. Think about how a calculator might work: if a user enters `+` then the calculator performs addition. That's control flow in action.
