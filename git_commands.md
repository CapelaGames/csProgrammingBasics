# Git, CMD and Bash Cheat Sheet


## CMD Only 
Windows commands

| Command			| Action			| Example			|
|-------------------|-------------------|-------------------|
| dir				|	Displays files in the current folder | `dir`|
| ..\\..			|	Substitute for Parent of Parent folder |	`ls ..\..` OR `dir ..\..` |		

## BASH Only 
Unix-like commands

| Command			| Action			| Example			|
|-------------------|-------------------|-------------------|
| ls				|	Displays files in the current folder | `ls`|
| ..\/..			|	Substitute for Parent of Parent folder |	`ls ../..` OR `dir ../..` |		

## General Commands
Works in both CMD and BASH

| Command			| Action			| Example			|
|-------------------|-------------------|-------------------|
| cd \<directory>	|	Change the folder you are navigating |	`cd ./Documents/GitHub` |
| mkdir	\<directory>|	Creates a folder	| `mkdir newFolderName` |
| .					|	Substitute for Current folder 	| `ls .` OR `dir .` |
| ..				|	Substitute for Parent folder	| `ls ..` OR `dir ..` |

## GIT Commands 
Works in both CMD and BASH


| Command			| Action			| Example			|
|-------------------|-------------------|-------------------|
| clone				| Copy remote repo	| git clone https://github.com/EpicGames/UnrealEngine			|
| init				| Create a repo		| `git init` |
| status			| Current status that git is in, used to check what branch you are in and if there is anything to commit| `git status` OR `git status -vv` |
| fetch				| Refresh, check if there is any changes | `git fetch`
| pull				| Download any changes					| `git pull`
| add				| Stage files, which is adding changed files ready to be commited	| `git add .` <br> (Note, `.` here means add all files, it acts like a wild card |
| commit			| Confirm the changes locally | `git commit -m "Write what changed here" `
| push				| Upload changes that have been commited | `git push`

## Branching

### Branching commands
| Command			| Action			| Example			|
|-------------------|-------------------|-------------------|
| branch			| used for checking your branchs as well as creating a new branch | `git branch` <br> OR `git branch -a` <br> OR `git branch new_branch_name`
| log				| used to display changes commited | `git log` |


### How to branch

Steps on making a branch and switching to it

```
git branch
```
* Displays branches that exists locally
* The star tells you what branch you are in
```
git branch -a
```
* You can add -a if you want to see remote branches too
```
git branch name_of_branch
```
* Copys your current branch and makes a new branch with the name provided
```
git checkout name_of_branch
```
* Switch to another branch
```
git push --set-upstream origin name_of_branch
```
* Uploads the branch to github



### How to merge

Steps on merging two branches

```
git checkout name_of_branch
```
* Switch to the branch you want to merge into

```
git merge other_branch
```
* other_branch will merge into the current branch
```
git push
```
* Don't forget to push

## Extras

### Make a file in bash
To make a file, use touch plus the name of the file you want to make (it will be empty)
```
touch nameOfFile.md
```

### Change default branch's name
If you want to change your default branch name
```
git config --global init.defaultBranch main
```

### Create a pretty log graph
If you want to have a pretty `git log` with a graph you can use `git log --all --decorate --oneline --graph`
Just remember A DOG
> "A Dog" = git log --**a**ll --**d**ecorate --**o**neline --**g**raph

<br>Or run this command:
```
git config --global alias.adog "log --all --decorate --oneline --graph"
```
then you can use:
```
git adog
```
![adog](./Screenshots/adog.jpg)

### Help I'm stuck in vim
type `esc :q!`



