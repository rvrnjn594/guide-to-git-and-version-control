# Git Clone

Learn how to clone remote repositories to your local machine in this lesson.

## The git clone command

We can **use the git clone command to clone or copy the entire codebase of a project from a remote repository** and set it up as a local repository on our machines.

While cloning the project, two more actions occur as well:

1.  The git clone command will **also create a remote link to the remote repository being cloned** and name it origin.  
    This is similar to manually entering the command

        git remote add origin <remote_repository_url>.

2.  It will copy and **set up the primary branch, which is the master branch in most cases, as the active branch** in the working directory.

You can test this command out yourself in the terminal provided at the end of the lesson. You can look up a repository on GitHub that you like and clone it.

        git clone <link_to_repository>

#### Cloning a particular branch

In case you want to clone a branch that the HEAD in the remote repository doesn’t point to by default, you can also provide the name of that specific branch with the git clone command.

> For example, you might want to download or clone a branch other than the master branch.
>
>       git clone --branch <branch_name> <link_to_repository>

#### Shallow cloning

Sometimes, we might come across a remote repository that we want to clone, but its commit history might be too long, resulting in longer times to download and clone.

This occurs when the project is very large and has a very large commit history.  
 **You can opt to clone the commit history up to a certain point by using the --depth flag.**

Try the following command in the terminal provided below:

        git clone <repository_url> --depth 1

You can change the depth number according to your requirements.
