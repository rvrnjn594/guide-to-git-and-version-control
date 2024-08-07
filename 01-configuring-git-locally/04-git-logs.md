# Git Logs

Let's take a deeper look at the **commit structure and see how we can view our commit history** using the Git log command.

## The git log command

Git tracks changes to a project by maintaining a chain of snapshots or commits.

If you are working on a collaborative project, you will find that your repository will have commits from different contributors.  
 The git log command lets you view the commit history for you project.

Entering the **git log command is you terminal will allow you to view a list of commits or snapshots that will be sorted based on the time they were created** with the latest one at the very top.

---

Each log will contain information about the author of the commit, displaying their username and email that we set with the git config command.

The log will also contain a timestamp of when each commit was creted along with the commit message.

One more critical piece of information that the log will show is the **40-characters-long unique hash**.  
 The hash is vital because it **helps identify commits and acts as an excellent way to secure the commit**.

> The commit hash **uses the cryptographic hash function SHA-1**. The hash key allows each commit to have integrity.  
>  If the hash were to change, we would be able to identify that the commit has been tampered with.
