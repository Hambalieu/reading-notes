# Git Tutorial
-Git -Use to take snapshots of your code
-Its a version control system
-Multiple developers can work on the same code
-Collaboration is possible

**commit** 
-Represent each successive version of a file or files 
-commits are the Git equivalent of a "save as"
-You need to assign yourself messages to commits

**code for installing Git on Ubuntu**
-$ sudo apt-get install git

-After installing Git, users should immediately set the user name and email address, which will be used for every Git commit.

-Type the following into Terminal or Command Line:

-git config --global user.name "Hambalieu Jallow"

- git config --global user.email "example@email.com"

**Head**
-is the most recent save of your project

**Repository**
-Git pay attention
-One project = one repository but sometimes large projects may have more than one 

-**clone** from Github to Computer
-**Push** from computer to Github


-To import an existing project or directory into Git, follow these steps using the Terminal or Command Line:

-$ cd test (cd = change directory)
-$ git init
-$ git add *.c
-$ git add LICENSE
-$ git commit -m “any message here”


**cloning**

-code for cloning  $ git clone https://github.com/test mydirectory

*checking for file status*
-$ git status


*After staging one or multiple files, you should commit the changes and record what you did within the commit message:*
-$ git commit -m “made change x,y,z”

* to commit all files just use*
-$ git commit -a


**Pushing Changes** 
-CODE for pushing changes  $ git push origin master

**Notes**
-By running the git remote command, you can view the short names, such as “origin,” of all specified remote handles.


*For more information refer to the link below*
-[Git Tutorial](https://blog.udemy.com/git-tutorial-a-comprehensive-guide/)












