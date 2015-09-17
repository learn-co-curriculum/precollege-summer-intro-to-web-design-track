# A Lot of Material To Get Through?
## And too many labs to chose from?

In order for Learn to mark a lab as complete, students have to push their work to GitHub and submit a pull request. Because all of that seems daunting, students can store their work on GitHub and automatically submit a pull request through the terminal command `learn submit`. 

If two or more students work together on a lab and all want credit for completion (and the work stored on everyone's Github), students can enter `learn submit --team comma, separated, list, of, github, usernames, from team`.

If Danny worked on a lab with Victoria and Lyel, he would enter in terminal in the lab directory: `learn submit --team vicfriedman, lresner`.

### Labs:
If students still need stretch labs for day one, have them move ahead to labs from day two.

+ `Find Missing Pets` - This lab is great practice for students to get comfortable moving around the terminal and learning about absolute v. relative paths. It's important to let students figure things out on their own (if they use cd to move around, and then move the image back each level manually before using paths), as long as they all end up using absolute or relative paths. This lab also has a test file `test.rb` that students can use to check their work. Just run in terminal `ruby test.rb` and the rests will run. Animals that are in the right place will appear in green.

+ `Sinatra Organizer` lab is more practice moving files that is less redundant for students. It can get stick because they don't know the Sinatra file structure, but early exposure is good. Nice to preface with "This structure will make way more sense next week".

+ `Bash Script` lab is an advanced lab for students who are really familiar with the terminal. Bash scripting is a language for writing bash commands in a file, and then running that file in terminal, so you can plan your actions before you take them.

+ `CLI Mystery` - This stretch lab is for advanced students to get familiar with even more Bash commands (like cat and nano) while they solve a mystery.

+ `Student Directory Project` - This idea of deploy on day one is a tradition in a lot of tech companies to get new developers to deploy code on day one, and a tradition of the Flatiron adult program. The goal of this exercise is to get students familiarized with HTML while creating their own profile page and feel the same pride to have their page deployed. Instructors do have to deploy the students pages.

+ `HTML Playground` - This lab is good for introductory material to let students make a Tumblr-like site and play with tags.



