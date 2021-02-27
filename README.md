# Lubin Laboratory - MELT Team Software Github Workshop
Demo Repository to Teach Git and GitHub

## What is Git and Github?
* Git: Software to track changes to code 
* Github: A place to store code

## Why Use Git and Github?
* Quicker and easier to collaborate on code and projects
* Create "checkpoints" and maintain a version history in case something goes very very wrong (anecdote)

## Prerequisites
* A Github account
* Git

## Terminology
* Repository - where the code is stored online
    
    To obtain a copy of the repository:
    * Go to the repository and hit the green "code" button
    * Copy the link on HTTPS
    * Open up your terminal and paste it in:
    
    `git clone PASTEITHERE`
    
    For example, if you were cloning this specific repository:
    
    `git clone https://github.com/vu-dylan/MELTGithubWorkshop.git`
* Branch - Your own workspace, essentially
    
    To create a branch:
    
    `git branch mybranchnamehere`
    
    `git push mybranchnamehere`
    
    To switch branches to mybranchnamehere:
    
    `git checkout mybranchnamehere`
* Main - Master copy of working code
* Committing - the "checkpoint"
* Pushing - updating the code on the repository

## Basic Workflow
This PDF has pretty much everything you'd need for commands: https://education.github.com/git-cheat-sheet-education.pdf
1. Add - "stating" what you will save
    
    Run:

    `git add FILENAME.EXTENSION`
    
    For example:
    
    `git add README.md`
    
    If you want to add all files in the directory:
    
    `git add .`
2. Commit - "saving" what you changed
    
    Make sure your code is saved locally on your computer. On VS Code, hit CTRL + S on Windows.
    
    Run this command:
    
    `git commit -m "commit message here"`
    
    For example:
    
    `git commit -m "fixed bug where script does not correctly run in main.py`
    
    `git commit -m "optimized runtime of myscript.py`
    
    These messages can be valuable if you ever need to revert back to a previous version of your code. You'll know exactly what was changed/what version you have.
3. Push - "updating" GitHub
    
    Depending on what branch you are on, you have to push to that branch. So if you were editing on mybranchnamehere:
    
    `git push origin mybranchnamehere`
    
    If you are on main:
    
    `git push origin main`
4. Merging with main (assuming you are a collaborator)
    
    First, update your own branch by adding, committing, and pushing to your branch
    
    Then switch to main:
    
    `git checkout main`
    
    Then merge:
    
    `git merge mybranchnamehere`
    
    `git push origin main`
5. Sometimes: pulling from main
    * If someone else edits a branch (main included) that you are working on, you have to update your local copy of the code.
    
    `git pull origin main`
    
    `git pull origin mybranchnamehere`
6. Fixing merge conflicts
    
    If two people edit the same lines of code at once, Git doesn't know which is the "correct" copy. So you will get a merge conflict. If this happens, you have to open up the file on your computer, fix the conflict, commit, and then push again


## Testing out GitHub

Test

# This is Dylan
