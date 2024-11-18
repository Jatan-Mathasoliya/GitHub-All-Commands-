## **Task 1: Create a Local Git Repository**

**1. Create a new project folder:**  
   ```bash
   mkdir MyProject
   => This command creates a new folder named "MyProject".

   cd MyProject
   => This command is used to navigates into the created folder.
   ```
**2. Initialize it as a Git repository:**  
   ```bash
   git init
   => This command initializes the current directory(Working Folder) as a Git repository.
   ```

**3. Verify the repository status:**  
   ```bash
   git status
   => This command displays the status of the repository, showing any untracked files.
   ```
### **1. Key Information Provided by git status Current Branch**
**It tells you the branch you're on. For example:**
```
On branch main
```
**Ahead/Behind Information**  
If your branch has commits not yet pushed to or pulled from the remote, it will display:
```
Your branch is ahead of 'origin/main' by 2 commits.
```
**Staged Changes**
Files that are staged (added with git add) and ready to be committed:
```
Changes to be committed:
(use "git restore --staged <file>..." to unstage)
    modified:   file1.txt
    new file:   file2.txt
```

**Unstaged Changes**  
Files that have been modified but not yet staged for commit:
```
Changes not staged for commit:
(use "git add <file>..." to update what will be committed)
(use "git restore <file>..." to discard changes in working directory)
    modified:   file3.txt
```
**Untracked Files**  
Files in the working directory that are not tracked by Git (haven't been staged or committed):
```
Untracked files:
(use "git add <file>..." to include in what will be committed)
    file4.txt
```
**Nothing to Commit**
If everything is committed and synced, Git will show:
```
nothing to commit, working tree clean
```

   - **Example Output**:  
     ```
     On branch main
     No commits yet
     nothing to commit (create/copy files and use "git add" to track)
     ```