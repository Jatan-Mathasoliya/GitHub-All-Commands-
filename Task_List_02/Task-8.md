## **Task 8: Handling Merge Conflicts**

### **1. Create two conflicting branches and resolve a conflict manually:**  

   ### **Step 1: Create Two Conflicting Branches Suppose you have a repository with a file example.txt.**

**Create and Switch to a New Branch:**
```
git checkout -b branch1  
```

Creates a branch named branch1 and switches to it.

**Modify and Commit in branch1:**
```
echo "Change from branch1" >> example.txt
git add example.txt
git commit -m "Update example.txt in branch1"
```

**Switch Back to main:**
```
git checkout main
```

**Modify and Commit in main:**
```
echo "Change from main" >> example.txt
git add example.txt
git commit -m "Update example.txt in main"
```

### **Step 2: Merge branch1 into main**
```
git merge branch1
```
**What Happens:**  
Git attempts to merge changes from branch1 into main.  
Since both branches modified example.txt, Git detects a conflict.

### **Step 3: Resolving the Merge Conflict**

**1.Check Conflict in Terminal: Git informs you about the conflicting file(s):**
```
Auto-merging example.txt
CONFLICT (content): Merge conflict in example.txt
Automatic merge failed; fix conflicts and then commit the result.
```

**2.View Conflict in the File: Open example.txt, and you'll see something like this:**
```
<<<<<<< HEAD
Change from main
=======
Change from branch1
>>>>>>> branch1
```
**HEAD: Represents the changes from the current branch (main).**

**branch1: Represents the changes from the merging branch.**

**3.Manually Resolve the Conflict: Edit the file to keep the desired changes. For example:**
```
Change from main
Change from branch1
```

**4.Mark the Conflict as Resolved: Stage the resolved file:**
```
git add example.txt
```
### **Step 4: Commit the Merge**
```
git commit
```
**What It Does:**  

Completes the merge process by committing the resolved conflict.  

The merge conflict is now resolved, and the branch has been successfully merged.

2. Use:  
   ```bash
   git add <resolved-file>
   git commit
   ```
