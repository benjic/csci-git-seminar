% Week 4
% Branching & Merging
% Feb 19 2015

# Branching

## Review

Branch commands

> * `git branch <name>      // Create new branch <name>`
> * `git checkout <name>    // Change HEAD to point to <name>`
> * `git checkout -b <name> // Combination of previous two`

##

![A simple branch][1]

## Lets Try

# Merging


## Merge

* `git co <into_branch>`
* `git merge <merge_branch>`
* `man git-merge`

## Merge

* Now we want to combine two divergent histories
* It is a comparison of three commits
    
...

> * HEAD
> * A common ancestor
> * Merging Branch



## Fast Forward

* The _easiest_ merge
* HEAD *is* common ancestor
* Diff between HEAD and branch is effectively branch
* Update current branch to point to merge branch

## Lets Try to Fast forward


## 

![Divergent History][2]

## Example

Lets build a divergent history

## Divergent History

* HEAD is different then common ancestor
* Two diffs; HEAD..commonAncestor, branch..commonAncestor
* No overlapping change; The change set is disjoint

## 

![No conflict Merge][3]

## Example

Lets merge!

## Dastardly Divergent History

```
Auto-merging file.txt
CONFLICT (content): Merge conflict in file.txt
Automatic merge failed; fix conflicts and then commit the result.
```

## Dastardly Divergent History

* HEAD is not common ancestor
* Two diffs; Again Head vs ancestor and branch vs ancestor
* Change set between HEAD and branch is *not* disjoint

## Example

* Lets build a conflicting divergent history
* Lets merge it back into one lineage

[1]: images/basic-branching-3.png
[2]: images/basic-merging-1.png
[3]: images/basic-merging-2.png
