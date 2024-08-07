# Creating a New Project With Git

In this lesson, you will create a new project and learn how to use Git to track it.

## Creating a new project directory

Let's start by creating a new working directory or folder in the terminal.  
 We'll call the new working directory test_project.  
 You can create a new directory by using the following command:

        mkdir test_project

Once we have created the new directory, we will need to set that as the current working directory.
We will do that by entering the following command:

        cd test_project

Once test_project directory becomes the working directory, which will be initially empty, we will create a plain text file.  
Let's call it file1.txt.

        touch file1.txt

To verify that the file was created, enter the plain command ls. It should print all the folders and files present withing the working directory, which, in our case, is file1.txt.

## The git init command

We can initialixe Git to track this project and its content:

        git init

The **git init** command simply creates an empty repository.  
 Therefore, your project will not automatically come under the ambit of version control with this command alone.

What git init does, however, is create a .git directory.  
 The .git directory will **contain all the metadata that Git will require for tracking the project**.

## The git add command

Now that we have a project that has a file and an empty Git repository set up, we want Git to track the contents of the entire project.  
 At this point, the git add command will help us. Enter the following command in the test_project directory.

        git add .

This will result in all of the contents within the test_project directory to be tracked by Git.

## The git status command

To verify what state your files in the repository are in, you can use the git status command.  
 It doesn't change or update anything.  
 Instead, it prints out which files are modified, staged, or untracked.

        git status

> Look at the kind of information you get with git status. You can identify when file1.txt is untracked by Git and how it then changes to a staged state.  
>  As you get more familiar with Git and use it more often, you will find yourself checking the status of your files quite often.
