1) Taken from https://www.youtube.com/watch?v=ecK3EnyGD8o
----------------------------------------------------------------------
* ``` git commit -am "this biscally combines add and commit commands/action into one" ```
*  ``` git config --global alias.ac "commit -am"  ``` Here you created alias(aka/custom command) so now you can use ``` git ac "commit message" ``` instead of ``` git commit -am "commit message" ```
*  ``` git commit --amend -m "to simply update the latest commit" ``` or ``` git commit --amend --no-edit ``` --no-edit allow you to keep previous commit message
*  ``` git stash ``` this remove the changes from your working directory and save them to a stash. then if you want to bring them back just type ``` git stash pop``` you can also use ```git stash save [a name]``` to reference it later, then use ``` git stash list ``` to see a list of saved stashes, then use ``` git stash apply 0 ``` to apply your desired stash,here 0 is the index no. for your saved stash.
*  ``` git branch -m main ``` to rename your master branch to main.
*  ``` git rebase master -i HEAD~3 ``` this will show  file with many branches as n option to 
