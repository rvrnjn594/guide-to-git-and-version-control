# Renaming Branches

Learn how to rename a branch in this lesson.

Git provides a very convenient way to rename the new brach you've created.  
We'll once again, **rely on git branch command to rename an existing branch**.

> Let's say you have been working on a significant feature. You want to add authentication to your application. The branch that you are making all the relevant changes to is called **new_branch.**  
>  The name new_branch is not related to what you are doing in any way. No one else will be able to identify what this branch is about, either. It is better idea to call it something like **authentication_feature**.

## Renaming a branch you are currently on

1.  Switch over to the branch you have to rename with the following command:

        git checkout new_brach

2.  Use the git branch command appended with the -m flag to provide the new name:

        git branch -m authentication_feature

To verify that you were able to rename the branch, use the plain git branch command to print out the list of branches and you will be able to see that the current branch you are on is now called "authentication_feature" instead of just new_branch.

## Renaming a branch without switching over to it

What if you want to rename the branch but want to remain on the branch that you are originally using at the moment?  
 The **git branch** command can do that too.

The general syntax for doing so is:

        git branch -m old_name new_name

> Therefore, if you want to rename new_branch as authentication_feature but also want to remain on the master branch, you would enter this command:
>
>           git branch -m new_branch authentication_feature

Once again, you can use the plain **git branch** command to verify if the branch has the new name or not.
