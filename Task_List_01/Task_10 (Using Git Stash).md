## **Task 10: Using Git Stash**
**1. Make changes to a file but don’t commit:**  
   ```bash
   echo "Temporary work" >> temp.md
   =>This command appends the text "Temporary work" to the file temp.md. The >> operator ensures that the text is added to the file without overwriting its contents.
   ```
**2. Stash the changes:**  
   ```bash
   git stash
   => The git stash command temporarily saves (or "stashes") any changes in your working directory that haven’t been committed. This is useful if you need to switch to another task or branch but don't want to commit your changes yet. It clears the changes from your working directory, allowing you to work on something else.

   ```
**3. View stashed changes:**  
   ```bash
   git stash list
   => This command lists all the stashes you have saved. Each stash entry is shown with a name like stash@{0}, stash@{1}, etc., indicating the order in which they were stashed.
   ```
**4. Apply the stashed changes:**  
   ```bash
   git stash apply
   => This command restores the most recent stashed changes to your working directory. It re-applies the changes you saved using git stash without removing them from the stash list. This allows you to apply the changes again later if needed.
   ```
**5. Drop the stash after applying:**  
   ```bash
   git stash drop
   => The git stash drop command removes the specified stash from the list of stashes. After you've applied a stash and no longer need it, you can use this command to clean up. If you don’t specify a stash, it will drop the most recent one (stash@{0}).
   ```

### **Summary of Workflow:**

**git stash :** saves your changes without committing them.  

**git stash list :** lists all the stashes you have saved.  

**git stash apply :** restores the most recent stashed changes to your working directory.  
**or**  
restores the changes you saved with git stash.  

**git stash drop :** removes a stash after you’ve applied it.  
**or**  
removes the specified stash from the list of stashes.
