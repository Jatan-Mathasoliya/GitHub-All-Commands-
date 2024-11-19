## Task 21: Sync Your Fork with the Original Repository :
**1. Add the original repository as a remote source :**
```
git remote add upstream https://github.com/original-owner/repo.g
```
+ This sets up a connection to the original repository (referred to as upstream). You would typically use this in a forked repository to pull updates from the original repo.  

**2. Fetch changes from the original repository :**
```
git fetch upstream
```
+ **Fetch Updates** :
It downloads all the changes (commits, branches, and tags) from the upstream remote repository.

+ **No Merge** :
The changes are not applied to your working directory or current branch. They are stored in your local repository under the upstream remote references.  

**3. Merge changes from the original repository into your local branch:**
```
git checkout main
git merge upstream/main
```
+ The commands ```git checkout main``` and ```git merge upstream/main``` update your local ```main``` branch with the latest changes from the original repository (```upstream```). First, ```git checkout main``` switches to your ```main``` branch. Then, ```git merge upstream/main``` merges the latest updates from ```upstream/main``` (fetched earlier using ```git fetch upstream```) into your branch. This process ensures your local branch is synchronized with the original repository, incorporating any new changes or updates. If there are conflicts, you'll need to resolve them before completing the merge.   

**4. Push the changes to your fork :**
```
git push origin main
```
+ The command ```git push origin main``` uploads the changes from your local ```main``` branch to the remote repository named ```origin```.
