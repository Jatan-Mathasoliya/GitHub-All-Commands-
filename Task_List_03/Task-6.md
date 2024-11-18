## **Task 6: Customize Log Outputs**

**1. View logs with a graphical representation:**

   ```bash
   git log --oneline --graph --decorate
   ```
   **1. --oneline**

Displays each commit on a single line, including:
The shortened commit hash (7 characters).
The commit message.  
Example:
```
a1b2c3d Initial commit
d4e5f6g Add user authentication feature
```  
**2.--graph**

Adds an ASCII graph to the log output to visually represent the commit structure.
Useful for seeing how branches diverge and merge.  
Example:
```
* a1b2c3d Initial commit
| * d4e5f6g Add user authentication feature
|/
* g7h8i9j Fix homepage bug
```
**3.--decorate**

Annotates the commits with references to branches, tags, and HEAD.
Makes it easy to see which commit corresponds to a branch or tag.  
Example:
```
* a1b2c3d (HEAD -> main, origin/main) Initial commit
* d4e5f6g (feature/login) Add user authentication feature
```

**2. Filter logs for a specific file:**

   ```bash
   git log README.md
   ```
=>The command git log README.md allows you to filter the commit history to display only those commits that involve changes to a specific file, in this case, README.md. This is extremely useful when you want to trace the history or evolution of a single file in your repository.

=> When you run git log with a filename, Git:

Lists all commits in reverse chronological order (most recent first) that affected the specified file.  

Includes changes where the file was:  

Created.  
Modified.  
Deleted.  
Renamed (if Git detected a rename).