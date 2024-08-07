# Git Stash

Learn how to use the git stash command to stash uncommitted changes in this lesson.

## The git stash command

> Often, you will be working on your separate branch and making some changes that you don't want to commit just yet, but you will be required to switch over to another branch to do something else in between.
>
> You don't want to get rid of the changes but also don't want to commit them either. This exact scenerios is where you can use the **git stash** command.

**git stash** temporarily stores the staged and modified files in a kind of a cache, all the while making the working branch directory clean.

You could either stash all of the uncommitted changes you have made in the branch or stash individual files.

        git stash

## When to use git stash

> Let's say you are currently working on a branch called new_branch and you made some changes to the file1.txt.  
>  You can verify which branch you are on by using the command git branch and check which files have changed using the command git status.
>
> Now, for some other task, you are required to move to the master branch. However, the changes to file1.txt aren't ready to be committed yet, but you don't want to lose the changes.
>
> Ideally, you want to switch to the master branch where the changes you have made to file1.txt do not exist.  
>  Once you are done working with the master branch, you want to go back to new_branch and continue working on the changes you had started.

Here is what you will need to do:

1. Enter the command **git stash** while you are still on new_branch.
2. Enter the command **git checkout master** to switch to the master branch.
3. After you have done whatever you needed to do on the master branch, you will, once more, enter **git checkout new_branch** to switch back again.
4. You want your changes to be present once again, so you will enter the command **git stash apply**.
5. Enter **git status** to verify if your changes are back or not.

And there you have it.  
 The uncommitted changes you had made are all back again in your working directory, and you will be able to continue with your work uninterrupted once more.  
 You didn't have to commit your unfinished work, and you were able to switch branches and still keep your changes!

A win-win situatioon.

---

Had you decided not to use git stash, **Git would have prevented you from switching over to any other branch if the other branch had changes that would be overwritten with the new uncommitted changes** (since the changes in the other branch would be out of context).

You would have to do one of the following:

- Commit your unfinished work, switch branches, do your work, switch back to new_branch, and revert the most recent commit.
- Completely get rid of the changes you had made, switch branches, do your work, switch back to new_branch, and start all over again.

**In case the altered file does not conflict with the branch you plan to switch to**, _Git will let you switch over without errors and the uncommited changes would still be present in that branch as well._
