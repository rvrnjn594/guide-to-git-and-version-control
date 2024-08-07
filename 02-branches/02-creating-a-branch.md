# Creating a Branch

Learn how Git lets us create branches seamlessly and quickly.

## The git branch command

The git branch command is useful, multi-purpose tool that lets us do a lot of different things.  
 When used as is (without any other options appended), the command will print out all the branches present in the repository and point out which branch we are currently on.

        git branch

The git branch command will print out the master branch with a prepended asterisk.  
 The asterisk denotes that this also happens to be the branch that is currently active in our repository.  
 In other words, we are currently using the master branch. If there were more branches, their names would also be listed.

## How to create a new branch

To create a new branch, we will need to modify the git branch command by appending a branch name.

        git branch my_new_branch

> It is preferred that the new branch not have a very long name or spaces in between.

After you create the new branch, enter the plain git branch command to double-check that it works.  
 You will know if it works because the name will now be printed along with the master branch.

One critical point to realize if you want to create a new branch in this manner is that you will still be using the parent branch in your current working directory.  
 That should be easy to identify, given the asterisk (\*) next to the master branch name.

This is significant point that you shouldn't ignore.  
 If you want to now switch to the newly created branch from the master, that is where the **git checkout** command will help you.
