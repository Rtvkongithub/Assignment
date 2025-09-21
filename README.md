# Assignment

# SSH GitHub Demo

## Difference between `git pull` and `git fetch`
- **git fetch**: Downloads changes from remote but does **not merge** into local branch.  
- **git pull**: Downloads changes and **merges** into your current branch.  

Example:  
- `git fetch` = "Check what’s new but don’t touch my work yet."  
- `git pull` = "Bring the new stuff and combine it with mine."

---

## Resolving a Git Merge Conflict
**Scenario:**  
- Branch `feature-A` changes line 1 in `file.txt` to "Hello A".  
- Branch `feature-B` changes line 1 in `file.txt` to "Hello B".  

When merging, Git can’t decide which line to keep → **conflict**.

**Steps to resolve:**  
1. Open conflicted file. You’ll see:
   ```txt
   <<<<<<< HEAD
   Hello A
   =======
   Hello B
   >>>>>>> feature-B
