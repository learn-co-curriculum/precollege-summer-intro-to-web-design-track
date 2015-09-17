#DAY-01 Student Directory Project

_A full lecture is available [here](LECTURE.md)_

## SWBATs
***Students will create their own profile page using HTML!***

### Motivation / Why Should You Care?

+ Start with an altered tweet from Justin Bieber on the screen using the dev tools that says “I LOVE FLATIRON SCHOOL AND CODING. EVERYONE SHOULD ATTEND AFTER SCHOOL.”  
  * Let them know by the end of the lesson they'll learn how we did that.
+ Ask students for their favorite websites and bring it up on the screen and click `view source`
+ Web pages are made up of two things: HTML and CSS. First we're going to start with HTML. HTML, hypertext markup language, is the structure and content of a web page. All it does is tell the browser what different types of content is on the page through "Semantic tags".


### Lesson Plan
Today, we'll be building a student directory with all of your profile information on it. By the end of this project, you'll have deployed live, working code to the internet the same way professional web developers do. [Lab: Student Directory Project](https://github.com/learn-co-curriculum/hs-intro-web-student-directory)

+ `cd` into this new directory we just cloned and open up the entire thing in your text editor
+ Open up index.html in your text editor - then right click on the page and click `open in browser` 
  * Click on the sample student to see what your personal profile page will look like
+ Walkthrough of the directories and files in this directory. I’m going to go from the bottom to the top. 
+ `README.md`: holds instructions on how to complete the lab
+ `index.html`: It is standard convention to name a home page index.html. 
+ `students` directory: It’s going to hold all of the individual files for each of your profiles. 
+ In terminal from inside the main directory for this project:
  * Create a new file that is named like this ‘vanessa-dean.html’ except with your own name in 'students' directory.
+ `css` directory: holds all of the files in charge of styling our pages (We will learn more CSS next class)
+ `img` directory: You are going to be adding an image of your face and also a background image inside of the `students` 
+ `js` directory: You’ll be learning more about javascript later in this course
+ open `student-profile.html` and copy all of the code there and paste it into your new `your-name.html` file

+ `<!doctype html>`:  tells our browser we're using HTML5 
+ `<html>`: opening HTML tag. Closing tag `</html>` is at the bottom.
+ Opening a closing tags create little baskets. Inside of this html basket we are going to nest all of our html.
+ `<head> </head>`: The head of our document is where we store all of the meta data -- information that the browser needs, but that your users don't necessarily need to see or know about. 
+ `<title></title>`: shows text in the tab in the browser
+ `<link>`: link to stylesheets
+ `<body></body>`: 
  + `ids` and `classes`: use these to help with CSS
+ Header: Comments mark the header
  *This grayed out text is called a comment.
+ `<h4></h4>`: header tags
  * h1-h6
+ `<a href="#"></a>`: link.
  * `href=""` attribute. hyper-reference - where the link goes
+ `<div></div>`: invisible box that clumps content together
+ `<p></p>` paragraph tags. 
+ `<ul></ul>`: unordered list.
+ `<li></li>`: list item. 
+ Scroll to where you see the comment: `<!--Begin Splash Image-->`
+ `<img>` tag:
    * `src="#"`: attribute of the img tag. stands for source
+ Students save a photo of themselves in the `img/students` directory and change the `src` 

##Stretch Activities 

Some students may have already taken the course or are familiar with the basics of the command line and git. Here are some ideas and stretch concepts you can use to continue to challenge students like this during this exercise.

+ Once students have finished editing their student profile pages and their profile menu page have them merge their repositories together with another student. This is a good chance to work through merge conflicts. 

+ Challenge students to add further customization to the profile page with background colors, custom CSS and fonts.

+ If students are comfortable with the command line, give them the Clmystery lab. 

## Conclusion / So What?
HTML makes up every single page on the internet. You can't create a web page without it. 

## Hints and Hurdles
+ Indentation does not matter to our browser when it reads the html and displays it but it is SUPER important for humans reading our code.
