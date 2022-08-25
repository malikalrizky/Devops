# Day 4

# Version Control System

A version control system is a kind of software that helps the developer team to efficiently communicate and manage(track) all the changes that have been made to the source code along with the information like who made and what changes have been made.

# git

git is one of version control system that created by Linus Torvalds, which have top feature called distributed revision control is git storage not only in one storage. But everyone involved in the project will get the git database, which make it easier to manage both offline and online.

![](./media/git.jpg)

# Versioning using git

1. Setup git environment on Ubuntu

Install git
`sudo apt install git`

![](./media/1.png)

![](./media/2.png)

Config username, email, and SSH key

![](./media/3.png)

Make private/public key
`ssh-keygen`

![](./media/4.png)

Open generated file
`cat ./.ssh/id_rsa.pub`

![](./media/5.png)

Go to profile settings

![](./media/6.png)

Choose SSH and GPG keys and enter the generated key

![](./media/7.png)

Test connection to Github

![](./media/8.png)

2. Making repository Github

`git init`

The git init command is used to initialize a new git repository or reinitialize an existing one. The git init command transforms the current directory into a Git repository.It will also create a new master branch.

![](./media/10.png)

### Git Ignore

.gitignore file is a text file that tells Git which files or folders to ignore in a project.

![](./media/11.png)

Adding file for committing

![](./media/12.png)

Creating repository

![](./media/13.png)

![](./media/14.png)

Copy SSH

![](./media/15.png)

Commit into local repository

![](./media/16.png)

![](./media/17.png)

Push to sent file on local repository into github repository

![](./media/18.png)

![](./media/19.png)

Create branch

Branching offers a way to work on a new feature without affecting the main codebase. This feature is very important to DevOps.

![](./media/20.png)

![](./media/21.png)
