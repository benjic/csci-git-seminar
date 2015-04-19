% Week 12
% Rewriting History
% April 16 2015

# Danger Will Robinson

## Established Lineage

Commits are hashed including their parent commits. If I change the content of a
commit I get a new hash.

...

And so do all of its children

## Propagation

Changing history is trivial.

...

It's letting the future know that is difficult.

## Rules of Thumb

* Only change public branches in communique with the public
* Otherwise, go nuts

# Undo with Amend & Reset

## Amending a commit

Sometimes the last commit is tarnished

* Bad commit message
* Added unrelated file
* Left a file out
* Forgot to ...

## Staging

* `git add file.ext`
* `git co HEAD~1 file.ext`
* `git rm file.ext`
* etc

## Amend

`git commit --amend ...`

## Reset

You may want to *throw away* commits

## Reset

Moves HEAD and branch pointers to given commit with varying degrees

> * `git reset --soft <commit>`
> * `git reset --mixed <commit>`
> * `git reset --hard <commit>`

## Different then checkout

A *checkout* moves HEAD while a *reset* moves all pointers

# Rebase

## What is a rebase
Given a *range* of commits; Replay them with a different ancestor

## Branches

Lets say I am on my feature branch and it is now outdated

* `git rebase master`
* `git rebase master myfeature`

## Upstream

This is useful in conjunction with `git fetch`

* `git rebase origin/master master`

## Upstream

![Upstream][1]

## Interactive

Rebase offers an interactive rewriting

...

`git rebase -i <commit>`

## Example

To the example!

# Questions?

[1]: images/upstream.png
