## Git Hidden Folder

There is a hidden folder called `.git` which tells you that our 
project is a git repo.


If we wanted to create a git repo in a new projecct we' create the
folder and the initalize that repo using `git init`

```
mkdir /workspaces/tmp/new-project
cd /workspaces/tmp/new-project
git init
touch Readme.md
code Readme.md
git status
git add Readme.md
#make changes to readme.md
git commit -a -m "add readme file"


```



## Cloning
We can clone three ways: HTTPS, SSH, Github CLI

Since we are using GitHub Codespaecs we'll create a
temporary directory in our worksplace.

```sh
mkdir /workspace/tmp
cd /workspace/tmp
```


### HTTPS
```sh
git clone https://github.com/joebloggsnln/Github-Examples.git
cd Github-Example
```

## Commits

When we want to commit code we can write git commit which will
open up the commit edit message in the editor of choice.

```sh
git commit
```

Set the globel editor 
```
git config --global core.edito emacs
```

Make a commit and commit message without opening an editor
```sh
git commit -m "add anther exclamation mark"
``` 

## Branches

## Remotes

## Stashing

## Merging


## Add

When we want to stage changes that will be included in the commit
we can use the . to add all possible files.

```
git add Readme.md 
git add .
```

## Reset

Reset allows you to move Staged changes to be unstraged.
 This is useful when you to revert all files not to be 
 not commited

 ```
 git add .
 git reset
 ``` 
> git reset will revet a git add.

## Status 

Git status shows you what files will or will not be commited.

```
git status  
```

## Gitconfig file

The gitconfig file is what stores your global configurations
for git such as enmail, name, editor and more.

Showing the contnets of our .gitconfig file
```
git  config--list
```

when you first install Git on a machine you are suppose to set up
your name and email

```sh
git config --global user.name "John Doe"
git conjfig --global user.email johndoe@examples.com
```
## Log
git log will show recent git commits to the  git tree

```sh
git log 
```


## Push 
When we want to push a repo to our remote origin

```sh
git push
```

