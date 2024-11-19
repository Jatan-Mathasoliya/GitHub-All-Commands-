# **Part 1: Understanding and Using `git stash`**

### **Task 1: Save Changes Temporarily with `git stash`**

**1. Make changes to a file without committing:**  
   ```bash
   echo "Temporary changes" >> temp-file.txt
   => This command is used to make file.
   ```
**2. View the status of changes:**  
   ```bash
   git status
   ```
   - **Output**:  
     ```
     Changes not staged for commit:
       modified:   temp-file.txt
     ```

**3. Stash the changes:**  
   ```bash
   git stash
   ```
   - **Explanation**: This command saves changes to a stash and restores the working directory to the last commit state.

**4. View the stashed changes:**  
   ```bash
   git stash list
   ```
   - **Output**:  
     ```
     stash@{0}: WIP on main: 27e5f23 Added temporary changes
     ```

## **Complete Explaination About ***git stash*****

git stash is a Git command used to temporarily save changes in your working directory without committing them. It allows you to "stash away" changes, switch branches or work on something else, and then return to your changes later.

Here’s a detailed explanation of how it works and its usage.

**What Happens When You Run git stash?**  

Uncommitted changes (both staged and unstaged) in your working directory are saved into a temporary storage called a "stash stack."  

The working directory is reverted to the last committed state, making it clean.  

You can later reapply the stashed changes to your working directory.  

**Basic Command**
```
git stash
```

**Effect:**

Stashes all changes (both staged and unstaged) and leaves you with a clean working directory.

### **How to Use git stash**

**1. Stashing Changes**

**Command:**
```
git stash
```

**What it does:**

Saves your current changes (staged and unstaged) and resets the working directory.

**Example:**

Suppose you’ve modified file1.txt and file2.txt but haven’t committed them. Running git stash will:
- Save these changes in the stash.
- Revert file1.txt and file2.txt to the last committed state.

**2. Listing Stashes**

**Command:**
```
git stash list
```

**What it does:**

Displays all stashes in a list with an identifier.

**Example Output:**
```
stash@{0}: WIP on main: a1b2c3d Add login feature
stash@{1}: WIP on main: d4e5f6g Update README
```

**3. Applying a Stash**

**Command:**
```
git stash apply
```
**What it does:**
Reapplies the latest stash (stash@{0}) to your working directory without removing it from the stash stack.

**4. Popping a Stash**

**Command:**
```
git stash pop
```

**What it does:**

Reapplies the latest stash and removes it from the stash stack.
**5. Dropping a Stash**
**Command:**
```
git stash drop stash@{0}
```
**What it does:**
Deletes a specific stash (stash@{0}) from the stack.
**6. Clearing All Stashes**
**Command:**
```
git stash clear
```
**What it does:**
Removes all stashes from the stack.