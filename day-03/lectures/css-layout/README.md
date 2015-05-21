# DAY-03 CSS Layout 

_A full lecture is available [here](LECTURE.md)_

## Objective

Students will be able to use the box model to create cohesive page layouts

## SWBATs

+ Understand box model and how it is affected by padding, margin and border
+ Understand how to use box-sizing property to standardize the box-model across browsers
+ Use content overflow property - visible, hidden, scroll, auto
+ Understand inline vs. block vs. inline-block element displays
+ Understand how to use float and clear properties
+ Understand how to apply clearfix solution
+ Understand how to use CSS position properties - relative, absolute and fixed
+ Use background properties for box styling

## Motivation

Yesterday we used CSS to style the fonts, images and backgrounds of our page. Today we’re going to learn how to use CSS to break up and arrange the content on our page.

## Lesson Plan

### Box Model

 You probably want to set your `div`s to a certain width and height.
+ There are several important elements that go into determining the total size of the div though. These include:
	+ Margin - the space that you want between your divs
	+ Border - you might want to include a bold border around your div
	+ Padding - how much space you want between the edge of your div and the content inside your div
+ These sizing attributes are part of something that we call the box model.

+ Luckily we have a box-sizing property that allows us to choose which model we want to follow
+ There are a few different measurements that we can use to scale divs:
	* Fixed (px)
	* Fluid (%)
+ Fixed px (what we’ve been using) gives the developer a lot of control over what the user sees, but it is not flexible.
	* No matter what size the screen is the div will be the same size
+ A fluid design uses percentages. So width and height can be set to take up a certain amount of the screen.
+ Another option is set min and max width and heights.
+ ***[Demo](height.html) these things for students and have them practice/test.*** 

### Overflow Visibility 

+ If you do not set a height for a div it will automatically be tall enough to fit the content. If you set a height you have a few options for how you display the content with the overflow property.
+ Demonstrate how each of these (`visible`, `hidden`, `scroll`, `auto`) 
+ Have students practice with [this example](http://jsfiddle.net/flatiron_school/sFfw5/)

### Display Type

Most browsers display `div`,`p`,`h` in `block` style. That means that each element on the page will be displayed directly below the next one and take up the whole width of the page. 
+ There are a few other elements, such as `span`s and `img`s which display inline - meaning they show up side by side. 
+ We can change the default display property in CSS
+ Margins will overlap for block elements (above and below) but not for inline elements (horizontal)

+ The `inline-block` is sort of a combo of the other two - the content of each item stays seperate, but display inline next to each other. 

### Float

+ By using the `float` property with display: block; you should have good control over how things are displayed on the page
+ The float property accepts two values: right and left.
	+ ***[Demo](https://jsfiddle.net/qjjqv315/) how float works with three divs.***
+ Float only affects elements after it
+ One more thing to be aware of is collapsing parents.

### Positioning and Z-Index

+ We can also control the positioning of our divs more granularly with CSS positioning techniques like:
+ `relative` - will position a `div` relative to its parent
+ `absolute` - will position a `div` in absolute relation to the screen UNLESS it is within a `div` that is positioned in some way.
+ `fixed` - Will position the `div` at a fixed place relative to the browser window - even if the person scrolls down the fixed `div` will stay on their screen.
+ Let’s take a look at how this works with this [example](http://jsfiddle.net/flatiron_school/rgyPC/1/).
+ One last thing you can control when it comes to positioning is the `z-index` which lets you layer divs and control their position into the third dimension!
+ Divs with a higher z-index will be positioned on top of elements with a lower z-index or no z index at all.

+ Let’s take a closer look with this [jsfiddle](http://jsfiddle.net/flatiron_school/nWGts/ )

## Conclusion 
With CSS, we can controls the entire layout of our page, and how elements relate to each other.

## Hints/Hurdles
+ Make sure you are familiar with all the coding examples, or create your own examples before class. Layout can get tricky and CSS elements can compete with each other. It's easy to break things live and not be able to dig yourself out.
