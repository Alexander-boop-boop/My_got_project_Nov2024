# Dictionary and concepts

- Git: timeline    
- Github: backup of your timeline

# Conceptual Areas

1. Dev. Area: the path to the topmost folder where you initialized your gift

2. Local Repository: the timeline

3. Staging Area: A space to prepare for a snapshot that will go in my timeline. When making unrelated changes and dont want to gommit them together you can use the staging area to commit one-by-one. 

4. Remote area: back up of the timeline, in this case in GitHub (could also be Gitlab)

# Why use the staging area

It gives a space to organize your changes in time. Because of this you can think logically before making a comit. 

# What if you forget -m in git commit?

it opens a text editor and makes you create a message! too important to escape!

# Complex problem 1: bad commit

-> git log -> search the commit where it went wrong, get the number for this one

-> git revert 1277cfccdf69e8

you can also revert the revert

# Differences git clone and git pull

Clone downloads everything when you have nothing

git pull looks at what changes are made in your online directory but not locally, and updates your local repository

# Conflicts

When you both push a change in the same document, the last one to push gets a conflict

# Alternative histories

Branches = alternative history of commits. They have a specific descriptive name. A branch is indipendent in itself. It is connected with the main branch in one point. 

You can push things at one time, without worrying the other will push before you. 

The most recent commit is always named head. I

Git checkout command makes you travel between branches. Do not mess up the path.



Git checkout: switch branches, git show displays info about git object 
