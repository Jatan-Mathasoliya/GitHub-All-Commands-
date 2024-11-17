## **Task 20: Aliases and Shortcuts**

### **1. Create an alias for frequently used commands:**

   ```bash
   git config --global alias.st status
   git config --global alias.cm commit
   ```

   => **git config --global:** Modifies your global Git configuration, applying the alias to all repositories on your system.  

**alias.st:** Creates an alias named st for the git status command.  

**alias.cm:** Creates an alias named cm for the git commit command.


### **2. Use the alias:**  
   ```bash
   git st
   => Executes git status, which shows the current status of your working directory (staged, unstaged, and untracked files).
   => This command is a shorthand of git status

   git cm -m "Message"
   => This command is a shorthand of git commit -m "Message
   ```

 ### **Why Use Git Aliases?**

**Efficiency:** Shortens long commands.  

**Example:** Replace git log --oneline --graph --all with git lg.
Customization: Tailor Git commands to your workflow.  

**Readability:** Makes frequently used complex commands easier to remember.