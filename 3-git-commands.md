
# Git commands to be successful in life

## .gitignore

## Getting started with a repo link

The following assumes you have Git and VS Code installed.

1. From your CLI, CD in to your repos directory.
2. Run `it clone https://github.com/nocticdr/github-basics`
   Note: If you are given a DevOps link, you might be required to authenticate.
   Also: When you do `git clone`, the directory is automatically initialised as a git directory. No need to run `git init`.
3. Add the new repo to the VS Code workspace on the left hand side.
4. CD in to the new repo and modify the content of the file README.md as you wish.
5. Run `git add readme.md` to tell Git to add the specific file to a staging area. (Use `git add .` if you want to add all files in the directory)
6. Tell git WHERE to save the file remotely (remote repo) `git push --set-upstream origin master`.
7. Tell git to save the file remotely (remote repo) `git push`.

## Quick steps for creating README.md file in a your own new repository

1. Create a local repository and initialise it using `git init`
2. Create a remote repository and clone it to move it to local and initialised at the same time.
3. Create a readme file, put some content in and save it.
4. Add it to the staging area with `git add filename` or `git add .`.
5. Save the file locally (local repo) and put a description with `git commit -m "I made some changes to the file"`.
6. Tell git WHERE to save the file remotely (remote repo) `git push --set-upstream origin master`.
7. Tell git to save the file remotely (remote repo) `git push`.

| Command | Description |
| ------- | ----------- |
| `git config --global --unset ked.mardemootoo@gmail.com` | unset email ID |
| `git config --global user.name nocticdr` | Set user name |
| `git config --global user.email ked.mardemootoo@gmail.com` | Set user email address |
| `git config --list` | Check user account configured |
| `git commit --amend --reset-author` | Reset registered author |
| `q` | Quit VIM |

### Making, saving and committing changes
| Command | Description |
| ------- | ----------- |
| `git add .` | Add a file to the staging area |
| `git commit -m "text"` | Commit changes with remark text |
| `git push` | Push changes to remote repository |





Step 1
### Getting & Creating Projects

| Command | Description |
| ------- | ----------- |
| `git init` | Initialize a local Git repository |
| `git clone https://github.com/[username]/[repository-name].git` | Create a local copy of a remote repository |

Step 2
### Basic Commands

| Command | Description |
| ------- | ----------- |
| `code filename.tf` | Create a new terraform file called filename with extension tf |
| `git status` | Check status |
| `git add [file-name.txt]` | Add a file to the staging area |
| `git add -A` | Add all new and changed files to the staging area |
| `git commit -m "[commit message]"` | Commit changes |
| `git rm -r [file-name.txt]` | Remove a file |
| `rm -rf [foldername]` | Remove a folder |
| `rm -rf .git` | Remove a git init |

### Branching & Merging

| Command | Description |
| ------- | ----------- |
| `git branch` | List branches (the asterisk denotes the current branch) |
| `git branch -a` | List all branches (local and remote) |
| `git branch [branch name]` | Create a new branch |
| `git branch -d [branch name]` | Delete a branch |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git checkout -b [branch name]` | Create a new branch and switch to it |
| `git checkout -b [branch name] origin/[branch name]` | Clone a remote branch and switch to it |
| `git checkout [branch name]` | Switch to a branch |
| `git checkout -` | Switch to the branch last checked out |
| `git checkout -- [file-name.txt]` | Discard changes to a file |
| `git merge [branch name]` | Merge a branch into the active branch |
| `git merge [source branch] [target branch]` | Merge a branch into a target branch |
| `git stash` | Stash changes in a dirty working directory |
| `git stash clear` | Remove all stashed entries |
| `git rebase master` | From within branch, it will rebuild branch with latest master code |

### Sharing & Updating Projects

| Command | Description |
| ------- | ----------- |
| `git push origin [branch name]` | Push a branch to your remote repository |
| `git push -u origin [branch name]` | Push changes to remote repository (and remember the branch) |
| `git push` | Push changes to remote repository (remembered branch) |
| `git push origin --delete [branch name]` | Delete a remote branch |
| `git pull` | Update local repository to the newest commit |
| `git pull origin [branch name]` | Pull changes from remote repository |
| `git remote add origin https://github.com/[username]/[repository-name].git` | Add a remote repository |
| `git remote set-url origin https://github.com/[username]/[repository-name].git` | Set a repository's origin branch to SSH |
| `git push --set-upstream origin master ` | Set the upstream branch for master. Create repository on GitHub first. |

### Inspection & Comparison

| Command | Description |
| ------- | ----------- |
| `git log` | View changes |
| `git log --summary` | View changes (detailed) |
| `git diff [source branch] [target branch]` | Preview changes before merging |
| `git remote -v` | View origin fetch and push URLs |
| `git remote rm origin` | Remote origin in case of "fatal: remote origin already exists." |
| `git remote show origin` | View local and remote status |

rsync
type nul > secret.tfvars
notepad secret.tfvars

CTRL+K+U - quick comment/uncomment in CODE
Shift+Option+A - Block Comment
Control+/ - Line comment

