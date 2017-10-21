# GitHub Tutorial

_by Shi Wei Zheng_

---
## Git vs. GitHub  
Git is the place where we code and keep the snapshot of the code that we did. Github is the cloud where all the codes are stored. In GitHub, we can see the changes that we made after we committed and pushed the code into GitHub. All the changes can be seen by others and people can give suggestions to the code to make it better. Git is able to run by itself, while GitHub requires git to run.


---
## Initial Setup

#### Creating A GitHub Account
1. Go to [GitHub](https://github.com/)
2. Click on the _Sign Up_ on the top right of the site
3. Input your _Username_, _Email Address_, and _Password_
4. Click on _Create an Account_
5. Choose a plan that you desire
6. Click _Continue_
7. Either fill out the tailor experience or click _skip this step_
8. You created a GitHub account

#### Using SSH Key
SSH key allows the user to connect the local remote or cloud9 to GitHub. The key allows GitHub to identify you, just like when you have to input your username and password to log in. GitHub remembers the key so it will know you are the one making the changes.

1. Go to [GitHub](https://github.com/)
2. Select _Settings_ on the top right (your profile icon)
3. Select _SSH and GPG keys_ on the sidebar located on the left
4. Click on _New SSH key_
5. Add a title
6. On a new tab, go to [cloud9](https://c9.io/)
7. Sign in to cloud9
8. Click on _Account Settings_ (the gear icon on the top right)
9. Select _SSH Keys_ on the sidebar located on the left
10. Copy the **second** SSH key
11. Go back to the GitHub tab
12. Paste the SSH Key in the _Key_ section
13. Click _Add SSH key_
14. Go to your **IDE** (Integrated Development Environment)in cloud9
15. Type `ssh -T git@github.com` (This make your terminal knwo that it is connected to GitHub) in your **terminal**
16. It should say something like "Hi <your username>! You've successfully authenticated, but GitHub does not provide shell access._"
17. You finish connecting cloud9 to your private git repository!


---
## Repository Setup
A respository is the place where you store codes. You can take the code and bring the code down to your local remote or computer.

1. Go to your **terminal**
2. Make your your are in **workspace**, if not, `cd ~/workspace` (This will bring you to workspace)
3. Make a new directory/folder using `mkdir` and give the folder a name
4. Move into the folder with `cd` and the folder name
5. Use `git init` to initialize the folder to make it able to work as git.
6. Create a new file with `touch README.md` (This will create a file called README.md)
7. Use `c9 README.md` to open the README file in your _cloud9 terminal_
8. Add some texts in the file
9. Save your changes
10. In the terminal, use`git add .` to add all the new changes in the staging area
11. `git status` to check what changes have been staged and what haven't
12. Commit/snapshot the new changes using `git commit -m "your message"` (when committing, you need to add a message to tell you and/or others what that commit does. The message have to be in the present tense. Example: "Create a readme file")
13. We will need a remote repo to push the commit into
14. Go to [GitHub](https://github.com/) and login if not already
15. Click on the _plus icon_ on the top right and select _New repository_
16. Type in the **exact same name for your directory/folder** as the _Repository name_
17. Click _Create repository_ on the bottom
18. Verify your email if asked
19. In quick setup, make sure SSH is selected
20. Copy and paste each line of code under "...or psuh an existing repository from the command line" one at a time into your _c9 terminal_. This first line should be `git remote add origin URL` (The URL is the link to the repository that you just made). This line of code will create a bridge/path connecting your local repository to your remote repository. The second line should be `git push -u origin master`. This will tell the computer to remember where to push to, so we don't have to keep including the URL everytime we push. We just have to put this line of code once and next time we can just type `git push`.
* To check the location of your remote use `git remote -v`
* To remove your remote use `git remote rm origin`
21. You finished setting up your own repository!



---
## Workflow & Commands
When making changes to your work, you should try to send those changes to GitHUb once you think it is a good place to commit. This will save your work virtually in GitHub and you can check what changes were made to the work. You will not lose your work when it is saved in GitHub. your can always get your work back even if your computer stopped, and get a new one. To save your work to GitHUb, follow these steps:
1. After your think your work is ready to be save, type `git add .` in your terminal to add all your changes to the staging area.
2. 


---
## Rolling Back Changes