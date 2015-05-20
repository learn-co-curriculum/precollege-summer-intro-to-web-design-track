### Objective
Students will understand the purpose of git and github, understand how to commit locally and push to a remote repository

###SWABTS

+ GIT - `add` and `commit` files to local repository
+ GITHUB - `push` and `commit` to a remote repository. Submit a pull request.

### Motivation / Why Should You Care?
It’s time to bring all of your individual pieces of the student project together. To do that we are going to need to track your progress locally in `git`, then push up your code to Github.

### Lesson Plan
+ Git and Github aren't the same thing
  * Github: where we save our code in the cloud, while `git` is a version control system that lives on your computer.
+ In terminal, enter `git status`. Like saying "hey git whats up?"
+ Want all files to go on Github, so `git add file_name`.
  * If it's a lot of files `git add .` will add everything
+ Enter `git status`: now says files that are ready to be committed.
+ In terminal: `git commit -m "summary of work"` (Commiting is like taking a snapshot of your entire codebase)
+ `git remote -v`: tells us where on Github.com the code will live
+ In terminal `git push`. Sends code to Github.
+ Pull request: Jr. Devs can't submit code without review.
  * Click the `Pull Request` button in the top right corner and confirm.

### Conclusion / So What?
This is the exact workflow for developers at every tech company. Every time you get work done, you git add, commit and push to save the state of your work. Then to get your code pulled into a master code base we have to get it approved.

