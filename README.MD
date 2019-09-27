## COM405 top tips GIT

Git is a version control system written by Linus Torvalds, the creator of Linux.

## Getting Started with GIT
Before doing anything else you will need to follow these getting started instructions.
This will teach you a little bit about git and how to fork a copy of this repository into your own github account.

You will then be able to clone your fork locally and then follow the instructions in the [maven-setup](../master/week1/maven-setup) project to get javac and maven working. 
After this you can then proceed to doing the exercises in [week1](../master/week1/).

### Introduction to GIT
To be a professional developer, you will need to become proficient at using version control systems.
Many version control systems (each with their own benefits and drawbacks e.g CVS, Subversion, git) have been popular over the years. 
Presently one of the most popular, git, was developed by Linus Torvalds to help with the collaborative development of the Linux Kernel.

In recent years many open source projects have migrated their code base to github (https://github.com) which supports a collaborative workflow for team development and sharing of source code using git. 

The principle advantage of git over other version control systems is that it is completely distributed. When you use git you clone a complete local copy of the repository you are cloning (usually referred to as the origin). You can develop code and save your changes in your local repository completely off line. At a later stage you may wish to push your changes to the on line repository or pull changes others have made into your local copy. 

There are many on line tutorials on using git and it will be worth while spending some time on these to get proficient. e.g.
 https://try.github.io/ Resources to learn Git
 https://guides.github.com/introduction/git-handbook/ Git Handbook 
 
Many IDE's including Netbeans support git natively, but it is very important to learn to use the git command line independently of the IDE so that you have more control over what is happening.

Using git successfully with a team can be complex but fortunately you only need to master a few commands to work on your own project
```
git clone  (a command to clone your local copy of the on line repository)
git status (a command to tell you what is the state of your local repository e.g are their any changes to commit and push)
git pull  (a command to pull the latest changes from the remote repository into your local copy)
git add --all (a command to stage all of the current changes ready for a commit)
git commit -m 'my commit message' (a command to commit changes to your local repository)
git push (a command to push your latest commits up to the remote repository)
```
### Forking the this repo
You could just clone with this repo and work on the clone locally. 
However you do not have write permissions to this repo and so you couldn't save (or push) any changes or work you have added.
Therefore, to be able to use the examples and save your own work, it will be better to create a copy (called a fork) of this repository in your own github account where you will be able to push and save your changes on line.

You should open your own personal github account and FORK this repository into your own account. 
This will give you your own copy to work with and a backup of your work on github.
PLEASE NOTE, while github is very reliable, you should also keep a backup copy of your repo in case anything goes wrong.

To create a fork of this repository
1. sign in to your own github account
2. navigate to this repository https://github.com/gallenc/com405
3. click the FORK icon

![alt text](../master/docs/images/ForkingARepo.png "Figure ForkingARepo.png")

you can understand the process by reading these documentation examples.
https://help.github.com/articles/fork-a-repo/

### checking out your own fork

Having forked the repository, go to your own github account and clone the repository into your own workspace on your machine. 
Rather than just clone the repository into a workspace on your IDE, it is good practice to create a separate folder on your local machine where you will clone your remote repositories. 
You can import separate projects from this clone into your IDE workspace as you need to work on them.

Create a git repo folder on your local drive and clone your fork of solent2Public into it.
```
mkdir gitrepos
cd gitrepos
git clone https://github.com/{your github id }/com405.git
```

You should now have a clone of your fork in your gitrepos directory gitrepos/com405.
you can now change directory (cd) into your folder
```
ls  # lists the files in the folder

cd com405   # cd into the git repository
git status  # show the files in the repository
```

## checking in your work

When you have finished your work you need to check it in.
Always do this at the end of class.
```
cd com405
git add --all
git commit -m 'write a first commit message'
git push
```

