% Week 8
% Remotes
% March 11 2015

# Remotes Abstraction

## What is a remote?

* A remote is a *noun* of a synchronization verb
* A complete repository located elsewhere

## Where can a remote be?

* Git is a file system based version control
* Synchronization occurs by passing files 
* We can use a *file based* protocol to transfer between remotes
* This can be a file path or a remote URI

# Protocols

## File

* git can use a simple file path to synchronize
* Pros
    * Simple setup
    * Uses existing resources
* Cons
    * Not very public
    * Can be slow on network filesystems

## SSH

* A common communication protocol
* Pros
    * Relatively fast
    * Authenticated
    * Ubiquitous 
* Cons
    * Authentication
    * No anonymous 

## HTTPS

* Two flavors, smart and dumb
* Pros
    * Ubiquitous
    * Anonymous
* Cons
    * Difficult to setup server
    * Authentication can be difficult

# Remote Management

## `git remote`

* Dense subcommands
* Addition/removal/rename of a given remote
* Maintenance Commands set-url, set-branches, prune
* `git remote show <name>`

## Adding Remote
* `git remote add <name> <URI>`
* Flags
    * `-t <branch_name>` Specify a branch to track
    * `-f` Fetch after adding
* You can have many remotes

## Removing/Renaming Remotes
* `git remote <remove | rename> <name>`
* Deletes the remote definition
* This removes local tracking branches

## Mutating Remotes
* `git remote set-branches <name> <branches>` Updates list of branches to track
    * Varadiac - you can have many branches
* `git remtoe set-url` Updates url/changes protocol

## Cleanup Remotes
* `git remote prune` Compares remote branch list and removes extra
* `git remote update` Updates list of available branches

# Remote Synchronization 

## Fetch

* Brings changes into local repository
* Updates local tracking branch
    * origin/master vs master
    * Does not update local branches

## I thought this was a pull

* A pull is an aggregate command
    * `git pull origin master` is two commands
    * `git fetch origin master`
    * `git merge origin/master`
* This can be hairy

## Push
* Takes remote and refspec as parameters
* **MUST BE FAST FORWARD FOR RECEIVER**
    * Your common ancestor is behind remote
    * You must fetch/pull and make HEAD of remote a common ancestor

# Questions?

## Future

* Next week will talk about
    * Remote branch definitions
    * More terminal examples
    * SSH Keys
