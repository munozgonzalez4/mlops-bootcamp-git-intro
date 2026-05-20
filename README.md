# mlops-bootcamp-git

A quick Git reference for the bootcamp exercises, with common commands and workflow notes.

## 1. Verify Git Installation

In Command Prompt:

- Check the installed Git version:
  ```bash
  git --version
  ```

## 2. Initialize a Local Repository

After creating a local project folder and adding files (for example, `README.md`):

- Initialize Git in the folder:
  ```bash
  git init
  ```

- List the contents of the folder:
  ```bash
  dir
  ```

## 3. First-Time Configuration

Set your global Git identity once on a new machine:

```bash
git config --global user.name "Santiago Muñoz"
git config --global user.email "munozgonzalezsantiago@gmail.com"
```

> If you need help, search for "Git global config".

## 4. Basic Workflow: Add, Commit, Push

- Check current repository state:
  ```bash
  git status
  ```

- Stage a file to commit:
  ```bash
  git add README.md
  ```

- Verify the staged file:
  ```bash
  git status
  ```

- Create the first commit:
  ```bash
  git commit -m "First commit"
  ```

- Confirm that the commit succeeded:
  ```bash
  git status
  ```

## 5. Branching Basics

- Show the current branch:
  ```bash
  git branch
  ```

- Rename the current branch:
  ```bash
  git branch -m new_name
  ```

- Confirm the branch name change:
  ```bash
  git branch
  ```

## 6. Connecting to a Remote Repository

- Add a remote named `origin`:
  ```bash
  git remote add origin <link.git>
  ```

- Confirm the remote URL:
  ```bash
  git remote -v
  ```

- Push the local branch to the remote:
  ```bash
  git push origin main
  ```

## 7. Making Changes and Revising Files

- See modified files:
  ```bash
  git status
  ```

- Stage a file after editing:
  ```bash
  git add README.md
  ```

- Stage all changed files:
  ```bash
  git add .
  ```

- Unstage a file:
  ```bash
  git restore --staged <file>
  ```

- Discard local changes in a file:
  ```bash
  git restore README.md
  ```

## 8. Undoing Commits

- Reset the current branch to the previous state:
  ```bash
  git reset
  ```

## 9. Viewing Differences

- Compare working changes that are not staged:
  ```bash
  git diff
  ```

- Compare staged changes that are ready to be committed:
  ```bash
  git diff --staged
  ```

## 10. Cloning a Repository

- Change into the target parent folder:
  ```bash
  cd folder_we_want_to_clone
  ```

- Clone the remote repository:
  ```bash
  git clone <link>
  ```

## 11. Branch Workflow

- Create a new branch:
  ```bash
  git branch <branch-name>
  ```

- Switch to that branch:
  ```bash
  git checkout <branch-name>
  ```

- Merge the branch into `main`:
  ```bash
  git checkout main
  git merge <branch-name>
  ```

- Push the updated `main` branch to remote:
  ```bash
  git push origin main
  ```

## 12. Viewing Commit History

- Show all commits:
  ```bash
  git log
  ```

- Show the last `n` commits with patch details:
  ```bash
  git log -p -<n>
  ```

## 13. Git Cheat Sheet

- Show the current branch:
  ```bash
  git branch
  ```

- Create and switch to a new branch:
  ```bash
  git checkout -b <branch-name>
  ```

- Stage all changed files:
  ```bash
  git add .
  ```

- Remove a file from staging:
  ```bash
  git restore --staged <file>
  ```

- Discard local edits in a file:
  ```bash
  git restore <file>
  ```

- Revert the last commit but keep changes locally:
  ```bash
  git reset --soft HEAD~1
  ```

- Show file status quickly:
  ```bash
  git status
  ```

- Fetch remote changes without merging:
  ```bash
  git fetch
  ```

- Pull remote changes into the current branch:
  ```bash
  git pull
  ```

- Push the current branch to the remote repository:
  ```bash
  git push origin <branch-name>
  ```
