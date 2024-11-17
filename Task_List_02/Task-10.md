## **Task 10: Push and Pull**

**1. Push changes to the remote repository:**  
   ```bash
   git push -u origin main
   ```
**Command Breakdown:**  
**git push:** Pushes the changes from your local branch to the corresponding branch on the remote repository.  

**-u:** Sets the upstream branch for the current branch. This simplifies future pushes and pulls, allowing you to run git push or git pull without specifying the remote or branch.  

**origin:** The name of the remote repository. (origin is the default name for the remote added when you run git remote add origin <url>.)
main: The branch on the remote repository where the changes will be pushed.  

**2. Pull changes from the remote:**  
   ```bash
   git pull origin main
   ```
**Command Breakdown:**

**git pull:** Fetches changes from the remote repository and merges them into the current branch.  

**origin:** The name of the remote repository.  

**main:** The branch from which changes are fetched. 

**What It Does:**
Downloads new changes from the remote main branch.
Merges those changes into your local main branch.