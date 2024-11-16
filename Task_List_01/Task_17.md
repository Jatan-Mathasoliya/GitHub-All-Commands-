#### **Task 17: Git Ignore**
**1. Create a `.gitignore` file:** 
```bash
echo "node_modules/" > .gitignore

=> echo "node_modules/": This outputs the string node_modules/.

>: This redirects the output of the echo command into a new file named .gitignore. If .gitignore already exists, this overwrites its contents.

.gitignore: This is the name of the file where you define patterns for files or directories that Git should ignore.
```

**2. Add files and ensure ignored files are not staged:**  
   ```bash
   git add .

   => git add .: This stages all changes (new, modified, or deleted files) in the current directory and its subdirectories for the next commit.

However, any files or directories listed in .gitignore will not be staged.
   ```
