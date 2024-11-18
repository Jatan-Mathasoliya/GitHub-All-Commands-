## **Task 4: Write Effective Commit Messages**
**1. Create a detailed commit message:**

   ```bash
   git commit -m "Added initial version of README.md with project overview"
   ```
   - **Explanation**: Commit messages should follow conventions such as starting with a capital letter, being concise, and using the imperative mood.

**2. Commit multiple files with one message:**

   ```bash
   touch file1.txt file2.txt
   git add .
   git commit -m "Added two new files for feature setup"
   ```
- **Explanation**:  
**=> The `touch` command creates new empty files.(This is a shorthand of echo command).**  

    => The `git add .` command stages all changes in the current directory.

    => The `git commit` command commits the staged changes with the specified message