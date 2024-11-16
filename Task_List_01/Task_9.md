## **Task 9: Renaming and Deleting Branches**

**1. Rename a branch:**
```bash
git branch -m old-branch-name new-branch-name
=> git branch -m: Renames a branch.
   old-branch-name: The current name of the branch.
   new-branch-name: The new name you want for the branch.
   ```
**2. Delete a branch:**  
```bash
git branch -d feature-login
=> git branch -d: Deletes the branch named feature-login.

Note: The -d option prevents deletion if the branch has unmerged changes to avoid data loss. Use -D to force deletion.
```
