# **Part 2: Rewriting History with `git rebase`**

## **Task 4: Rebase Commits to a New Base**

**1. Rebase the current branch onto `main`:**  
   ```bash
   git rebase main
   ```
   - **Explanation**: This command applies the commits from your current branch on top of the latest commit from `main`.
   - This Command will rebase your current branch onto the latest commit from the `main` branch.
   - In git rebase , the commits from your current branch are replayed on top of the latest commit from the target branch
   - That's why commit history will be good and clean.
   - And that's why we can use any commit easily.

**2. Resolve any conflicts that may arise during rebase, and continue:**  

   ```bash
   git rebase --continue
   ```
### **explaination:**  

The command git rebase --continue is used during a rebase operation to tell Git to continue applying commits after you've resolved a conflict or made changes during the rebase process.

**When to Use git rebase --continue**  

During a rebase, Git applies each commit from your branch onto the new base one by one. If there are no conflicts, Git handles this automatically. However, if a conflict occurs:

- Git pauses the rebase process.
- It allows you to manually resolve the conflict.
- After resolving, you use git rebase --continue to proceed.

### **How It Works**

**Rebase Starts:**

When you run git rebase, Git begins replaying commits on the new base.

**Conflict Occurs:**

If a conflict is detected, Git stops and displays the files with conflicts:
```
error: could not apply <commit-hash> <commit-message>
CONFLICT (content): Merge conflict in <file-name>
```

**Resolve the Conflict:**

Open the conflicted files, fix the issues, and save.
Stage the resolved files using:
```
git add <file-name>
```
**Continue the Rebase:**
```
git rebase --continue
```

Git will finalize the current commit and proceed with the next commit in the rebase sequence.