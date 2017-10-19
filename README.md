# GitHub Tutorial

_by Shi Wei Zheng_

---
## Git vs. GitHub  
Git is the place where we code and keep the snapshot of the code that we did. Github is the cloud where all the codes are stored. In GitHub, we can see the changes that we made after we committed and pushed the code into GitHub. All the changes can be seen by others and people can give suggestions to the code to make it better. Git is able to run by itself, while GitHub requires git to run.


---
## Initial Setup

#### Creating A GitHub Account
1. Go to [GitHub](www.github.com)
2. Click on the _Sign Up_ on the top right of the site
3. Input your _Username_, _Email Address_, and _Password_
4. Click on _Create an Account_
5. Choose a plan that you desire
6. Click _Continue_
7. Either fill out the tailor experience or click _skip this step_
8. You created a GitHub account

#### Using SSH Key
SSH key allows the user to connect the local remote or cloud9 to GitHub. The key allows GitHub to identify you, just like when you have to input your username and password to log in. GitHub remembers the key so it will know you are the one making the changes.
1. Go to [GitHub](www.github.com)
2. Select _Settings_ on the top right (your profile icon)
3. Select _SSH and GPG keys_ on the sidebar located on the left
4. Click on _New SSH key_
5. Add a title
6. On a new tab, go to [cloud9](c9.io)
7. Sign in to cloud9
8. Click on _Account Settings_ (the gear icon on the top right)
9. Select _SSH Keys_ on the sidebar located on the left
10. Copy the **second** SSH key
11. Go back to the GitHub tab
12. Paste the SSH Key in the _Key_ section
13. Click _Add SSH key_
14. Go to your **IDE** in cloud9
15. Type `ssh -T git@github.com` in your **terminal**
16. It should say something like `Hi <your username>! You've successfully authenticated, but GitHub does not provide shell access._`
17. You finish connecting cloud9 to your private git repository


---
## Repository Setup



---
## Workflow & Commands



---
## Rolling Back Changes