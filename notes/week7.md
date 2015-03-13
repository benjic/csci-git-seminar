% Week 7
% Merging 
% March 11 2015

# Merging

## Review

* `git merge <target_branch>`
* Merge Instructs git to compare the current branch and target branch
* Take the differences between their common ancestor and combines them
* CONFLICT

## Git Alpha 

* A file containing a list of alphabetized words
* We merged consonants and vowels into a respective branches
* Finally we merged the *meta* branches into the main **master** branch
* This was repetitive but fairly strait forward

## Git Fibonacci

* Real world example
* Two implementations of Fibonacci sums; Want to merge iterative version
* The conflict is terrible
* Lets look...

## Merge Abort

* Bailing out is important 
* `git merge --abort`
* Reverts working directory to pre merge state

## Merge Strategy

* Algorithms to choose the better difference
	* Resolve
	* Recursive
	* Octopus
	* *others*

## Resolve Strategy

* Hope for the best
* Spends a little extra time to gain information
* *Guesses* how to resolve conflict

## Recursive

* Default merge strategy
* Options
	* *ours* and *theirs*
	* *ignore-<whitespace>*
* Wait, lets try *theirs*

## Git Fibonacci

* `git merge -s recursive -X theirs iterative_refactor`
* Wait, if there is no conflict
	* How do we know its correct
	* How do we revert

## --no-commit

* `git merge -s recursive -X theirs --no-commit iterative_refactor`
* Stops merge just before commit
* Allows inspection and opportunity to test

## Octopus

* Allows merging of many heads
* Context: If there are many independent heads
	* The merge must be trivial

## Tips

* Practice 
* Pick your battles
	* It is much easier to merge your own commits
	* Do so often and aim for triviality
* Use --abort and --no-commit to confirm merges

## Q & A

* Questions?
* Stories?

