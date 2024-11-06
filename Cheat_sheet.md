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

...

I'm getting in trouble
