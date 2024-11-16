## **Task 12: Cherry-Picking Commits**
**1. Create a new branch:**  
   ```bash
   git checkout -b cherry-pick-example
   => git checkout -b <branch-name>: This command is used to create a new branch and switch to it in one step.

-b: This option tells Git to create a new branch.

cherry-pick-example: This is the name of the new branch that you are creating. You can replace this with any branch name you prefer.
   ```
**2. Cherry-pick a specific commit from another branch:**  
   ```bash
   git cherry-pick <commit-hash>
   => git cherry-pick <commit-hash>: This command is used to apply the changes from a specific commit (identified by its commit hash) to the current branch.
   
<commit-hash>: This is the unique identifier (hash) of the commit you want to cherry-pick. You can find the commit hash by running git log or git log --oneline in the branch where the commit exists.        
   ```
