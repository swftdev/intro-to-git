

# Intro to Git
git is a version control tool. It allows you to manage your code over time. Where multiple versions of the code can exist. And you can go back to points in time to view what the code was.

## Setting up a new git repo
```powershell
# Make sure you are in the folder that you want to create the repo in.
# you can always run a git status to understand the repo status
# it will let you know if you are not in a repo

git status
# this should return 
# fatal: not a git repository (or any of the parent directories): .git

git init 
# you should see 
# Initialized empty Git repository in <folder location>

# At this point you have a .git folder that holds all the info needed for git to work
# you can see this with ls
dir -Force

```
***note*** don't nest repos, if you have a git repo don't create a new one inside of it.

## making a commit
```powershell
git status
# This shows that you have changes to the file you are not including yet

# A commit is a two step process, the first is adding a file / many files to the "stage"
git add intro.md

git status
# now you can see the changes have been staged

git commit -m "intial commit: added intro.md"
# this takes the things group in the stage and commits them with the message

git status
# now you can see the the working tree is clean with nothing new to commit
```

## creating a branch
```powershell
# We would like to make a branch to work on
# first we should ensure our local branch is up to date with changes from the remote
git pull origin main
# now if we see Already up to date. we know it's a good time to create a branch
# to create a branch
# git branch <branchname>
git branch develop
# check to make sure the branch was made, using
git branch
# now if you see you branch you can switch to it
# git checkout <branchname>
git checkout develop
```

