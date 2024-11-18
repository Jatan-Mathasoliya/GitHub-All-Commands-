## **Task 5: View Detailed Commit History**

**1. View full commit logs:**

   ```bash
   git log
   ```
   - **Explanation**:  
   Shows a detailed list of commits with hash, author, date, and message.  
   => This command is useful for understanding the commit history and identifying specific changes.  
   =>This command is used to view full the commit history.

2. View commit history in a compact format:  
   ```bash
   git log --oneline
   => This command provides a simplified and concise version of the commit history for your Git repository. It displays each commit as a single line, making it easier to quickly view the history without extra details.
   ```
   - **Example Output**:  
     ```
     e23d8a7 Added initial version of README.md
     f7b3c62 Initial commit: Added README.md
     ```
     => In this example, e23d8a7 is git hash(7 characters) and after that it's a commit message.

     => so by using this code you direcly see git hash and commited message without any history.
