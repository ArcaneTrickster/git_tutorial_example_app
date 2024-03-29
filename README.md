this is a dummy app for git tutorial

also see https://guides.github.com/features/mastering-markdown/ for markdown guide.

download git from www.git-scm.com and gitbash is the terminal i used here.

------------------------------------------
configure your username and email so your uploads are marked with your name and email. (optional probably)

* ``` git config --global user.name "Pushkar Shrivastava" ```
* ``` git config --global user.email "pushkar.shv@gmail.com" ```
----------------------------------------------------------

* ``` git init                 			   ```initialize local git repository.
* ``` git add [file]				    ``` add file(s) To index,or to staging, or to be tracked by git. 
									```git does not track you files unless you instruct git to do so. After files are tracked/staged/indexed, you can go further.
* ``` git add * .[html]  				``` to add all files with html extension to staging or be tracked by git.
* ``` git add . ``` or   ``` git add --a   		  ``` to add all files for staging.
* ``` git rm --cached [file name]  			```to remove a file from staging area.
* ``` git status 					    ``` check status of working tree.
* ``` git diff					   ``` to see the differences between your staged and unstaged/modified file(s).
* ``` git diff --staged			  	 ``` to see differences in every previous stages.
* ``` git reset 						``` this will unstage all the staged/tracked files.
* for security plz add ssh. reference = "https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent" , "https://devmarketer.io/learn/set-ssh-key-github/"

* for ssh
* ``` ssh-keygen -t rsa -b 4096 -C "your_email@example.com" ``` -t = type,-b = byte size, -C = label, It will asks you a few things like what should be the file name in which you want to save the shh key. I use multiple files for multiple accounts, each for each github account.
* ``` eval `ssh-agent -s`  ``` to start ssh agent
* ``` ssh-add ~/.ssh/id_rsa  ``` this add/register the generated ssh to ssh agent
* ``` clip < ~/.ssh/id_rsa.pub  ``` to copy ssh text to clipboard
* next part of ssh is on reference = "https://help.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent" , "https://devmarketer.io/learn/set-ssh-key-github/"

* ``` git commit -m "commit message"		```to commit with a message.
* ``` git commit -a -m "Direct commit"          ``` commit files directly,from tracked state. and skip the staging phase.
* ``` git rm "file name" ``` or ```git mv "file name" "new file name" ``` to change file names    ``` having a git keyword before these type of command auto stages the output of command.
* upon adding a file to .gitignore,you should also run ```git rm --cached [file name] ```command to untrack those ignored files from git.

* ``` git remote add origin https:github.com/USERNAME/REPOSITORY.git ``` to add a remote connection for your project folder to another folder on github.
* ``` git remote set-url origin https://github.com/USERNAME/REPOSITORY.git    ``` to update an existing link.
* ``` git remote rm origin ``` to remove a link completely,it works only at local pc not on remote.

* ``` git remote           ```to see all remote connections existing.

* ``` git push -u origin master     ```to upload your project to github folder. with master as a branch.


* ``` git push origin [branch name]     ```this will create a new branch of your branch name at remote repository and push the code.

* ``` git push origin [branch name]:[branch name at remote]    ```this will create a new branch at remote repository with specified name and push the code.

* ``` git clone [github link]   ```to download a git project.

* ``` git pull    ``` to download an upto-date version of github project.

* ``` git log				``` this command gives a brief info of all commits done on your project.
* ``` git log -p 				``` it also tell what is being removed and add in your log info.
* ``` git log -p -[number]			``` gives only the number of commit as you specified.
* ```git log --stat				```give slightly less breif info of commit.
* ``` git log --pretty=[oneline],[short],[full]    ```another way to represent your commit logs.

* ``` git checkout --[file name]              ``` to bring you file state back to prevoius commit state.
* ``` git checkout -f			``` to bring you project state back to prevoius commit state.

* ``` git config --global alias.[alias name] '[your command you want to have an alias for]'      ``` this way we can give a short name for a command in git so when we write the short name,its corresponding command is used by git.

* ``` git clone 				   ``` clone Repository into a new directory.
* ``` git pull 				  ``` pull latest version of repo from remote repository.
* ``` rm -rf .git         			     ``` this will remove your .git folder and end all git services to your project.

*  if you delete something on your project and want to move to previous state,use :-
* ``` git fetch origin master ```
* ``` git reset --hard FETCH_HEAD ```
  
* create a file with ```touch [file name]```.

* add a file name inside .gitignore to ignore the specified file being accessed by git.

* ``` git branch   ``` to see all branches you have.

* ``` git branch [branch name]     ``` to add a branch to your project.while you are in a branch,you cannot see any file created in other branches. this command does not execute if you have just initialized git and haven't added and performed your first commit.

* ``` git checkout [branch name]    ``` to switch to the specified branch...by defaulf all projects have a master branch.

* ``` git merge [branch name]   ```to merge a specified branch to the master branch.first switch to the master branch then use merge command.

* ``` git branch --merged   ```to see merged branches.

* ``` git branch --no-merge  ```to see branches which are not merged.

* ``` git branch -d [branch name]   ```to delete a specified branch. git will give a warning message if the branch is not merged to master and ask you to rewrite command with a capital D again.




