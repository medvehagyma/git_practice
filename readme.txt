This is the first file in this repo.

This second line is written by Falesz after being invited. People or "collaborators" 
can be added to remote repositories on GitHub and then they can push commits to the repo.

This file is in a versioncontrolled folder called a repository.
When I make a change in this folder, I can use the following command to tell git, that i made a change that I would like to versioncontroll.
git add <file_name>
When I am satisfied with the changes I can tell git that I would like to keep these changes with the following command.
git commit -m <commit message text>

-m is short for message
The commit message should be a brief description of the changes contained within the commit.
Commit message convention
when you want to write a commit message ask to yourself what will this commit do 
the answer this commit will ... "make these changes"

Git is a versioncontroll system that tracks changes in text files. 
This is tipically used by programmers writing code. So it's a program that runs on your computer.
Git will be controlled with commands, the most important ones are git status, git add, git commit, git push, git pull.

GitHub is a hosting service, it provides free servers where programmers can put their remote repositories.
This allows them to work together on the same codebase asynchronously.

Commits are local changes that live on my computer.
When I want everyone else to start working with my changes I can push these commits to the remote reprository with the following command 
git push
Sometimes git push needs to be configured, because we need to tell it which remote repository to push to.
In this case we didn't need to configure it because we created the remote repository first on GitHub.
And then we used the cloning command to create the local reprository on my computer.
git clone https://github.com/medvehagyma/git_practice.git
Because of this in this local repository git automatically knows to push to this remote repository.