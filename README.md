# GitHub Tutorial

_by < Mahmoud  Bakr >_

---
## Git vs. GitHub
 Git is a version control system that allows software developers to track changes to their projects over time locally, Github on the other hand is a remote where software developers can push (upload) their saved changes (from git) to and then it can be used to collaborate with others. 
![]()


---
## Initial Setup
 In order to start using the various features of git and github you will need a github account.
 1. Go to [Github.com](https://github.com/)
 2. On the top right hand corner press on **Sign up**
 3. Follow the instructions and your github account is ready to be used 
 -------
 Now you will need to set up your IDE where all your files are going to be
1. Go to the [CS50 IDE](https://ide.cs50.io/)
2. Sign in with your [Github](https://github.com/)
3. Once you are in follow [these](https://github.com/hstatsep/ide50) instructions to set up your ide

_Its important to set up the **SSH key** because without it you will need to verify yourself every single time you try to use the IDE._ 


---
## Repository Setup
1. In your IDE create a directory using **mkdir**
2. **cd** into your created directory 
3. Now you will have to initialize git in your directory using the command **git init** .  _If done correctly, now in your command line next to the directory name you should see (master)_
4. Go to [Github](https://github.com/)
5. On the top right hand corner press on the plus sign and then press **New Repository**
6. Under repository name, give your repository a name and then press create repository
7. On the top make sure you select SSH 
8. copy the two lines of code under (**…or push an existing repository from the command line**) into your command line

 ```
 git remote add origin git@github.com:(your_username)/(repository_name).git 
 git push -u origin master 
 ```


_If all steps are done correctly, your local repository now has a remote that you can push your changes too_



---
## Workflow & Commands
 1. Go into your local repsitory using ```cd```
 2. Make sure next to the file name on the command line it says ```(master)``` 
 3. In order to add stuff to the folder that we will be able to track using Git we will need a README file using the command ``` touch README.md ```
 4. The open the README file using the command ```c9 README.md```
 5. In the README file write anything then go back to the command line 
 6. In order to check the status of the files in the folder use the command ```git status``` which will show the files and if they are in red then they can't be commited yet or they arent ready for git to take a snapshot of them.
 7. Using the command ```git add .``` the readme file will be ready to be taken a screenshot of by git
 8. To double check if its ready use the command ```git status``` and if the readme file is in green , you are ready to go on and commit.
 9. Now in order to commit you will use this command ```git commit -m ""``` in between the quotation belongs a small note of what you are commiting. It should be short and simple.
 

---
## Rolling Back Changes
+ To undo any edits you use ```git checkout <file name>``` which discards all changes since last commit. 
+ To undo adding to the stage you use the command ```git reset <file name>``` which unstages the file.
+ In case you want to revert back to a certain commit you have made, you will need to ```git log``` , find the commit you want to revert to and copy the long commit ID, then in your command line use ``` git revert ``` then paste the commit ID.

---
## Error Handling
+ If you initialize git in the wrong directory you will need to ```cd``` into the directory and then use the ```rm -rf``` command which forcefully removes files but after it you will type "git" so it should look like this ```rm -rf git```.