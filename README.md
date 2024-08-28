# Github-Git

## Module 1 Glossary: Git and GitHub Fundamentals
Welcome! This alphabetized glossary contains many of the terms in this course. This comprehensive glossary also includes additional industry-recognized terms not used in course videos. These terms are essential for you to recognize when working in the industry, participating in user groups, and in other professional certificate programs.

Estimated reading time: 4 minutes

Term	Definition
Branch	A separate line of development that allows to work on features or fixes independently.

Clone	A local copy of the remote Git repository on the computer.

## Commit	- A snapshot of the project's current state at a specific point in time, along with a description of the changes made.
## Continuous delivery (CD)	- The automated movement of software through the software development lifecycle.
## Continuous integration (CI) -	A software development process in which developers integrate new code into the code base at least once a day.
## Distributed version control system (DVCS) - 	A system that keeps track of changes to code, regardless of where it is stored. Multiple users work on the same codebase or repository, mirroring the codebase on their computers if needed, while the distributed version control software helps manage synchronization amongst the various codebase mirrors.
## Fork	- A copy of a repository into your GitHub account.
## GitHub -	A web-hosted service for the Git repository.
## GitHub - branches	A branch stores all files in GitHub. Branches are used to isolate changes to code. When the changes are complete, they can be merged back into the main branch.
## GitLab -	A complete DevOps platform delivered as a single application. It provides access to Git repositories, controlled by source code management.
## Git - Free and open-source software distributed under the GNU General Public License. It is a distributed version control system that allows users to have a copy of their own project on their computer anywhere in the world.
## Merge - A process to combine changes from one branch to another, typically merging a feature branch into the main branch.
##Pull request -	A process used to request that someone review and approve your changes before they become final.
## Repository -	A data structure for storing documents, including application source code. It contains the project folders that are set up for version control.
## SSH Protocol - 	A method for secure remote login from one computer to another.
## Version control -	A system that allows you to keep track of changes to your documents. This process allows you to recover older versions of the documents if any mistakes are made.
## Working directory -	A directory in your file system that contains files and subdirectories on your computer that are associated with a Git repository.
----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
## Le tableau suivant présente différentes commandes Git :

git init

git checkout

git revert

git-format-patch

git fetch upstream

git status

git merge

git config --global user.email

git-request-pull

git merge upstream/main

git add .

git clone

git config --global user.name

git-send-email

git pull upstream

git commit

git pull

git remote -v

git-am

git web

git log

git push

git remote rename

git-daemon

git-instaweb

git reset

git version

git remote add origin

git remote -v

git-pull downstream

git branch

git diff

git-remote

git remote add upstream

git-rerere
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------Reading: Git Commands
In this reading, you will summarize and describe additional Git commands that you may use while working on your projects. You will also look at the syntax for each command.

Git is a widely used version control system that offers numerous benefits to developers and teams working on software development projects.

Let's look at some useful Git commands and understand them:

git add

Description: It adds changes to the staging area. This command stages the changes made to the files and prepares them for the next commit.

Syntax:

git add <filename.txt> (to add a specific file)
git add . (to add all the files that are new or changed in the current directory)
git add -A (to add all changes in the entire working tree, from the root of the repository, regardless of where you are in the directory structure)
git reset

Description: It resets changes in the working directory. When used with –hard HEAD, this command discards all changes made to the working directory and staging area and resets the repository to the last commit (HEAD).

Syntax:

git reset
git reset –hard HEAD
git branch

Description: It lists, creates, or deletes branches in a repository. To delete the branch, first check out the branch using git checkout and then run the command to delete the branch locally.

Syntax:

git branch (to list branches)
git branch <new-branch> (to create a new branch)
git branch -d <branch-name> (to delete a branch)
git checkout main

Description: It switches to the "main" branch. This will switch your current branch to "main."

Syntax: git checkout main

git clone

Description: It copies a repository from a remote source to your local machine. This will create a copy of the repository in your current working directory.

Syntax: git clone <repository URL>

git pull

Description: It fetches changes from a remote repository and merges them into your local branch. First, switch to the branch that you want to merge changes into by running the git checkout command. Then, run the git pull command, which will fetch the changes from the main branch of the origin remote repository and merge them into your current branch.

Syntax: git pull origin main

git push

Description: It uploads local repository content to a remote repository. Make sure you are on the branch that you want to push by running the git checkout command first, then push the branch to the remote repository.

Syntax: git push origin <branch-name>

git version

Description: It displays the current Git version installed on your system.

Syntax: git version

git diff

Description: It shows changes between commits, commit and working tree, etc. It also compares the branches.

Syntax:

git diff (shows the difference between the working directory and the last commit)
git diff HEAD~1 HEAD (shows the difference between the last and second-last commits)
git diff <branch-1> <branch-2> (compares the specified branches)
git revert

Description: It reverts a commit by applying a new commit. This will create a new commit that undoes the changes made by the last commit.

Syntax: git revert HEAD

git config –global user.email <Your GitHub Email>

Description: It sets a global email configuration for Git. This needs to be executed before doing a commit to authenticate the user's email ID.

Syntax: git config –global user.email <Your GitHub Email>

git config –global user.name <Your GitHub Username>

Description: It sets a global username configuration for Git. This needs to be executed before doing a commit to authenticate users' username.

Syntax: git config –global user.name <Your GitHub Username>

git remote

Description: It lists the names of all remote repositories associated with your local repository.

Syntax: git remote

git remote -v

Description: It lists all remote repositories that your local Git repository is connected to, along with the URLs associated with those remote repositories.

Syntax: git remote -v

git remote add origin <URL>

Description: It adds a remote repository named "origin" with the specified URL.

Syntax: git remote add origin <URL>

git remote rename

Description: The git remote rename command is followed by the name of the remote repository (origin) you want to rename and the new name (upstream) you want to give it. This will rename the "origin" remote repository to "upstream."

Syntax: git remote rename origin upstream

git remote rm <name>

Description: It removes a remote repository with the specified name.

Syntax: git remote rm origin

git format-patch

Description: It generates patches for email submission. These patches can be used for submitting changes via email or for sharing them with others.

Syntax: git format-patch HEAD~3 (creates patches for the last three commits)

git request-pull

Description: It generates a summary of pending changes for an email request. It helps communicate the changes made in a branch or fork to the upstream repository maintainer.

Syntax: git request-pull origin/main <myfork or branch_name>

git send-email

Description: It sends a collection of patches as emails. It allows you to send multiple patch files to recipients via email. Please make sure to set the email address and name using the git config command so that the email client knows the sender's information when sending the emails.

Syntax: git send-email *.patch

git am

Description: It applies patches to the repository. It takes a patch file as input and applies the changes specified in the patch file to the repository.

Syntax: git am <patchfile.patch>

git daemon

Description: It exposes repositories via the Git:// protocol. The Git protocol is a lightweight protocol designed for efficient communication between Git clients and servers.

Syntax: git daemon –base-path=/path/to/repositories

git instaweb

Description: It instantly launches a web server to browse repositories. It provides a simplified way to view repository contents through a web interface without the need for configuring a full web server.

Syntax: git instaweb –httpd=webrick

git rerere

Description: It reuses recorded resolution of previously resolved merge conflicts. Please note that rerere.enabled configuration option needs to be set to "true" (git config –global rerere.enabled true) for git rerere to work. Additionally, note that git rerere only applies to conflicts that have been resolved using the same branch and commit.

Syntax: git rerere
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------Module 2 Cheat Sheet: Git Commands and Managing GitHub Projects
Package/Method	Description	Code Example
git add	Used to move changes from the working directory to the staging area	
1
git add sample.md
Copied!
git add .	Allows to move the changed files into the staging area on GitHub repositories	
1
git add .
Copied!
git am	Used to apply patches emailed to the repository	
1
git am < patchfile.patch
Copied!
git branch	Allows to create an isolated environment within the repository to make changes	
1
git branch <new-branch>
Copied!
git checkout	Allows to see and change existing branches	
1
git checkout <existing-branch>
Copied!
git checkout main	Allows to switch to the main branch	
1
git checkout main
Copied!
git clone	Allows to create a copy of the remote repository	
1
git clone <repository-url>
Copied!
git commit	Allows you to take staged snapshots if changes and commit them to the project	
1
git commit -m "Your commit message here"
Copied!
git config --global user.email	Example 1: Sets a global email configuration for Git

Example 2: Sets a global username configuration for Git	Example 1:
1
git config --global user.email "your.email@example.com"
Copied!


Example 2:
1
git config --global user.name "Your Name"
Copied!
git daemon	Used to allow anonymous download from the repository	
1
git daemon --reuseaddr --verbose
Copied!
git diff	Helps others to review your code to identify and compare the changes	
1
git diff example.txt
Copied!
git fetch	Used to transfer the changes from the remote repo to your local repo	
1
git fetch <options> <remote name> <branch name>
Copied!
git fetch upstream/master	Used to grab upstream branches	
1
git fetch upstream master:upstream-master
Copied!
git format-patch	Generates or prepares e-mail submission if you adopt Linux kernel-style public forum workflow	
1
git format-patch -n <number_of_commits>
Copied!
git http-backend	Provides a server-side implementation of Git-over-HTTP, allowing both fetch and push services	
1
2
3
git clone --bare /path/to/repos/myrepo.git
cd myrepo.git
git update-server-info
Copied!
git init	Used to clone an existing repository	
1
git init <directory>
Copied!
git instaweb	Allows to set up web front-end to Git repositories	
1
git instaweb -p 8080
Copied!
git log	Enables to browse previous changes to a project	
1
git log -p filename
Copied!
git merge	Used to merge changes in the active branch into another branch	
1
git merge feature_branch
Copied!
git merge upstream/master	Merges changes from the 'upstream/master' branch to the current branch	
1
git merge upstream/master
Copied!
git pull	Used to transfer the changes from the remote repo to your local repo, and merge them to a branch	
1
git pull origin main
Copied!
git pull downstream	Pulls changes from a downstream repository, specifically from the master branch of that repository	
1
git pull downstream main
Copied!
git pull upstream	Pulls changes from the "upstream" repository into the current branch	
1
git pull upstream main
Copied!
git push	Used to push all the committed changes into the repository	
1
git push origin your_branch_name
Copied!
git remote	A command to manage a set of tracked repositories	
1
git remote add upstream https://github.com/original/repo.git
Copied!
git remote add origin <URL>	Adds a remote repository named "origin" with the specified URL	
1
git remote add origin https://github.com/yourusername/your-repo.git
Copied!
git remote add upstream	Adds the original repository as a new remote repository labeled upstream	
1
git remote add upstream https://github.com/original/repo.git
Copied!
git remote rename	The git remote rename command is followed by the name of the remote repository(origin) you want to rename and the new name(upstream) you want to give it	
1
git remote rename origin new-origin
Copied!
git remote -v	Allows to view the remotes associated with the local repository	
1
git remote -v
Copied!
git request-pull	Example 1: Creates a summary of changes for your upstream to pull

Example 2: Generates a summary of pending changes for an email request	Example 1:
1
git request-pull origin/main your-branch
Copied!


Example 2:
1
git request-pull <base> <head> <repository>
Copied!
git rerere	Reuses recorded resolution of previously resolved merge conflicts	
1
2
git rerere
git rerere diff
Copied!
git reset	Undoes changes that were made to the files in your working directory	
1
git reset HEAD~1
Copied!
git revert	Used to undo botched commits	
1
git revert HEAD
Copied!
git send-email	Example 1: Sends your email submission without corruption by your MUA

Example 2: Sends a collection of patches as emails	Example 1:
1
2
git send-email --to=recipient@example.com
path/to/patchfile.patch
Copied!


Example 2:
1
2
git send-email --to recipient@example.com
patches/*.patch
Copied!
git-shell	Used as a restricted login shell for shared central repository users	
1
sudo usermod -s /usr/bin/git-shell gituser
Copied!
git status	Allows to see the state of your working directory and the staged snapshot of the changes	
1
git status
Copied!
git version	Displays the current Git version installed on your system	
1
git --version
Copied!
git web	Provides a web front-end to Git repositories	
1
git instaweb --port=8080
---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
Module 2 Glossary: Git Commands and Managing GitHub Projects
Welcome! This alphabetized glossary contains many of the terms in this course. This comprehensive glossary also includes additional industry-recognized terms not used in course videos. These terms are essential for you to recognize when working in the industry, participating in user groups, and in other professional certificate programs.

Estimated reading time: 4 minutes

Term	Definition
## Cloning	A process of creating a copy of the project's code and its complete version history from the remote repository on the local machine.
## Commit	A snapshot of the project's current state at a specific point in time, along with a description of the changes made.
## Developer	A computer programmer who is responsible for writing code.
## Distributed version control system (DVCS)	A system that keeps track of changes to code, regardless of where it is stored. Multiple users work on the same codebase or repository, mirroring the codebase on their computers if needed, ## while the distributed version control software helps manage synchronization amongst the various codebase mirrors.
## Fork	A copy of a repository into your GitHub account.
## Forking	Forking creates a copy of a repository on which one can work without affecting the original repository.
## GitHub	A web-hosted service for the Git repository.
## Git	A free and open-source software distributed under the GNU General Public License. It is a distributed version control system that allows users to have a copy of their own project on their computer anywhere in the world.
## Integrator	A role that is responsible for managing changes made by developers.
## Master branch	A branch that stores the deployable version of your code. The master branch is created by default and is definitive.
## Merge	A process to combine changes from one branch to another, typically merging a feature branch into the main branch.
## Origin	A term that refers to the repository where a copy is cloned from.
## Pull request	A process used to request that someone review and approve your changes before they become final.
## Remote repositories	Repositories that are stored elsewhere. They can exist on the internet, on your network, or on your local computer.
## Repository administrator	A role that is responsible for configuring and maintaining access to the repository.
## Repository	A data structure for storing documents, including application source code. It contains the project folders that are set up for version control.
## Staging area	An area where commits can be formatted and reviewed before completing the commit.
## Upstream	A term used by developers to refer to the original source where the local copy was cloned from.
## Version control	A system that allows you to keep track of changes to your documents. This process allows you to recover older versions of the documents if any mistakes are made.
