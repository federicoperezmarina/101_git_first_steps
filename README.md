# 101_git_first_steps
This is a repository to learn how use git (control version)

## Table of Contents
* [Git installation](#Git-installation)
* [Git configuration](#Git-configuration)
* [Git starting a project](#Git-starting-a-project)
* [Git day to day work](#Git-day-to-day-work)
* [Git branching model](#Git-branching-model)
* [Git review your work](#Git-review-your-work)
* [Git tagging commits](#Git-tagging-commits)
* [Git reverting changes](#Git-reverting-changes)
* [Git synchronizing respositories](#Git-synchronizing-repositories)
* [.gitignore](#gitignore)


## Git installation
Git is a free and open source distributed version control system designed to handle everything from small to very large projects with speed and efficiency.

Git is easy to learn and has a tiny footprint with lightning fast performance. It outclasses SCM tools like Subversion, CVS, Perforce, and ClearCase with features like cheap local branching, convenient staging areas, and multiple workflows.

You can download and install from this [site](https://git-scm.com/downloads)


## Git configuration
```sh
git config --global user.name “Your Name”
```
Set the name that will be attached to your commits and tags.

```sh
git config --global user.email “you@example.com”
```
Set the e-mail address that will be attached to your commits and tags.

```sh
git config --global color.ui auto
```
Enable some colorization of Git output.


## Git starting a project
```sh
git init [project name]
```
Create a new local repository. If [project name] is provided, Git will
create a new directory name [project name] and will initialize a
repository inside it. If [project name] is not provided, then a new
repository is initialized in the current directory.

```sh
git clone [project url]
```
Downloads a project with the entire history from the remote repository


## Git day to day work
```sh
git status
```
Displays the status of your working directory. Options include new,
staged, and modified files. It will retrieve branch name, current commit
identifier, and changes pending commit.

```sh
git add .
git add [file]
```
Add a file to the staging area. Use in place of the full file path to add all
changed files from the current directory down into the directory tree.

```sh
git diff [file]
```
Show changes between working directory and staging area.

```sh
git diff --staged [file]
```
Shows any changes between the staging area and the repository.

```sh
git checkout -- [file]
```
Discard changes in working directory. This operation is unrecoverable.

```sh
git reset [file]
```
Revert your repository to a previous known working state.

```sh
git commit -m"descriptive message"
```
Create a new commit from changes added to the staging area.
The commit must have a message!

```sh
git rm [file]
```
Remove file from working directory and staging area.

```sh
git stash
```
Put current changes in your working directory into stash for later use. 

```sh
git stash pop
```
Apply stored stash content into working directory, and clear stash.

```sh 
git stash drop
```
Delete a specific stash from all your previous stashes. 

## Git branching model


## Git review your work


## Git tagging commits


## Git reverting changes


## Git synchronizing respositories


## .gitignore

