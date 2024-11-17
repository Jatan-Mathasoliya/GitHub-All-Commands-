## **Task 19: Cleaning the Repository**
### **1. Remove untracked files:**  
   
```bash
   git clean -f
   ```

**git clean:** The base command for removing untracked files.  

**-f:** Stands for "force." Git requires this flag to confirm that you  
 really want to delete untracked files, as this action is irreversible.  

**When you run this command:**  

Git removes all untracked files from your working directory.  
Files tracked by Git or ignored via .gitignore are unaffected.