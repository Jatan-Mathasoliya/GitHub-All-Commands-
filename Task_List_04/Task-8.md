# <ins>**Part 4: Cherry-Picking Commits (```git cherry-pick```) :**</ins>
<br></br>
## **Task 8: Pick a Specific Commit :**

**1. View the commit history to find the commit hash you want to cherry-pick :**
```
git log --oneline
```
+ The command ```git log --oneline``` is used to display a simplified, one-line summary of the commit history in your Git repository.

**2. Cherry-pick a specific commit by its hash :**
```
git cherry-pick <commit-hash>
```
+ The command ```git cherry-pick <commit-hash>``` is used to apply a specific commit from one branch onto your current branch. It allows you to bring in a single commit (identified by its commit hash) from another branch into your current working branch.  

**3. Resolve conflicts if any, then commit the changes :**
```
git add .
git cherry-pick --continue
```
+ The commands git add . and git cherry-pick --continue are used together during the process of resolving conflicts while performing a git cherry-pick.

