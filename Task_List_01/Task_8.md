## **Task 8: Handling Merge Conflicts**
**1. Create two branches:**  
```bash
git branch branch-A
=> Creates a branch named branch-A.

git branch branch-B
=> Creates a branch named branch-B.
```

**2.Modify the same line in `README.md` in both branches.**  

**=>Changes are made to the same line in README.md on branch-A and branch-B, creating a potential conflict when merging.**


**3.Merge `branch-A` into `main`:**  
```bash
git checkout main
=>Switches to the main branch.

git merge branch-A
=> Integrates changes from branch-A into main.

```
**4.Attempt to merge `branch-B` into `main` (this will cause a conflict):**  
```bash
git merge branch-B
=>This merge attempt detects conflicts in README.md because the same line was modified differently in branch-A and branch-B.

```
**5.Resolve the conflict manually in `README.md`, then:**  
```bash
=> Resolve conflict manually: Open README.md, edit the conflicting sections to keep the desired changes, and save the file.

git add README.md
=> Stage the resolved README.md file.

git commit -m...
=>Commits the resolved conflict with a message describing the resolution.
```
