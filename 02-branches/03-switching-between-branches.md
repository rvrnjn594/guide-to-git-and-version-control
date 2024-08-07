# Swiching Between Branches

Learn how Git allows us to quickly switch between different branches.  
 This lesson also discusses an alternative way to create a new branch with Git.

## The git checkout command

Using the git branch command lets us create new branches seamlessly. However, the problem is that even though we get to create new branches, we still don’t actually know how to switch over to those branches and use them. The git checkout command lets us do just that.

Once you create a new branch (let’s call it new_branch), use the following command while still currently on the master branch, to switch over to that new branch:

        git checkout new_branch

## Creating new branches with git checkout

Right now, we need to rely on entering two separate commands to create a branch and then switch over it.

What if we could create a new branch that is a child of the branch that we are currently on and directly switch over it with just one command?  
 Well, **git checkout** lets us do that too.

#### The -b flag

Using the -b flag along with **git checkout** provides us with a convenient way to first implicitly execute **git brach** and then run **git checkout** to switch over to the newly created branch immediately.

        git checkout -b new_branch

> You've mastered how to create a new branch and switch over to it with one single command.

---

To really see the benefits of working on and creating new branches, try the following scenario out in the terminal provided above.  
 In the new branch that you just created, add a new file using the command:

        touch file2.txt

Then, make Git track this new file:

        git add file2.txt

Finally, commit the newly created file.

        git commit -m "created file2"

Now, you can switch back to the master branch, and you'll realize that the new file isn't there.
For now, it will only be available to you if the new branch is the active branch in the current directory.
