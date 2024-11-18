#### **Task 3: Commit Changes Locally**
1. Create a new file and add content:  
   ```bash
   echo "Welcome to Git" > README.md
   => This command is use to make a file in directory.
   ```
2. Stage the file:  
   ```bash
   git add README.md
   ```
   - **Explanation**: `git add` moves changes to the staging area.

3. Commit the staged file:  
   ```bash
   git commit -m "Initial commit: Added README.md"
   ```
   - **Explanation**: Commits save the current state of the repository with a message describing the change.
