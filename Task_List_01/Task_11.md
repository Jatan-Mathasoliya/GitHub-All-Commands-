## **Task 11: Rewriting History with Interactive Rebase**
**1. Create multiple commits:**  
```bash
echo "Commit 1" > file1.txt && git add file1.txt && git commit -m "Commit 1"
echo "Commit 2" > file2.txt && git add file2.txt && git commit -m "Commit 2"
echo "Commit 3" > file3.txt && git add file3.txt && git commit -m "Commit 3" 

=> echo "Commit 1" > file1.txt:
 This command creates or overwrites the file file1.txt with  the text "Commit 1".

=> git add file1.txt:
 This stages the changes in file1.txt, preparing them for commit.

=> git commit -m "Commit 1":
 This commits the staged changes with the message "Commit 1".
```
**The same sequence is repeated for file2.txt and file3.txt, each creating new commits (Commit 2 and Commit 3) in your Git history.**



**2. Squash commits into one:**  
```bash
git rebase -i HEAD~3
=>The git rebase -i HEAD~3 command starts an interactive rebase that affects the last three commits in your current branch (HEAD~3 refers to the last 3 commits, starting from the most recent).
```
After you run this command, Git opens an editor with a list of the last 3 commits, similar to this:

pick <commit-hash-1> Commit 1  
pick <commit-hash-2> Commit 2  
pick <commit-hash-3> Commit 3  
In the editor, you can replace pick with different actions:

Example: Replace `pick` with `squash` for the second and third commits.

**To squash commits, change the word pick on the second and third lines to squash or s:**

pick <commit-hash-1> Commit 1  
squash <commit-hash-2> Commit 2  
squash <commit-hash-3> Commit 3  

**pick:** This keeps the first commit as it is.  

**squash:** This combines the second and third commits into the first one, creating a single commit with the changes from all three.