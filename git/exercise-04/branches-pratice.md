
#Brach

*Why doesn't a commit created on one branch appear on another branch?*

A branch is a "timeline" where your commits are made.

When we create a second branch and make commits on it, the first branch 
cannot access them because it is a separate "timeline."

That is why, if we use `git branch` to switch to another branch, make a 
commit, switch back to the previous branch, and run `git log --oneline`, 
we cannot see the commit from the second branch.


It is the result of the `git branch` command:

$ git branch
* main
  second-branch
