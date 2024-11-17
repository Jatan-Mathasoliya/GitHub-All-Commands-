## **Task 12: Stashing Changes**

**1. Save uncommitted changes:**  
   ```bash
   git stash

   => What it does:
-Saves all modified tracked files and staged changes to a "stash" (a temporary storage) and reverts the working directory to the last committed state.

-This action temporarily removes changes but keeps them safe for later use.
   ```
**2. Apply stashed changes:**  
   ```bash
   git stash apply
   => Reapplies the most recent stash (stash@{0} by default) to the working directory.

The stash remains in the stash list after applying.
   ```
**3. Drop the stash:**  
   ```bash
   git stash drop
   => Each stash in Git is identified by an index, like stash@{0}, stash@{1}, and so on.

The git stash drop command removes the specified stash from the list of stashes but does not affect your working directory or repository.

OR

git stash pop

=> Reapplies the most recent stash and then removes it from the stash list.
   ```
