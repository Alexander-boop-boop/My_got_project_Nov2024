# Commands list

- git init: initialize a new repository. We only initialize it once. 

- git add: adding in the staging area to monitor and keep track off (any changes, not only new files)

- git commit -m "Meaningful Msg": saving a point in the timeline with a message that describes (Why, How, Effects, Limitations)

- git config --global --list : list all your configs

- git config --global user.name "My name": To have your name in the config

- git config --global user.email "my_email@vib.be": to have my email in the config

- git mv old.file.text new.file.txt: when changing a name so git knows it is the same file

- git status: checks which files are in developing or staging area, or are untracked

- What happens if i gorget the -m in the commit

# The staging area

is for making a space to organise things in time before making a commit

# How to see history of timeline

- git log: without arguments it lists the commits made in the repository, in reverse chronological order. The first thing is the commit hash, unique identifyer for each commit. Second line: author: see who commited it. It will also tell you the message, date, & time. 

- git log -n: will limit the number of listed commits. -3 --> check last 3. 

- git log --abbrev-commit

- git log --oneline: each commit on a single line with the abbreviated commit hash and the commit message.

- git log -p: shows the changes in each commit

- git log --pretty=format:"%h - %an, %ar : %s": commit hash, author name, relative date, and the commit message.

- 

# How to check for differences in versions of timelines

- git diff HEAD <ID> 
  
  - Met comit headers uit git log
  
  - Met laatste 2: git head, head1 --> two most recent comments, 

- git diff HEAD ⁓2
  
  - git diff HEAD⁓2: compares the last 2
  
  - git diff 

- git show: prints all files info, describes each line as considered in the moment. 

# How do we connect to a remote repository

* git remote add <name> <ssh>
* git remote add origin ssh-adress: establish the bridge between the local and the remote repository

# A bridge works both ways

* git push: transfers everything that has been commited (what is in the gitignore has not been commited). The first time you need git push -u origin main. You can just use git push further down the line. 

* git pull: transfers any updates commited remotely

# Routine local 2 remote

...

* git status 

* git add

* git commig -m "meaningdul msg

* git push 

# Problem solving commands

* git revert 
  
  * If you gave a bad commit, which you dont want
  
  * git log --> search number of commit you want to reverse --> put this number in git revert 

* git clone
  
  * When you removed your local repository
  
  * go to github and get the ssh you need
  
  * then put git clone ssh
  
  * gitignore wont be there, it was ignored. git remote is already done. When you did everything 

* git rebase, also exists, but makes more drastical changes, we dont really talk about it during the course
  
  # Alternative histories
- git branch <name>
  
  - git branch parallell_timeline
  - git branch -a --> gives overview of timelines

- git checkout <branch_name>
  
  - Do not mess with the past
  - git checkout parallell timeline --> switches to here
  - Before you move branches, close the files you are working in

- First time you push in a different timeline: --set-upstream origin parallell_timeline

 git push --set-upstream origin parallell_timeline

* git branch <name>
  
  * git branch parallell_timeline

* git checkout parallell_timeline

* git log --oneline --decorate --graph -a --> get a graphic overview 



# Tagging: naming a commit

* git tag -> gives all names you have

* git tag <name>
  
  * tags the head; the last commit

* git tag <name> <commitID> 

* git tag cb0a38 ( komt van git log) c war_zone

* git push --tags 
  
  * Pushes specifically the tags. Normal git push might not work

* git tag -d 
  
  * Deleting a tag
    
    git tag -d war_zone
    
    
