% Week 13 and 14
% Odd's and Ends
% April 30 2015

# Reflog

## HEAD

Everytime git updates the HEAD pointer a reflog entry is created.

* Previous SHA hash
* Current SHA hash
* Time & Operation

## What is this good for?

Commits are rarely removed so reflog allows you to undo commands.

## Commands

* `git reflog`
* `git co HEAD@{23}`
* `git reset HEAD@{23}`

## Example

Lets make a bad change and undo.

# Stashing

## WIP

Wouldn't it be nice if we had a place to put stray commits?

You can with the stash!

## The Stash Stack

You can push a temporary commit and pop previous stash commits

* `git stash`
* `git stash save "my message"`
* `git stash list`
* `git stash apply`

## Example

# Hooks

##

![Hooks][1]

## Embarrassment
Often we have tests for our code. You pushed a commit that fails.

## Automation
Why didn't you just run your tests before pushing? You forgot!

## Introducing Hooks
git allows you to run scripts and key points of the git process

* pre-push
* pre-commit

## Example

Go Tests

# Cherry Picking
## Selective commits

Cherry picking is selective rebasing

Given a commit or range it applies the commit to current branch

## Why?

* We can construct collective fixes/features
* Backport feature/fixes to previous releases

## 

![Git Flow][2]

## Commands

`git cherry-pick 123abd90f`
`git cherry-pick ..master`


# The End

## 

Thanks!

[1]: images/hooks.jpg
[2]: images/git-flow.svg
