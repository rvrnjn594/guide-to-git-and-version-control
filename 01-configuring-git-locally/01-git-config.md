# Git Config

Learn how to set up Git for your local machine by familiarizing yourself with the Git config command.

## Installing Git

The Git software is a powerful command-line tool that you can install on your machine, whether you use windows, macOS, or Linux.

Once you havee Git installed on your machine, you will be able to use all the Git commands locally.

To verify that Git is installed successfully, try

        git --version

If Git is properly installed, the command above should display the installed version of Git that you are going to use.

## The git config command

The git config command works for a large variety of cases.  
 Moreover, the config command works on different levels.

Our main goal is to set our credentials that will identify our contributions and changes in the project source code.  
 Doing so will help us identify and differentiate between the changes made by various contributors.

#### The coding command works on different levels

We can set our credentials to be limited to a particular project, i.e., **locally**, or we can set them up **globally.**  
 Finally, we can also use the **config command to work on a system level.**

- Setting configurations at a **local level** will only affect the working project directory.
- Using the **global configuration** will result in the same configuration to apply to our repositories that the currently logged in user for that machine makes, except for the projects where the user has assigned a different local configuration.
- Configurations that are set up on a **system level** will, by default apply to all the users on that particular computer.

#### Setting our email and username for Git

We will set up our name and email globally for Git by using the following commands:

        git config --global user.email "rvrnjn594@gmail.com"

Similarly, we will also set up our username too:

        git config --global user.name "ravi ranjan"

You can verify you configurations for setting up the email and username by typing in the commands:

        git config user.email
        git config user.name

If they work fine, you should be able to see your desired email and username printed on the terminal.
