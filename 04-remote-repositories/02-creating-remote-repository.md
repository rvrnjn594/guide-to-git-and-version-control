# Creating a Remote Repository

Learn how to create a remote repository for projects on GitHub.

## Creating your first repository on GitHub

Once you are logged in and are on the homepage, you will notice a button on the top left side titled ‘New'.

Once you click on the ‘New’ button, GitHub will redirect you to a different page where you will have to provide a name for the repository.  
 Additionally, you can add a description of your repository. You may provide the sample information given below for your first repository:

- Name: test_project
- Description: “The first repository that I will use to learn Git commands.”

#### Public and private repositories

Besides providing a name and description, you need to choose whether you **want your repository to be public or private.**

- As the name suggests, **a public repository is accessible to anyone who wants to look it up.**  
   Anyone is able to see the codebase and clone this repository to their local machine for use.
- Since you are creating your first repository and will only be using it to learn Git and GitHub, it would be wise to opt for a private repository.

## The README file

Another decision you will have to make while creating a new repository is whether or not you’ll create a README file.

The **README file contains necessary information about the repository.**

> For example, it might include the following information:
>
> - Instructions on how to clone and run the source code on local machines
> - A basic guide on how to use the library or package that the repository contains
> - What to do if you come across certain kinds of bugs
> - Licensing and copyright information
> - Contact information about people who contributed to the code

For now, let’s opt to create a repository that won’t have a README.  
 GitHub will provide you with the option to choose to initialize a project with or without a README:

## The .gitignore file

Finally, you will be able to choose whether or not you want a .gitignore file with your repository.  
 The **purpose of the .gitignore file is to filter out files and subdirectories in your repository that you do not want Git to keep track of.**

Therefore, any changes you make to **files contained in a .gitignore file will not be marked as modified, staged, or committed by Git.**

> Here is an example of a .gitignore file:
>
>       # if you don't want to track a single file
>       abc.txt
>
>       # if you don't want to track files with a certain extension
>       *.pyc
>
>       # if you don't want to track a directory
>       htmlcov/

For now, you can opt not to create a .gitignore file with your repository.  
 Once you fill in all the options, you will be ready to create your GitHub repository.
