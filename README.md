# Introduction  
This repository is a practical guide to learning Git and GitHub commands. It helps you understand how to set up Git, manage repositories, work with branches, and collaborate using GitHub. 

## Table of Contents
- [Installation Check](#installation-check)
- [Git Setup](#git-setup)
- [Git Initialize & Clone](#git-initialize--clone)
- [Basic Workflow](#basic-workflow)
- [Undo / Fix Mistakes](#undo--fix-mistakes)
- [Branching](#branching)
- [Remote Repository](#remote-repository)
- [Merging Code](#merging-code)
- [Fixing Mistakes](#fixing-mistakes)
- [What is Forking?](#what-is-forking)

## Installation Check
    Show how to verify Git is installed: git --version


## Git Setup (use bash)
1. git config --global user.name "Your name"
2. git config --global user.email "Your email"

## Git Initialize & Clone 
git init            # Start a new Git repo in your folder  
git clone 'url'     # Copy a repo from GitHub to your system  

## Basic Workflow
1. git status                     => Check file changes in the repo
2. git add 'file'                 => Stage a file
3. git add .                      => Stage all changed files
4. git commit -m "Your message"   => Save staged changes with a message
5. git push                       => Upload commit to GitHub
6. git pull                       => Download latest changes from the GitHub
7. git log                        => Show commit history

## Undo / Fix Mistakes
1. git restore 'file'                # Undo changes in a file (restore unmodified version)
2. git restore --staged 'file'	     # Unstage a file (after git add)
3. git reset --hard                  # Delete all changes (⚠️ careful)

## Branching
1. git branch                # List branches  
2. git branch 'name'         # Create a new branch  
3. git checkout 'name'       # Switch to a branch  
4. git branch -M main        # Rename branch to main  
5. git checkout -b 'name'    # Create + switch branch  
6. git merge 'branch'        # Merge another branch into current  
7. git branch -d 'name'      # Delete a branch  

## Remote Repository
1. git remote -v                                    # Show remote links  
2. git remote add origin 'url'                      # Link local repo to remote  
3. git push -u origin main                          # Push main branch (-u = upstream)  
4. git push --set-upstream origin 'branch name'     # Create a remote branch  

## Merging Code
1. git diff 'branch name'   # Compare commits, branches, files & more  
2. git merge 'branch name'  # Merge another branch into current  

OR Get a PR(Pull Request)
    A Pull Request lets you propose changes and discuss them before merging into another branch or repository on GitHub.

## Fixing mistakes
Case 1: staged changes  
    i. git restore --staged 'filename'  
    
Case 2: committed changes (for one commit)  
    i. git reset HEAD~1  
    
Case 3: committed changes (for many commits)  
    i.git reset 'commit hash'  
    ii. git reset --hard 'commit hash'  

## What is Forking?
Forking is the method of copying a repository from an organization or another person into your own GitHub repository or profile. Fork is a rough copy.
