this is my app


git commands
-------------------------------------------


configure your username and email(just a local record)

* git config --global user.name "Pushkar Shrivastava"
* git config --global user.email "pushkar.shv@gmail.com"
----------------------------------------------------------
from https://www.youtube.com/watch?v=SWYqp7iY_Tc

* git int                 			   //initialize local git repository
* git add <file>				    // add file(s) To index,or to staging or to be tracked by git
* git status 					    // check status of working tree
* git diff					   // to see the differences between your staged and unstaged/modified file(s).
* git diff --staged			  	 // to see differences in every previous stages.
* git commit 				   	// Comit Changes in index
* git commit -m "commit message"		//to commit with a message
* git commit -a -m "Direct commit"          // commit files directly,from tracked state. and skip the staging phase
* git rm "file name" or git mv "file name" "new file name" => {to change file names}    // having a git keyword before these type of command auto stages the output of command
// upon adding a file to .gitignore,you should also run [git rm --cached <file name>] command to untrack those ignored files from git

* git log				// this command gives a brief info of all commits done on your project
* git log -p 				// it also tell what is being removed and add in your log info
* git log -p -<number>			// gives only the number of commit as you specified
*git log --stat				//give slightly less breif info of commit
* git loog --pretty=<oneline>,<short>,<full>    //another way to represent your commit logs

* git checkout --<file name>              // to bring you file state back to prevoius commit state
* git checkout -f			// to bring you project state back to prevoius commit state

// for security plz add ssh. reference = "https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent"

* git pull 				  // pull latest version of repo from remote repository
* git clone 				   // clone Repository into a new directory
* rm -rf .git         			     // this will remove your .git folder and end all git services to your project.

* git add *.<html>  				//to add all files with html extension to staging or be tracked by git
* git add .  or   git add --a   		  // to add all files
* git rm --cached <file name>  			//to remove a file from staging area

create a file with :- touch <file name>

add a file name inside .gitignore to ignore the specified file being accessed by git.

* git branch <branch name>     // to add a branch to your project.while you are in a branch,you cannot see any file created in other branches

* git checkout <branch name>    // to switch to the specified branch...by defaulf all projects have a master branch.

* git merge <branch name>   //to merge a specified branch to the master branch.first switch to the master branch then use merge command.

* git remote add origin https://github.com/ArcaneTrickster/myappsample.git   // to add a remote connection for your project folder to another folder on github.

* git remote           //to see all remote connections existing.

* git push -u origin master     //to upload your project to github folder. with master as a branch.

* git clone <github link>   //to download a git project.

* git pull    // to download an upto-date version of github project.


