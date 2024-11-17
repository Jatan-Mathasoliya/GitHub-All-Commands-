## **Task 9: Remote Setup**

**1. Add a remote repository:**

   ```bash
   git remote add origin https://github.com/your-username/repo.git
   ``` 

  **What It Does:**  
  
**origin:** The name assigned to the remote repository. origin is a conventional name, but you can choose another name if desired. 
 
**URL:** The URL of your remote repository (e.g., GitHub link). It can be an HTTPS or SSH URL.  

**Use Case:**
You use this command to connect your local Git repository to a remote repository so you can push and pull changes.


**2. Verify the remote:**  

   ```bash
   git remote -v
   ```
**What It Does:**  
Lists all configured remote repositories for your local repository.
Displays two entries for each remote:  

**Fetch URL:** The URL used to pull updates from the remote.
**Push URL:** The URL used to push changes to the remote.