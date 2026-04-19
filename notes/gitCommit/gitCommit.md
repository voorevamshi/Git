### 1. Unstage the files
Run this command to tell Git to stop tracking the `.idea` folder without deleting the actual files from your computer:

git rm -r --cached .idea/

### 2. Update your `.gitignore`
To prevent Git from accidentally staging these files again in the future, add `.idea` to your ignore file:

echo ".idea/" >> .gitignore
echo "target/" >> .gitignore

### 3.  What if the `target` folder is already tracked?
If you previously committed the `target` folder to Git, simply adding it to `.gitignore` won't remove it from the repository. You must manually "untrack" it:

Remove the target folder from the Git index (but keep it on your disk)

git rm -r --cached target/

### 4. Commit the changes
Now you can safely commit your project files while the `.idea` ,  `target`  folder stays strictly local to your machine:

git add .gitignore
git commit -m "Remove .idea from tracking and update gitignore"


### Maven build output
target/

### IntelliJ IDEA files
.idea/
*.iml
out/

### Log files
*.log

### OS generated files
.DS_Store
Thumbs.db
