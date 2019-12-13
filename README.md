![Git](Git-icon-black.svg.png)

# git-tutorial

__Version Control Automatic way to track changes__

## Why use Git

* develop speculative features without disrupting development - branching
* collaborate easily and conviniently
* view previous versions
* securely backup project and history

### Popular Git PLatforms

![Github](github-icon.jpg=250x250)

<img src="github-icon.jpg" width="250" height="250">
![Gitlab](GitLab_Logo.svg.png)

## Commands you need to know

* installing git
* git config
* git init
* git add 
* git commit -m"..."
* git stash
* git branch
* git push/pull
* git clone
* git checkout
* git merge
* git reset
* git remote

## git sequence

![Git Sequence](git_status_sequence.png)

### Installing Git & Setup

__Install (Linux):__

`sudo apt-get install git`
Check if installation was successful: 
`git --version`

__Configure:__ 

`git config --global user.name "Your Name"`
`git config --global user.email your.email@example.com`


__SSH Keys__

__Create pair:__

`ssh-keygen -t rsa -b 4096 -C "email@example.com"`
`cat ~/.ssh/id_rsa.pub`

Copy and paste into "SSH Keys" Section in your account settings

__Check Success:__ 
`ssh -T git@gitlab.com` 

(Works with Gitlab)
$ ssh -T git@github.com

Hi lut! You've successfully authenticated, but GitHub does not provide shell access.

__Github fix:__

`git remote set-url origin git@github.com:lut/EvolutionApp.git`


__Commence Version Control__


`git init`
`git add .`
`git commit -m"..."`
`git remote add origin`
`git push -u origin master`

__Level up (Branch management)__

Create and switch to new branch: 
`git checkout -b branchname`
`git log`(view records of commits)
`git reflog:` record when branch tips are updated
`git status`
`git branch`
`git checkout branchname`(if exists)

__Start Flexin (run the commands people are afraid of)__

`git stash`: save changes you do not want to commit already
`git merge`: merge two branches you were working on 
`git reset`: sets index to latest commit that you want to work with
`git remote`: check source



