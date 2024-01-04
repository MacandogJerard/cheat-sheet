Git Command Quick Reference

1. **git clone**
   - **Purpose:** Duplicate a repository from an existing source.
   - **Args:** Repository URL (and, optionally, a directory name).
   - **Example:**
     - `git clone https://github.com/user/repository.git`

2. **git branch**
   - **Purpose:** Create, list, or delete branches.
   - **Args:** `-d` (delete), `-m` (move/rename).
   - **Example:**
     - `git branch feature-branch`   # Create a new branch
     - `git branch -d feature-branch`  # Delete a branch

3. **git reset**
   - **Purpose:** Unstage changes or adjust the HEAD pointer.
   - **Args:** `--soft` (move HEAD only), `--hard` (discard changes).
   - **Example:**
     - `git reset --soft HEAD~1`   # Undo the last commit and retain changes
     - `git reset --hard HEAD~1` # Undo the last commit and discard changes

4. **git stash**
   - **Purpose:** Temporarily store changes not ready for immediate commit.
   - **Args:** `-u` (store untracked files), `pop` (apply and remove latest stash).
   - **Example:**
     - `git stash save "WIP: work in progress"`   # Save changes to stash
     - `git stash pop`    # Apply and remove the latest stash

5. **git bisect**
   - **Purpose:** Conduct a binary search to locate the commit introducing a bug.
   - **Args:** start (begin bisecting), good (mark a commit as good), bad (mark a commit as bad).
   - **Example:**
     - `git bisect start`
     - `git bisect good v2.0`
     - `git bisect bad v2.5`
