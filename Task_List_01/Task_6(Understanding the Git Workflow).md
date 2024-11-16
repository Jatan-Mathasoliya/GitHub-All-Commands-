## **Task 6: Understanding the Git Workflow** 
#### **1. Make changes to a file in the **working directory**:**  
```bash
echo "Workflow example" > workflow.md
ANS:- Creates a file workflow.md in the working directory and addthe text "Workflow example" to it.
```
#### **2. Stage the file:**  
```bash
git add workflow.md
ANS:- Moves workflow.md to the staging area, preparing it for the next commit.
```
#### **3. Commit the file to the **repository**:** 
```bash
git commit -m "Added workflow example"
ANS:- Saves the staged changes to the repository with a message ("Added workflow example") describing the commit.