##Command Line - Full Lecture

### SWBATs

Objective: Students will be able to navigate their system’s file structure using the CLI (command line interface) in terminal.

#### CLI
* Understand and explain what a terminal is and why we use it
* Navigate through directories using relative and absolute paths
* Use the `cd` command to move up and down directories
* Use the `ls` keyword to list items in a directory
* Remove a file and a directory by using `rm` and `rm -rf` keywords
* Move files and directories using the `mv` command


### Motivation / Why Should You Care?
Back in the day (the 1980s!), computers only had a terminal to control them. Later on, Graphical User Interfaces (GUIs) were created to make computers more accessible (like for your computer-illiterate grandparents). Developers continue to use the terminal instead of the GUI because it speeds up development and allows for more granular control.

### Lesson Plan
***Any students that have done this lesson before should do the advanced during this lecture [CLI Bash Scripting Lab](https://github.com/learn-co-curriculum/hs-advanced-cli)***

#### The Backstory
You've been recruited by MI6 as the next 007. The name's Bond. James Bond. The idea is to loosely follow the plot of one of the Bond movies...have fun with it and take students input of what your mission should be. The idea is that Bond should go to different cities and then specific locations in that city and then within that location he needs to recover classic 007 artifacts like a microchip with codes to hack into The Main Frame, a map with the location to a submarine carrying nuclear warheads, a Golden Gun, a bag of flawless, uncut diamonds etc. The mission is to get this item back into safe hands of Her Majesty's Secret Service.

+ Open your terminal. You'll see a tilde: `~`. This is the user's home directory.
+ Enter `pwd`. Explain `pwd` means print working directory.
+ Let's change directories. First check what directories are within the directory where you are standing by using `ls`.
+ Show students how to change directories by using the `cd <directory-name>` command. Change to `desktop` directory.
+ Students `mkdir dev`. 
+ Show students how to make a new directory in `development` called `mission`. Check and see that the directory was made by using `ls`.
+ Show students how to...
  + create directories for mission destinations within the `mission` directory. 
  + create directories for cities Bond will need to visit to track down the bad guy inside of the mission. create on directory called London, you'll want to get the weapon/stolen goods back into the hands of the good guy. make another called monte carlo.
  + create directories inside each destination city of the scene for your mission like a lavish casino, private island or abandoned nuclear testing site.
  + create text files the dangerous weapon/stolen goods you need to retrieve.
  + open the file in your text editor and add information about details about what it is you'll retrieve.
  + touch a villain file (like oddjob, goldfinger, jaws)
  + take out the villain with `rm`.
  + remove an entire directory using `rm -rf` once you've completed your task there.
+ Accidentally place a file in the wrong directory(you followed the wrong clue, it happens to even the most seasoned spies), then show students how to move it with `mv`.
+ Students practice moving up the tree using `cd ..`.
+ Important: directories only know what's directly inside of them.
+ Show students how to write out the relative path to each mission city from the mission directory.
+ Show students how to write out the absolute path to different files and directories.
+ Interactive Practice - have students...
  + use `cd  ..` to move to the mission directory.
  + create one mission city directory.
  + create two new settings directories inside the city directory.
  + create files of treasures to recover on the mission.
  + on your whiteboard, draw out the tree for each directory and file inside the trip directory.

### Conclusion / So What?
+ As we learn to build complicated applications, being able to swiftly navigate your computer using the command line will make your life much easier. The command line will be important not just for navigation, but you'll also use it to do things like boot the local server for your web apps, write scripts to automate tasks, and execute other important functions on your computer.

### Hints and Hurdles
+ Navigating your computer from the command line is a lot about muscle memory. It's important that students get a lot of repetition in with these commands.
+ In [Lab: Find The Missing Pets]( https://github.com/learn-co-curriculum/find-missing-pet), instructor should complete one or two examples before releasing students.

### Additional Media
+ It might be fun for the class to play around with these [CLI easter eggs](https://github.com/learn-co-curriculum/hs-cli-cultural-piece).
