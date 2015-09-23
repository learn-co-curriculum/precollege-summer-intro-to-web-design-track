# Responsive Web Design - FULL LECTURE

## SWBATs
+ Explain the purpose of responsive web design
+ Use media queries to implement a responsive web design
+ Use `max-width` and `min-width` appropriately

## Motivation
+ Ever looked at a website on your phone and the text was so tiny and the layout so bad and it was hard to maneuver? It's a horrible experience.
+ On the flip side, ever been to a website that has a great mobile version? The text is readable on your phone, the layout is clean. Examples of this are:
  + [Google Maps](maps.google.com)
  + [Etsy](etsy.com)
  + [Buzzfeed](buzzfeed.com)
+ Isn't it much better to view a website with a mobile-friendly version? 
+ Some websites go so far as to build a desktop version of their site, and mobile version of their site (twitter.com v. mobile.twitter.com), but this means that every time you want to add a new feature, or redesign the page, you have to do it TWICE. thats twice as much work and twice and expensive.

+ Responsive web design allows you to build a website that looks great on any size browser, tablet or smart phone with just one code base. It's the smartest way to ensure that whatever browser size a user is using, they will love your site. Sweethatclub.org is a great example of a website that is fully responsive.

## Lesson Plan
+ We're going to use a 'Desktop Down' approach to responsive design, which means we're going to design our site to be optimized for the desktop, and scale down as the screen gets smaller for mobile. This might mean we have to remove some features. 
+ You can also use a 'Mobile Up' approach which designs for a mobile phone first, and scales up for a Desktop. This version typically adds features for a desktop, but we're going to follow the 'Desktop Down' approach

+ We've been hired as developers for a reggae music store. They want a responsive site that has a heading that spans the entire width of the top of the page, and then below that, three columns for Roots music, Dancehall music, and Dub music. When the page shrinks for a mobile phone, they want it to scale to one column, keeping the heading at the top and the music genres following one under the other.

+ Let's create a directory for this project, and call it `reggae_music`. Go ahead and make `index.html` and `style.css` files inside that directory.

HTML:
```
<div class="container">
      <div class="row">
          <div class="heading black-bk white-txt ">
              <h1>Jahstafari Tunes</h1>
          </div>
      </div>
      <div class="row">
          <div class="col-3 red-bk"> 
              <h2>Roots</h2>
          </div>
          
          <div class="col-3 yellow-bk">
              <h2>Dancehall</h2>
          </div>
          
          <div class="col-3 green-bk">
              <h2>Dub</h2>
          </div>    
      </div>
  </div>
```

CSS
```css
/*////////// Text & Box Styles //////////*/

.red-bk { background: red; }
.yellow-bk { background: yellow; }
.green-bk { background: green; }
.black-bk { background: black; }
.white-txt { color: white; }

/*////////// Grid System //////////*/

* { box-sizing: border-box; }

.container { 
    width: 90%;
    margin: 0 auto;
}

.row { 
    clear: both;
    margin-bottom: 2%;
}
.row:after {
    content: ".";
    display: block;
    clear: both;
    visibility: hidden;
    height: 0;
    line-height: 0;
}

.heading {
    with: 100%;
    padding: 20px;
}

.col-3 {
    display: inline-block;
    width: 33%;
    margin: 0;
    padding: 20px;
}
```
+ We have one big `div` with the class `container`. Inside of that, we have a `div` for the header with the `h1` "Jahstafari Tunes". The header is styled to take up 100% of the width of the screen, have a black background and white text.
+ Next we have a `div` with the class `row` and inside that, 3 `div`s for each music genre. Each of these genre `div`s are styled so that they take up 33% of the screen, display inline-block, and have different colored backgrounds.

+ Now that we have our desktop version, let's shrink our browser to see what happens the our code. It should look super messy. We want it all to stack, so now we need to add specific styling based on different sized browser windows.

CSS:
```css
@media only screen and (max-width: 700px) {
   .col-1, .col-3{
        float: left;
        width: 100%;
        padding: 20px;
        margin-left: 2%;
    }

  
}
```

+ `@media` is our call that we're defining a new media query
+ `only screen` sets up a condition that the query will only apply to specific size screens. It's considered best practice to include the `only` so that older browers that don't support media queries will ignore the command.
+ Because we're building from a Desktop Down approach, we set `(max-width: 700px)`, which basically says if the browser window is less than 700px wide, apply this styling below.
+ The styling we're applying is to float the heading and the music genres to the left and, set a margin of 2% and have them take up 100% of the width of the screen so they will stack on top of each other
+ This will prevent words stick out further than their backgrounds, and making boxes so small that text is no longer readable.


## Conclusion / So What?
+ responsive web design is crucial for designing a great experience for users across all browser sizes. In a world where people use different sized phones and tablets and computers, it's impossible to guarantee that all users will use one type of device. It's best to plan for all to be used

