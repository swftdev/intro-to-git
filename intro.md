

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


