#Day-01: Command Line

_A full lecture is available [here](LECTURE.md)_

## Objective

Students will be able to navigate their system’s file structure using the CLI (command line interface) in terminal.

## SWBATs


#### CLI
* Command line interface 
* Understand and explain what a terminal is and why we use it
* Navigate and manipulate directories

## Motivation / Why Should You Care?

Back in the day (the 1980s!), computers only had a terminal to control them. Later on, Graphical User Interfaces (GUIs) were created to make computers more accessible (like for your computer-illiterate grandparents). Developers continue to use the terminal instead of the GUI because it speeds up development and allows for more granular control.


## Lesson Plan

***Any students that have done this lesson before should do the advanced [CLI Bash Scripting Lab](https://github.com/learn-co-curriculum/hs-advanced-cli) ***


### Lesson Plan

You're going to learn about the command line by planning for a trip. 
+ Open your terminal. You’ll see a tilde: `~`. This means you’re in your user's home directory.
+ Enter `pwd`. Explain `pwd` means print working directory.
+ Let’s change directories. First check what directories are within the directory where you are standing by using `ls`.
+ Show students how to change directories by using the `cd <directory-name>` command. Change to `desktop` directory.
+ Show students how to make a new directory `mkdir development`.
+ Show students how to make a new directory in `development` called `trip`. Check and see that the directory was made by using `ls`.
+ Show students how to...
  + create text files for landmarks you want to visit in the cities directories by using `touch`. 
  + remove a file that they longer want using `rm`.
+ Place a file in the wrong directory, then show students how to move it with `mv`.
+ Students practice moving up the tree using `cd ..`.

## Conclusion / So What?
+ As we learn to build complicated applications, being able to swiftly navigate your computer using the command line will make your life much easier. The command line will be important not just for navigation, but you'll also use it to do things like boot the local server for your web apps, write scripts to automate tasks, and execute other important functions on your computer.

## Hints and Hurdles
+ Navigating your computer from the command line is a lot about muscle memory. It's important that students get a lot of repetition in with these commands.

## Additional Media
+ It might be fun for the class to play around with these [CLI easter eggs](https://github.com/learn-co-curriculum/hs-cli-cultural-piece).

