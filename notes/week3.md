% Week 3
% Configuration & Branching
% Feb 12 2015

# Configuration

## Scope

- System
    - /etc/gitconfig
	  - not mutable
- Global
	  - ~/.gitconfig
    - git config --global <parameter> <value>
- Project
    - .git/config
    - git config <parameter> <value>
 
## File format

```
# My comment
[section]
	parameter = value
 
# Example section for user parameters
[user]
	name = Ben Campbell
	email = me@benjica.com
```

## User Options
 
- email
    - Used when creating commits in conjunction with name
    - git config user.email me@benjica.com
- name
    - Used in commits to identify commit author
    - git config user.name Benjamin Campbell

## Core Options
 
- editor
		- Defines what editor to use for commits
		- git config core.editor vim

. . .

Windows has no tride and true mechanism for this parameter. 

## Example

- man git config
- git config <parameter> <value>
 
# Branching

## 

![Commit Anatomy][1]

##

![Linear History][2]

## Where does the branch fit in?

. . .

A branch is simply a pointer to any commit.

##

![Two Branches Added][3]

## HEAD

- A special pointer to the current state of the repo
- Apparent everywhere committing, merging, etc...
- Command: 
    - git checkout <COMMIT HASH | branch_name >
    - Moves HEAD to point to given value
 
## Branch Commands

- git branch <branch_name>
    - Usese the current HEAD to create new branch
    - can pass a second param to hash different then HEAD
- git branch -d <branch_name>
   - _Safely_ removes a branch

## Branch Commands
- git branch -m <old_branch> <new_branch>
    - Renames a branch

[1]: images/commit.png
[2]: images/commits-and-parents.png
[3]: images/two-branches.png
