# mlops-bootcamp-git

In command prompt:

To know version of git
git --version 

Create a file locally and commit to repository

I created manually the README.md file in the local folder

Initialize git: create a new repository with a .git file hidden (won't be committed)
git init

Check files in the new path
dir

Global config - first time git setup
Search in Google "Git global config"

git config --global user.name "Santiago Muñoz"
git config --global user.email "munozgonzalezsantiago@gmail.com"

Understand status of changes
git status

Make git to track a file
git add README.md

Check that file is now being tracked. Will be added to "Changes to be committed"
git status

Commit -> staging environment before pushing
git commit -m "First commit"

Check that commit has been in place, so "nothing to commit"
git status

Know the current branch
git branch

Rename a branch 
git branch -m new_name

Check
git branch

Connect local repository (local .git file) to remote repository
git remote add origin <link.git>

Understand where is the origin
git remote -v

Push to remote repo
git push origin main