## **Task 7: Branching and Merging**
#### **1. Create a new branch for a feature:**  
```bash
git branch feature-login
ANS:- Creates a new branch named feature-login.

git checkout feature-login
=> Switches to the feature-login branch.
```
Or use:  
```bash
git checkout -b feature-login
=> Combines the two steps above: creates and switches to the feature-login branch.
```
**2. Add a new file and commit changes:**  
```bash
echo "Login Page" > login.html
=>Creates a file named login.html with the content "Login Page".

git add login.html
=>Stages the new file for the next commit.

git commit -m "Added login page"
=>Saves the staged changes to the repository with a descriptive commit message.

```
**3. Merge the feature branch into `main`:**  
```bash
git checkout main
=> Switches back to the main branch.

git merge feature-login
=> Integrates the changes from the feature-login branch into the main branch.
```
