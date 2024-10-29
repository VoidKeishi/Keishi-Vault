## Sources
- [Gitbook](https://git-scm.com/book/en/v2)  
- [Introduction to Git and Github Google Course](https://www.coursera.org/learn/introduction-git-github)
## Basic Concepts
### What is Version Control
- Version Control is a system that records changes to a file or set of files over time so that you can recall specific versions later.
### What is Git
- Git is a Distributed Version Control System (DVCS) that stores data in a file system made up of snapshots.
### What is GitHub
- GitHub is a code hosting platform for version control and collaboration. It lets you and others work together on projects from anywhere.
## Git Basic
### How to install Git
- Download Git from [Git](https://git-scm.com/downloads) and install it.
### How to configure Git
- git config --global user.name "Your Name"
- git config --global user.email "
### How to create a repository
- git init
### How to add files to the staging area
```shell
git add <file_name>
```
### How to commit changes
```shell
git commit -m "Commit message"
```
### How to check the status of the working tree
```shell
git status
```
### How to check the differences between the working tree and the staging area
```bash
git diff
```
### How to check the differences between the staging area and the repository
```bash
git diff --staged
```
### How to check the differences between the working tree and the repository
```bash
git diff HEAD
```
### How to check the differences between two commits
```bash
git diff <commit_id_1> <commit_id_2>
```
### Show graph of commits
```bash
git log --graph --oneline
```
### Git rebase
```bash
git pull --rebase
```
- If get conflict
```bash
git rebase --abort
```
## Github
### How to synchronize local folder with remote repository on GitHub
First create repository on GitHub
If start from GitHub:
- Clone from repository on GitHub:
        git clone <https://github.com/username/remote-repository.git>
- Add origin to repository on GitHub:

  

        git remote add origin <https://github.com/username/remote-repository.git>

- Pull changes from remote repository if there are changes:

  

        git pull origin <branch_name>

- Push changes from local folder to remote repository if there are changes:

  

        git push origin <branch_name>

  

If start from local folder:

  

    - git remote add origin <https://github.com/username/remote-repository.git>

    - git push -u origin master

  

### How to restore a version of a file from a previous commit on github

  

    - git reset --hard <commit_id>

    - git push --force origin <branch_name>

  

### Three ways merge

  

Fetch from remote first:

  

    - git fetch origin

Make the history linear:

  

    - git checkout <branch_local>

    - git rebase <branch_remote>

  

Fast foward merge:

  

    - git checkout <branch_name>

    - git merge <branch_name>

  

Delete old branch:

  

    - git branch -d <branch_name>

    - git push origin --delete <branch_name>

  

### Delete a branch
Locally:  
    - git branch -d <branch_name>
Remotely:

  

    - git push origin --delete <branch_name>

  

### Collaborating

  

#### How to fork a repository

  

Forking is a way to make a copy of a given repository so that it belongs to our user.

  

Workflow : Fork on a repository -> Clone on local machine -> Make changes -> Push to forked repository -> Pull request to original repository