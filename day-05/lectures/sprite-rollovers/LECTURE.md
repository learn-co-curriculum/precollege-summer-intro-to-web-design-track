# Sprites and Rollovers - FULL LECTURE

## SWBATs
+ Explain what an image sprite is
+ Explain what a sprite rollover is
+ Implement an image sprite with CSS

## Motivation
+ Ever been to a website where some action happened when you rolled your mouse over an image? Maybe the image moved or text appeared? Pretty cool right? Sorta seems like magic. But it's much more simple than that. It's all done with CSS!


## Lesson Plan

+ Show students this [JS Fiddle example](http://jsfiddle.net/flatiron_school/jc2QR/).
+ This is the image for that [walking man ](http://orig12.deviantart.net/1b2d/f/2012/295/e/c/john_sprite_sheet_part_1_by_blahjerry-d5imaq2.png)

+ This image is considered an image sprite. It's one png that contains 50+ images in one. Sprites are typically used in navigation items when the nav links are all images. Image a navigation bar with 10 images. That would be 10 different HTTP requests to load each image. It can make your website really really slow.

+ In the example in JS fiddle, we only see one of the boys in the image due to the CSS. But when we roll our mouse over the image, the original boy is hidden, and we see a running boy, which is known as a state change. The original image has changed states. That is a sprite rollover.

+ It is necessary to do a rollover with a sprite because the state change on the rollover could take too long is the second image had to load when the mouse rolled over the original image. The magic with the sprite rollover is how quickly it happens. It wouldn't be quite so cool if you had to wait two seconds.

+ let's build our own! In your `development` directory, create a directory called `sprites-practice`. Inside that directory a file called `index.html` and another `style.css`

+ We'll be using this [image sprite](https://s3.amazonaws.com/after-school-assets/GravitatorSprites.png)

HTML:
```html
<a href="www.google.com"></a>
```

First we create a link on the page. We're going to add the sprite as the background image of this link, but we can still click it and it will take us to Google.

Then, we added styling the the `a` tag in our css.

CSS:
```css
a {
    display: block;
    width: 42px;
    height: 75px;
    overflow: hidden; /* sets overflow outside the element to hidden */
    white-space: nowrap; /* prevent line breaks (text wrapping) */
    background: url(https://s3.amazonaws.com/after-school-assets/GravitatorSprites.png) no-repeat; /* set background image */
    background-position: -110px 0;
}
```
+ We `display` property to block so that the background image will actually show up on the page
+ We set the `width` to 42px and the `height` to 75px so that it is wide enough to only display one part of the sprite
+ We set `overflow` to hidden so that we don't see the rest of the image that is bigger than the 42x75 box we set for it
+ `white-space` set to nowrap prevents the image from breaking lines
+ `background` sets the background url to the image sprite, with the `no-repeat` property so the image doesn't repeat to fill the page
+ `background-position` handles the vertical and horizontal movement of the background position. This moves how far over to the right/left and up/down the 42px and 75 pixels moves.

Next, we need to use some more CSS to determine what will get shown when we hover:

```css
a:hover {
    background-position: -270px 0;

```

+ we use the selector `a:hover` which tells the browser, we want to apply this styling when we hover the cursor over the `a` tag.
+ We change the `background-position` to -270 0, which moves the visible image 270 pixels to the right, and 0 pixels from the top.

+ Save your changes, and refresh in the browser. You'll see the alien standing ready to jump. When you hover your mouse over the alien, you'll see him jumping with his arms in the air.

## Conclusion / So What?
+ Sprite rollovers are a cool and easy way to add fun additional features to your websites.

