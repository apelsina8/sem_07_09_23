# Welcome to git: essentials guide

## Commands to use and what they do
1. git init - create local repository
2. git add (file) - see that the letter U is changed to an A (next to the file name on the left), that means the file is added and is being tracked

P.S. git add. - with the dot at the end - will automatically add all files to be tracked

3. git commit -m "Commit: what changed?" - save changes + message (detailing the changes - can be viewed in log)
OR
Save changes by pressing control + s
OR
At the top press file => auto save (make sure there is a галочка)

P.S. git commit -am "New commit message" - save commits without adding the file and changes first. Much quicker and more efficient.

4. git log - see my commits and the time they were made
- git log --graph - to see the log in a more visual way
- an even better graph is by downloading git graph, then to use it - choose the middle thing on the left, like branches seperating, then choose the almost last option, before the 3 dots, it is similar tovseveral lines with circles at the top, ta-da! In a new window - you can see the easiest to comprehend graph of your log: the commits and branches, next to each - their last commit saved.

P.S. press q to quit

5. git status - check if there are any unsaved changes or modifications from previous save

6. git checkout 
- first 4 symbols of a commit version in the log you want to transfer to - your previous versions (like if you messed up or want to change the stuff you did to create a better version)
- git checkout main - to get back to the most recent version (FYI for the professors it is master, not main)

7. git diff 
- 4b16 (first 4 symbols) - to see the changes made from the commit which symbols you typoed and latest version
- 4b16 188e (first 4 symbols of one commit and first 4 symbols of the other to compare the version - used when comparing not with the latest version in the log)

8. git branch - see all your branches and see which one you are in
- git branch vetka1 - create a new branch
- git checkout vetka1 - go to that branch
- git merge vetka1 (merge 2 branches - to merge with main branch - checkout to main first)
- git branch -d vetka1 - delete branch. Can only do that after you checkout from this branch to another one,like your main one,

P.S. to create a new branch and checkout at the same time using 1 line of code:
- git checkout -b vetka1

9. .gitignore
- to ignore a file, type in the name of it on the .gitignore file (that are on the left, so they are in the same folder, but you do not want to upload them for everyone to see, for example, whne uploading to the GitHub, to keep them private)
- if you want files of the same category to be ignored, for example: *.txt -if you want to ignore all .txt files...


## GitHub: add to an online repository (not local)
Step 1: create an account on GitHub & merge with your local computer
- allow access (seems scary at first)

Step 2: push local repository (my current file in VS code) to my online account
- copy-paste the 3 lines of code provided on GitHub

Step 3: edit your file on your online account - press pencil to edit, when you are done: press commit changes (do not forget to leave a message to commemorate the commit).

Step 4: git pull - to integrate the new version to your local repository.

New commands:
- git push
- git pull
- git clone (link to the fork code)
- cd (file name) - if using someone else’s, forking over their work.

P.S. to fork over someone else’s work and edit the code, find the account and code you are interested in, fork it, then press the copy code link. Enter that link in your VS code terminal after  the words **git clone**. Then cd the file to allow the computer to edit. Create a new branch and edit ONLY in that branch.