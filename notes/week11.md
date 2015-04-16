% Week 10
% Collaboration Strategies 
% April 16 2015

# Models

## Centralized Repository

* A Blessed Repository
* Staggered permissions of access
* Tiered access based on number of contributors

----------------------------------

![Centralized Repository][1]

----------------------------------

![Integration Manager][2]

----------------------------------

![Benevolent Dictator][3]

## Asynchronous Repositories

* Fork Model
* Copy of Blessed Repository
* Acts as a public point demarcation

----------------------------------

![Fork a Repo][4]

## Asynchronous Repositories

* Allows contributors to boot strap without intervention
* Github allows PR's to be created across forks
* Acceptance of outside contribution can be out of band

# Pull Request Model

## Overview

* Staggered integration of commits
* Logically separates functionality/fixes
* Promotes Code Review

# Example

## This slide is purposeful 

yeah!

## Feature Branch

* Create new branch from the main(**master**) branch
* I plan to remove the slide mentioned previously
* The branch now has a small set of commits that achieves my goal

## Push to Github

* `git push --set-upstream origin remove_slide`
* Sends commits to Github and branch pointer

## Create Pull Request

* Github highlights the new branch
* Allows me to create a new pull request
* I must choose my compare branches
* And write a good summary

## Review and Merge

* Github offers tools to annotate the changes
* Once consensus is reached (:+1:, LGTM)
* Merge and close

## Pull upstream

* The change has been merge into the main branch
* `git pull origin master`
* The main branch is updated and ready for the next feature branch

[1]: images/central_repository.png
[2]: images/integration-manager.png
[3]: images/benevolent-dictator.png
[4]: images/fork-a-repo.gif
