# Lubin Laboratory - MELT Team Software Github Workshop
Demo Repository to Teach Git and GitHub

## What is Git and Github?
* Git: Software to track changes to code 
* Github: A place to store code

## Why Use Git and Github?
* Quicker and easier to collaborate on code and projects
* Create "checkpoints" and maintain a version history in case something goes very very wrong (it's saved me before, trust me)

## Prerequisites
* A Github account
* Git software (https://git-scm.com/downloads)
* A repository to you are the owner of/are a collaborator
    * If you want to be added as a collaborator
        * Ask the owner of the repo to go to "Settings" -> "Manage Access" -> Add you as a collaborator

## Terminology
* Command Line/Terminal - If you're familiar with Python, it'll be where you run all the `pip install` commands. On Windows, you can use cmd or powershell as well.
    * All `git` commands will be run in the terminal
* Directory - Where you currently are working on. In the terminal, you'll see something along the lines of: `PS C:\Users\Dylan Vu\Visual Studio Code Projects\Projects\MELTGithubWorkshop>` before where you can type in the terminal. That is your current directory that you're working in.
* Path - If you are on Windows and go on file explorer, if you click on the top you'll have a URL-equivalent on the computer. For example: `C:\Program Files`
* Repository/Repo - where the code is stored online
    
    To obtain a copy of the repository on Github:
    * Go to the repository and hit the green "code" button near the top
    * Copy the link on HTTPS
    * Open up your terminal and change directory to where you want to create this repository on your device
        * On Windows: to change directory, copy the path. In the terminal: `cd "PATHHERE"`

            For example: `cd "C:\Users\Dylan Vu\Visual Studio Code Projects\Projects\"`

    * Paste that link in the terminal: `git clone PASTEITHERE`
    
        For example, if you were cloning this specific repository: `git clone https://github.com/vu-dylan/MELTGithubWorkshop.git`
* Branch - Your own workspace, essentially
    
    To create a branch:
    
    `git branch mybranchnamehere`
    
    `git push mybranchnamehere`
    
    To switch branches to mybranchnamehere: `git checkout mybranchnamehere`
* Main - Master copy of working code
* Committing - the "checkpoint"
* Pushing - updating the code on the repository

## Basic Workflow
This PDF has pretty much everything you'd need for commands: https://education.github.com/git-cheat-sheet-education.pdf

0. `git status` is super helpful. It tells you what files you haven't added yet, what files you have, and what branch you are on.
1. Add - "stating" what you will save
    
    Run: `git add FILENAME.EXTENSION`
    
    For example: `git add README.md`
    
    If you want to add all files in the directory: `git add .`
2. Commit - "saving" what you changed
    
    Make sure your code is saved locally on your computer. On VS Code, hit CTRL + S on Windows.
    
    Run this command: `git commit -m "commit message here"`
    
    For example:
    
    `git commit -m "fixed bug where script does not correctly run in main.py`
    
    `git commit -m "optimized runtime of myscript.py`
    
    These messages can be valuable if you ever need to revert back to a previous version of your code. You'll know exactly what was changed/what version you are looking at.
3. Push - "updating" GitHub
    
    Depending on what branch you are on, you have to push to that branch. So if you were editing on mybranchnamehere: `git push origin mybranchnamehere`
    
    If you are on main: `git push origin main`
4. Merging with main (assuming you are a collaborator. If you are not, you have to submit a pull request)
    
    First, update your own branch by adding, committing, and pushing to your branch
    
    Then switch to main: `git checkout main`
    
    Then merge:
    
    `git merge mybranchnamehere`
    
    `git push origin main`
5. Sometimes: pulling from main
    * If someone else edits a branch (main included) that you are working on, you have to update your local copy of the code.

        For example:
    
        `git pull origin main`
    
        `git pull origin mybranchnamehere`
6. Fixing merge conflicts
    
    If two people edit the same lines of code at once, Git doesn't know which is the "correct" copy. So you will get a merge conflict. If this happens, you have to open up the file on your computer, fix the conflict, commit, and then push again


## Testing out GitHub

Test

# This is Dylan
