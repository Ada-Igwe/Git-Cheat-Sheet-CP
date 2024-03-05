![Git_image](/Git_image.png)

git # Git and Github basics
Taking you from the very basics of Git, version control, and Github to the common processes you will use.

## Table of Contents
- [What is Git](#what-is-git)
- [What does Git do](#what-does-git-do)
- [Getting Started with Git](#getting-started)


### What is Git?
- Git is a free and open source version control system
- Git is used to:
  - Track code changes
  - Track who made changes
  - Collaborate during coding

### What does Git do
- Manage projects with **Respoitories**  
- **Clone** a project to work on a local copy
- Control and track changes with **Staging** and **Committing**
- Branch and merge to allow for work on different parts and versionas of a project.
- Pull the latest version of a project to a local copy.
- Push local updates to the main project.

### Getting Started
1. ##### Download Git from [Git-scm](htttps://git-scm.com)
2. ##### Using Git on the Command line
   - Open your terminal
   - Windows can sue GitBash, installed with Git

3. ##### Check your version of Git on your machine

```bash
git --version
# or
git -v
```
4. ##### Let git know who you are
- Create an account on [Github](https://github.com)
- In terminal, configure your name and email so Git knows who is making the changes.
- Use global to set the username and email for every repository on your computer.
- If you want to set the username/email for just the current repo, you can remove ```--global```

```bash
git config --global user.name "Jane Doe"
get config --global user.email "Jane@example.com"
```

5. ##### Create a project to work in
- If you already have a folder that you use, then  navigate to it using the terminal.

```bash
#make a new directory
mkdir your_folder_name
#change to the current working directory
cd your_folder_name
```
6. ##### Initialize Git 

```bash
git innit
```
- Git knows that it should watch the folder that you initiated it on.
- Git creates a hidden folder to keep track of the changes

```
# how to show the folder in vs code
Code|File --> Preferences --> settings
Search for "exclude" to find the default exclude list
Edit ".git extension to remove it from the list and allow it to be visible in VS code. 
```
7. ##### Open the text editor and add some files
There is  shortcut to open your current working directory in vs code. Mac users may have to look up how to configure this.

```bash
code .
```
8. ##### Let's work with files
```bash
#create a new file
touch index.html
```
9. ##### Check the status of the repo
```bash
git status

#check with the compact output

git status--short

#the short status flas are:
# ?? - Untrcked
# A - Files are added to stage
# M - Modified
# D - Deleted Files
``` 
- After initialization,Git is aware of the file but not added to the repo
Untracked are not added to the repo yet. Git add changes the status of the files to tracked and are now in the staging environment.

10. ##### Staging our files
```bash
#add our file to the staging environment

git add index.html

#or add multiple files at once
git add --all


  #or 

 git add .
 ``` 