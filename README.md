# GitHub Tutorial

_by Jonathan Cutler_

---
## Git vs. GitHub
If Git is your camera, GitHub is your camera roll. Git is a tool you can use while you code; it's a system to help with version control. GitHub is the website linked to the system to help with visualizing what you do.  
But enough about Git & GitHub. Let's talk how to start using 'em.  

---
## Initial Setup
**First things First, get a GitHub account if you don't have one already. after that, continue onwards.**
You'll be working on `` ide.cs50.io ``

do **NOT** copy paste! It may commit things you don't want to have actually put in.
1. Login with your GitHub account.
2. Enter `` git config --global user.email "______@____.___"``  *(your email)*
3. Enter `` git config -- global user.name "____ ____"`` *(your name)*
4. Enter `` ssh-keygen -t rsa -b 4096 -C "______@____.___"``  *(same email)* and press ``enter`` until you see something like this:  
``[insert snapshot]``
5. Enter `` eval "$(ssh-agent -s)"``
6. Enter `` ls -al ~/.ssh``
7. Enter `` cat ~/.ssh/id_rsa.pub`` and copy ***all*** results  (starting with ssh-rsa and ending with your email)  
8. In GitHub, make a new SSH key, title it "ide50" and where it says key, paste your results.  
``[insert snapshot]``
9. Back in your ide, enter `` sudo nano ~/.ssh/config``
10. copy/paste the following:  
```
Host github.com
 Hostname ssh.github.com
 Port 443
 ```
11. Hit ctrl + x to exit, and answer yes with y, then hit enter.
12. Enter `` ssh -T git@github.com``
13. Type `` yes`` and hit Enter.  
*you should see a message saying "hi" and "welcome!"*

Ok then, you should be all good for the next part!

---
## Repository Setup



---
## Workflow & Commands



---
## Rolling Back Changes