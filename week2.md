% Structure
% Version Control with Git
% January 29, 2015

# Heads up

## Core Commands

- Fundemental Commands
- Illustrate abstraction
- Peek under the covers

# The Repository

## Where is it?
> - .git/
> - What's in there?
> - Concepts of storage?

## git init

> - *Lets try it out*
> - man git init
	>	- Our first sub command!
> - git init

# The Stage

----

![Demarcation](images/areas.png)

----

## git status

> - Describes the stage
> - Files that changed
> - Files we don't know?

## Lets try it!
> - man git status
> - git status

## git add

> - adds file to stage
> - wide degree of granularity

## Lets try it!
> - man git add
> - git add
> - git add -p

## git commit

> - Captures the stage
> - Binds the state to the commit log

## Lets try it!
> - man git add
> - git add
> - git add -p

## Reversing Direction

> - git checkout -- <file>
	> - replaces working directory with last commit
	> - undoes what you did
> - git reset HEAD <file>
	> - unstages file

# The log

## git log

> - Each commit adds information
> - *Provides Context*
> - As well as persistent information

## Lets try it

> - man git log
> - git log
	> - Pager?
> - git log --graph
> - git log --patch
> - git log --author

# Finale

## QA
- Anything to share?
- Anything to ask?
