# New Project
This is a new project created from the local system.

# Git Setup
1. git config --global user.name "Your name"
2. git config --global user.email "Your email"

# Git Initialize & Clone 
1. git init => Start a new Git repo in your folder
2. git clone 'url' => Copy a repo from GitHub to your system

# Basic Workflow
1. git status => Check file changes in the repo
2. git add 'file' => Stage a file
3. git add . => Stage all changed files
4. git commit -m "Your message" => Save staged changes with a message
5. git push => Upload commit to GitHub
6. git pull => Download latest changes from the GitHub
7. git log => Show commit history

# Undo / Fix Mistakes
1. git restore 'file'	Undo changes in a file (unmodified version)
2. git restore --staged 'file'	Unstage a file (after git add)
3. git reset --hard	Delete all changes (⚠️ careful)

# Branching
1. git branch => List branches
2. git branch 'name' => Create a new branch
3. git checkout 'name' => Switch to a branch
4. git branch -M main => to rename branch
5. git checkout -b 'name' => Create + switch branch
6. git merge 'branch' => Merge another branch into current
7. git branch -d 'name' => Delete a branch

# Remote Repository
1. git remote -v => Show remote links
2. git remote add origin 'url' => Link local repo to remote
3. git push -u origin main => Push main branch (-u = upstream)