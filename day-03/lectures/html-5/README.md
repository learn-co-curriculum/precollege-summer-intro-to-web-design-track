#### HTML

+ break up a page with divs
+ Understand how to use HTML5 semantic elements - header, footer, nav, etc.


### Motivation

We've already learned some of the basics of using html tags. Today, we're going to use semantic tags to break up and describe the content of our page. 

### Why Should I Care?

HTML code can be hard for a human being to read! Breaking up and describing our content makes it easier to collborate with other programmers. 

### Lesson Plan 


+ We've already learned about some html tags to identify content on our page. What are some of the different tags we know how to use? 
	* Let students call some out - p, h1, img, etc. 
+ But what if we have content that goes together? Say that I have an h1, p, and an image that go should stay together on my page. How can I tell my differnet tags that they're in a group together? 

+ We can break up a page with a generic sort of container called a div. Div is short for division - it's a very basic way of dividing up our page. We write it like this: 

```html
<div></div>
```
+ Inside of our divs, we can put any other tags that we want. h1, p, img, audio, video, even other divs. 
+ We can add `class`es and `id`s to these divs to style them however we want. Adding `id`s and `class`es is the only way to differentiate these generic div containers.
+ Problem is how does a computer know the different things that a div could contain?
+ HTML5 provides us with some helpful elements that we can use to break up our page and describe what each section is being used for. These are:
	+ `header`
	+ `footer`
	+ `nav`
	+ `aside`
	+ `section`
	+ `article`
+ These are effectively just `div` elements. You’ll still need to apply styles to these items like:
```css
	footer {
		background-color: purple;
		color: white;
		display:block;
		float: right;
}
```
+ But it is a little cleaner and saves you some time by eliminating the need to add a div with the class or ID footer.
+ Not all older browsers support these HTML5 semantic elements but in other cases they just show up as a normal `div` element
+ So how do we style these `div`s? Let's find out!!!