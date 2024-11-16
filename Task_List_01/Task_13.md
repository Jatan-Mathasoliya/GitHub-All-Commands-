
## **Task 13: Tagging Commits**
**1. Tag the current commit:**  
   ```bash
   git tag -a v1.0 -m "Version 1.0 release"

   => git tag: This command creates a tag in Git.

-a: The -a option creates an annotated tag, which includes metadata such as the tagger's name, email, date, and an optional message.
v1.0: This is the name of the tag. You can use any name that makes sense (e.g., v2.0, release-1, beta).

-m "Version 1.0 release": This adds a message to the tag, similar to a commit message. The message explains the purpose of the tag (e.g., marking a release version).
```
**2. Push the tag to the remote repository:**  
   ```bash
   git push origin v1.0

   => git push: This command pushes changes from your local repository to the remote repository.

origin: This specifies the remote repository you are pushing to. By default, origin is the name of the primary remote repository.

v1.0: This specifies the tag you want to push to the remote repository.
   ```