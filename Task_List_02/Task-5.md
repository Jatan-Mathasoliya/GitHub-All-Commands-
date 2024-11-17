## **Task 5: Undoing Changes**
**1. Unstage a staged file:**  
   ```bash
   git reset file1.txt

   => What It Does:
Moves the file (file1.txt) from the staging area back to the working directory.

Any changes in the file remain intact, but they are no longer staged for the next commit.

Use Case:
If you accidentally staged a file with git add, and you don’t want it to be included in the next commit, you can "unstage" it.
   ```

**2. Discard uncommitted changes:**
   ```bash
   git checkout -- file1.txt
   => What It Does:
Restores the file (file1.txt) in the working directory to match the latest committed version (HEAD).
Any uncommitted changes in the file are discarded and cannot be recovered.

⚠️ Warning: Use this command carefully. Once you discard changes, they are lost unless you have a backup or saved them elsewhere.

Use Case:
If you make unwanted changes to a file and want to revert it to the state of the last commit.
   ```
