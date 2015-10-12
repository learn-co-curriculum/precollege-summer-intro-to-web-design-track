# DAY-06 Using Selectors

_A full lecture is available [here](LECTURE.md)_

## Motivation/Why Should You Care? 

We've seen how powerful jQuery can be, but the syntax can be a little hard to pick up. Let's practice together to start getting the hang of it. 

## Lesson Plan

### Selecting an Element

+ Open Google Chrome and navigate to [beyonce.com](http://www.beyonce.com)
+ In the toolbar, click "View" > "Developer" > "Javascript Console"
+ Let's write some jQuery. What do we type to tell jQuery "hey, jQuery, wake up"?
+ Go ahead and type a dollar sign. Next, in parenthesis, we need a selector. Let's see if we can figure out what text the h1 has. 
+ Type `$( "h1" )` and press enter. 
+ Boom! There's our h1!

### Modifying an Element

+ So we can now select an h1 element. What if I want to know what text it contains? I can do this by calling a jQuery method on the element. 
+ We can get the text from the h1 by using `.text()`
+ We'll type `$( "h1" )` to select the h1 tag. Next, we'll add `.text()` - the whole thing looks like `$( "h1" ).text()`
+ Go ahead and press enter - you should see the text that's contained in that h1! 
+ If we want to, we can change the text by putting it in the parenthesis at the end of our method. 
+ Type: `$( "h1" ).text("Flatiron Rules!")`
+ There's a lot going on here, can someone explain to me all of the steps?

### Bonus Fun - Animation Methods

+ Do you guys want to see something cool? jQuery has lots of great animation methods built into it. Try selecting our h1 again, but this time call the `slideUp()` method on it. 
	* `$( "h1" ).slideUp()`
+Take a few minutes to try out some other jQuery methods. Feel free to use the documentation, or use Google to find more. 

