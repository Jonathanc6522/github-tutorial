# GitHub Tutorial

_by Jonathan Cutler_

---
## Git vs. GitHub
If Git is your camera, GitHub is your camera roll. Git is a tool you can use while you code; it's a system to help with version control. GitHub is the website linked to the system to help with visualizing what you do.  

Essentially, **Git** is your version control. --Doesn't require GitHub.-- **GitHub** is your human way to moniter the versions, while also allowing you to work with others and store code online. --Does require Git.--

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
Ok, now we're starting to get a lil more personal work wise. *I found this easy at first by comparing it to running through files in my own computer (like with video game configs and such)*


Now, get into your ide and GitHub and do the following:  
* **in GitHub**  
-- make new repository  
-- make a title  
-- make sure it's empty; NO README.md files or anything like that  
-- you should see an option to...  
`[insert snapshot]`  
   you'll want to click the copy to clipboard button, that'll be all you have to do on GitHub for now.


* **in your ide**  
-- `mkdir ______` makes a directory with whatever you decide to call it.  
-- `cd _______` takes you from the root terminal (~~) to the directory you entered the name of.  
-- enter `git init` to initialize the directory with git and make it into a repo. You should see `(master)` next to where it tells you where you're working from.
-- then do `touch README.md` this will create a text file that you can edit the content of with a `c9 _____` command.  
-- then do `git add` to stage your changes.  
-- enter `git commit -m "______"` as a commit message. Although not imperative, it's a good habit to commit in the present tense. (`git commit -m "finish repo setup section"`)  
-- remember the last instruction from  **"in GitHub?"** well, now you're going to want to copy past what you did from before.

---
## Workflow & Commands



---
## Rolling Back Changes

`[wip]`

