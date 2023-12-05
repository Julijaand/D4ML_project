# D4ML_project
D4ML is DevOps and Infrastructure Engineering Research &amp; Development project

#Task
As a junior DevOps engineer, you have a message from your Team Lead.
He wants a list of commands which could be used to achieve the next things:

#Task 
Install Git Bash:

Download from official website and follow the steps:
Git - Downloads (git-scm.com)

#Task
Initialize a new local repository:

$ cd /path	 			note path for project folder
$ mkdir D4ML_project 	 		create folder for project
$ git init 				creates an empty Git repository

#Task
Create a README.md file and put a few lines in there using Markdown syntax. Commit changes to master branch

$ cd D4ML_project	 		move to project directory
$ touch README.md			create readme.md file
$ vim README.md				make notes in readme file
$ git add README.md			adds file to index
$ git commit -m “commit message”	performs a commit, and the -m "message" adds a message	

#Task
Create 3 versions of master branch with names feature_a/b/c.

$ git branch Feature_A/ Feature_B/ Feature_C 		creates branches
#Task
Make different changes in each branch and commit them.

$ git checkout Feature_A		change branch
$ touch main.htm main2.html 		create files
$ vim main.htm				edit files
$ git add				adds file to index
$git commit -m “commit message”	performs a commit, and the -m "message" adds a message

#Task
Merge changes from all feature branches to feature_d branch.
$ git branch Feature_D				creates Feature_d branch
$ git checkout Feature_D			changes branch	to Feature_d
$ git merge Feature_A Feature_B Feature_C	Merge changes from all feature branches to feature_d branch
$ git add .
$git commit -m “commit message”

#Task
Merge feature_d to master.
$ git checkout main
$ git merge Feature_D
$ git push 

#Task
Check if you have all changes in master branch.
$ git branch		check if in main branch
$ ls -la		lists all files and directories in current branch	

#Task
Check what was changed and what was added commit by commit. You could play more with branches and code changes in your local repo to be more familiar with the background processes of 
$ git reflog 		history commits

#Task
Change git to a remote origin which is your gitlab/github account. Make sure your remote repository is accessible for team

$ git remote add origin <https://github.com/Julijaand/D4ML_project.git>
$ git remote -v
$ git push --set-upstream origin main
