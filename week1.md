% Week 1
% Version Control with Git
% January 29, 2015

# Administrative

## Syllabus
- 1 Credit for Attendance
- No Required Text*
- Academic Dishonesty
- DSS Accommodation
 
## People
-  I am Ben.
	- Junior
	- [5 years w/ Git][github_benjic_user]
	- Daily user
- Rob Smith
	- Seminar Mentor
	- Greivences
 
## Seminar Goals
-  Mine
	- Share knowledge
	- Encourage peer support
	- Have fun
- Yours?
	- ...
	- ...

## Git Goals

- Conceptualize how commits are generated and collected
- Communicated ideas and problems related to Git
- Make effective use of non linear history
- Stratigize for distributed team interaction
- Annotation and metadata of versioning
- Tooling and platform integration

## Plan
- Only use the git command
- Encourage daily use
- Offer QA every week

## Tools & Resources
- [Pro Git][pro_git]
- `man git`
- Github 
- [asciienma][asciienma]

-------------------------------------------------------------------------

<script type="text/javascript" src="https://asciinema.org/a/15400.js"
id="asciicast-15400" async></script>
  
# Version Control?

## 
![Order][filing]

## 
![Diffs][diff_image]

##
![Snapshots][snapshots_image]

## File Versioning

- nested directories
- versioned zips
- Why is this difficult?
	- Hard to _order_
	- Hard to _diff_
	- Hard to _revert_
- Why is it good?

##
![Central Server][central_server]

## Central Server
- CVS, Subversion
- Why is this good?
	- Ordered
	- Authoritative
- Why is it *BAD*?
	- Centralized dependency
	- Hard to synchronize
	- Deltas

## 
![Distributed][distributive_image]

## Distributed 
- Git, Mecurial
- Every actor has a copy of entire repo
- Why is this good?
	- Redundant Copy
	- Local Operations
	- Independent Operations

# Git Installation

## Distribution

- Git is readily available
	- Linux
		- Package Management
		- Compile from source
	- Max OS X
		- homebrew/macports
		- native w/ mavricks+
		- Binary Installer
	- Windows
		- Binary Installer

## Installation Sanity

- `git version`
- `git help`

## Lets get you setup!

[github_benjic_user]: https://api.github.com/users/benjic
[pro_git]: http://git-scm.com/book/en/v2
[asciienma]: https://asciinema.org/
[messy_papers]: images/messy_papers.jpg
[filing]: images/filing.jpg
[central_server]: images/central_server.png
[diff_image]: images/deltas.png
[snapshots_image]: images/snapshots.png
[distributive_image]: images/distributed.png
