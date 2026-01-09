This is the first file in this repo.

This second line is written by Falesz after being invited. People or "collaborators" 
can be added to remote repositories on GitHub and then they can push commits to the repo.

This file is in a version controlled folder called a repository.
When I make a change in this folder, I can use the following command to tell git, that i made a change that I would like to version control.
git add <file_name>
When I am satisfied with the changes I can tell git that I would like to keep these changes with the following command.
git commit -m <commit message text>

-m is short for message
The commit message should be a brief description of the changes contained within the commit.
Commit message convention
when you want to write a commit message ask to yourself what will this commit do 
the answer this commit will ... "make these changes"

Git is a version control system that tracks changes in text files. 
This is tipically used by programmers writing code. So it's a program that runs on your computer.
Git will be controlled with commands, the most important ones are git status, git add, git commit, git push, git pull.
These git commands can be executed from the command line terminal or the git bash terminal. For beginners the command line terminal is recommended.
Because the command line terminal is a tool of the operating system and by using git from the cmd you also practice using the operating system.
Optionally if you are using some development environment that supports built in git usage you may also use that.
For example VSCode has a built in terminal that can also be used to execute git commands.
Other version control systems are Subversion (SVN) and perforce.

GitHub is a hosting service, it provides free servers where programmers can put their remote repositories.
This allows them to work together on the same codebase asynchronously.
Other popular version control hosting services are GitLab and BitBucket.

Commits are local changes that live on my computer.
When I want everyone else to start working with my changes I can push these commits to the remote reprository with the following command 
git push
Sometimes git push needs to be configured, because we need to tell it which remote repository to push to.
In this case we didn't need to configure it because we created the remote repository first on GitHub.
And then we used the cloning command to create the local reprository on my computer.
git clone https://github.com/medvehagyma/git_practice.git
Because of this in this local repository git automatically knows to push to this remote repository.

The following command may be used to view the last n count of commits with their authors, dates and commit messages.
git log -n <count>
example 
git log -n 5
Usually when you use this command in the terminal git will enter a commit view mode. While you are in this mode you can't use the terminal.
To quit this mode just press Q.

Git is a great tool for avoiding mistakes in the code base by making the development easy to follow, easy to track changes, revert to a previous
stat if I made a mistake and so on.
Many times however we make mistakes while using git itself for example we make a typo in a commit message. 
It is important to keep the git history clean and free of mistakes that could cause confusion. 
When we make a mistake using git we have many options to fix that.
One of the most commonly used is the interactive rebase.

git rebase -i HEAD~3
This means that I want to replay the last commits from the latest commit with some modifications that can be specified.
Alternatively this command says that I want to put the third commit onto the fourth commit with some modifications.