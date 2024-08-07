# Undo a Commit

Let's learn how to **undo or reset a commit from our local repository** in the lesson.

> While working on any project, it is common for us to make mistakes.  
>  For example, we might accidently delete files, misunderstood the requirements and code up something else.  
> Or just got stuck in some bug, and now we do not have a working copy of our code.

- There are several ways to fix these problems. We can simply nuke the local repository and create a new clone.  
   However, this approach will only work if we have a remote repository to fall back on.
- Another option would be to undo all the changes that we have made.  
   But, if our changes are present in multiple files, this process can be time-consuming. There is an easier alternative.

## The git reset command

The git reset command is a useful **tool to help fix past mistakes.**  
 There are a lot of ways it can be used depending on the scenario.

### Unstage files

Suppose you have staged some files to be commited. But later you change your mind and decide to unstage a few or all of them.  
 Maybe because you do not wish to commit them. To achieve this, we can simply use the following command:

        git reset

Type the following commands in the terminal below:

        touch file1.txt
        echo "Hello World" > file1.txt
        cat file1.txt
        git add file1.txt

At this point, file1.txt is staged and is ready to be committed.

        git status
        git reset
        git status

### Undo the last commit

What if while you are working on your project, you decide to create another file, file2.txt, and want to commit it into a new snapshot?

        touch file2.txt
        git add file2.txt
        git commit -m "added a new file"

##### The --soft flag

If you want to modify or update your changes from the previous commit but don't want to remove them completely, you can use the following command:

        git reset --soft HEAD~1

The --soft flag changes the state of the committed files to "staged".

Note how the output that git status command produces will change after you reset the most recent commit using the --soft flag. This flag preserves the changes.

##### The --hard flag

If you want to completely get rid of the changes that were part of the recent commit, you can use the --hard flag instead.  
 It will reset the changes and not preserve them

        git reset --hard HEAD~1

---

The git reset command can prove to be very useful if we want to update or revert changes made in older commits.  
 The example shown above dealt with reverting only the most recent commit.  
 You will have notices the reset commands used in this lesson had the **HEAD~1 portion. The number indicates how many commits you want to go back**.

If you're going to reset several older commits, you can change the number to how many commits you want to be reverted, and that will land back to an earlier snapshot of you project.

For example:

        git reset --soft HEAD~2

would revert the two most recent commits.
