
## **Task 14: Working with Remote Repositories**
**1. Add a remote repository:**  
   ```bash
   git remote add origin <repository-url>

   => git remote: This command is used to manage remote connections in your Git repository.

add: This subcommand adds a new remote connection.

origin: This is the name you assign to the remote repository. It's a convention to name the primary remote repository origin, but you can choose a different name if needed.

<repository-url>: This is the URL of the remote repository (e.g., https://github.com/username/repo.git or git@github.com:username/repo.git).
   ```
**2. Push your changes to the remote repository:**  
   ```bash
git push origin main

=> git push: This command uploads commits from your localrepository to a branch in the remote repository.

origin: This specifies the remote repository to which you want to push your changes. It refers to the remote you added in the previous step.

main: This specifies the branch you want to push. Replace main with the name of your branch if you're pushing a different branch.
   ```