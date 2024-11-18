## **Task 10: Simulate a Merge Conflict**

**1. Modify the same line in a file on two branches:**  
   ```bash
   echo "Main branch content" > conflict.txt
   git add conflict.txt
   git commit -m "Added conflict.txt in main branch"
   ```

**2. Switch to the other branch and make conflicting changes:**  
   ```bash
   git checkout feature-branch
   echo "Feature branch content" > conflict.txt
   git add conflict.txt
   git commit -m "Modified conflict.txt in feature-branch"
   ```

**3. Merge `feature-branch` into `main`:**  
   ```bash
   git checkout main
   git merge feature-branch
   ```

**4. Resolve the conflict by editing the file and choosing the correct version:**  
   - Open `conflict.txt` and decide which changes to keep.
   - Stage the resolved file:  
     ```bash
     git add conflict.txt
     ```
   - Commit the merge:  
     ```bash
     git commit -m "Resolved conflict in conflict.txt"
     ```

**explaination:**
- First make file in main branch and add it to staging area and commit it.
Add some content in that

- Then switch to feature branch and add some content and make same file and commit it.

- Then switch to main branch and merge feature branch into main branch.

- Then resolve the commit :   
You have two options to resolve the conflict either you can choose one of the version or you can write your own version.