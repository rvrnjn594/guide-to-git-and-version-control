# Deleting a Brach

Learn how to delete a branch from your local repository in this lesson.

## Using git branch to delete a branch

We can use the git branch command to **create, list, rename, and delete a branch**.  
 In this lesson, we will take a new look at how we can delete a branch from our repository.

#### The -d flag

The syntax for deleting a brach is fairly simple:

        git branch -d <branch_name>

If you have a branch called **new_branch** in your repository and want to remove it, you will need to enter the following command:

        git branch -d new_branch

As always, to double-check that the deletion process has been executed successfully, you can rely on the simple **git branch** command to verify this.  
 The branch that is deleted should no longer be listed in the output.

> **NOTE:** You can't delete the branch you are currently on. You will need to switch over to another brach and then delete it.
