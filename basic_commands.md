# basic_git_commands

Basic Commands I am using 
- git log (to check what has been updated)
- git pull (to pull latest versuib from tracjed repo and override my local before starting work)
- git status (check local repo changes)
- git add 'file name'(add the file to staging - or add file for tracking)
- git commit -m "message here" (add an message at every commit)
- git push (push changes to the remore master)  
- git push origin master (you can push to branches as well)
- git remote show origin (To know where you current local file is tracking to which remore branch)

- git diff  (this "-" minus means what is in the repository "+" means what's added - little dif from unix)

git diff checks 
a (remote repo file) 
b (local file)

--- a/basic_commands.md
+++ b/basic_commands.md


- # git diff --staged 

Once you "git add <file>"
The file will be in the the staged environemnt

If you do git diff --staged
you are comparing 
a) Remote repo file
b) local staged file

This check  only in the staged v.s repo. So repo is - minus, staged is + plus  ) 



- # Reset
 git reset --hard <commit-hash>
 git push -f origin master

 Hard reset revert local
 you have to "force" push so that the remote master reads your local Head.
 git push is not ENOUGH - git will say conflicts
