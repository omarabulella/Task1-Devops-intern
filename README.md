# Task1-Devops-intern!
At Task 1 Step 10: Debugging
*I deleted case 1 commit from development branch instead of case 2 commit*

Task2:
1-What is git stash and when is it useful?
git stash is a command that allows you to temporarily save changes that you haven’t committed yet. It helps you switch branches without losing the changes you’re working on.

2-When is it useful?
When you need to switch to another branch to fix a bug, but you have uncommitted changes.
When you want to temporarily put aside your changes without committing them.

3-we can use git stash command to Temporarily Save Uncommitted Changes 
This will save all the changes (tracked files) in our working directory and return it to the state of the last commit

4-List all stashed changes: we can use git stash list command to view the list of all stashed changes

5-Restore Stashed Changes Using the Appropriate Command we can use git stash apply stash@{0}
This applies the stashed changes to our working directory, but the stash still exists in the list
and we can use git stash pop command but this will restore and remove the changes from the stash list

6-To clear all stashes in list we can use this command git stash clear
and to clear specific stash we can use this command git stash drop statsh@{0}

7-What happens when you use git stash pop vs git stash apply?
git stash pop applies the changes and then removes the stash from the list.
git stash apply applies the changes but keeps the stash in the list for future use

8-What is the purpose of git stash save "message"?
Adding a message helps us describe the stashed changes so we can easily identify them later

9-How can you stash changes for specific files instead of the entire working directory?
To stash changes for specific files we can use this command git stash push f1 f2

