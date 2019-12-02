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



---
## Rolling Back Changes