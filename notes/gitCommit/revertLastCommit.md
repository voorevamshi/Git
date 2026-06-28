### To see the last commit made in your repository, run this command in your terminal:
```
git log -1
```

### Variations Based on What You Need:

-   **Show only a clean, one-line summary:** (Shows just the hash and commit message
    
    ```
    git log -1 --oneline
    ```
    
-   **Show the last commit along with the detailed file changes (diff):**
    ```
    git show   
    ```
    (If you only want to see a clean list of the changed file names without the actual lines of code, use `git show --name-only`).
    
-   **Show only the commit message itself:**
      ```
    git log -1 --pretty=%B
    ```
### 2. Revert the last commit

To safely undo the changes from that last commit by creating a new, matching counter-commit, run:
```
git revert HEAD
```

_(`HEAD` is simply Git's pointer for the absolute latest commit on your current branch. This avoids having to copy and paste the commit hash manually)._

Once the revert command opens your terminal text editor, simply save and exit to finalize the undo.
