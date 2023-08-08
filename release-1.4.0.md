
# Release Notes - All-in-One Snippet Master Extension (Version 1.4.0)

## What's New

### Git Log Beautify
Description: Git log with more visibility. Using `--graph` and `--format`, you can quickly get a summary view of git commits in your project.
Snippet:
```
git log --graph --format=format:'%C(bold blue)%h%C(reset) - %C(bold green)(%ar)%C(reset) %C(white)%an%C(reset)%C(bold yellow)%d%C(reset) %C(dim white)- %s%C(reset)' --all
```

### Git Stat
Description: Using the `--stat` flag, you can see the commit summary along with the files that changed and details on how they changed.
Snippet:
```
git show <commit> --stat
```

### Git Config
Description: Useful Git config commands to set user email, name, and check all configurations.
Snippet:
```
git config --global user.email "email@gmail.com"
git config --global user.name "your username"
git config -l //to check all the config is set or not
```

### Git Status Only Modified
Description: Display git status for only modified files.
Snippet:
```
git ls-files -m //git status only modified files
```

### Git Author Reset Entire Project History
Description: Reset the author for the entire project history.
Snippet:
```
git rebase -r --root --exec 'git commit --amend --no-edit --reset-author'
```

### Git Author Reset Single Commit
Description: Reset the author for a single commit.
Snippet:
```
git commit --amend --no-edit --reset-author
```

### Generate SSH Key
Description: Generate an SSH Key for secure communication with your repository.
Snippet:
```
ssh-keygen -t ed25519 -C 'your_email@example.com'
```

### Show All Branches (Local and Remote)
Description: List all branches, including local and remote branches.
Snippet:
```
git branch --all
```

### Clear Git Cache
Description: Remove the cache in Git (useful for refreshing ignored files).
Snippet:
```
git rm -rf --cached .
```

### Git Rename Branch
Description: Rename a branch in the local Git repository.
Snippet:
```
git branch -m <oldname> <newname>
```

### Git Add Remote Origin
Description: Add a remote origin URL to your Git repository.
Snippet:
```
git remote add origin <url of your repository>
```

### Git Update Remote Origin
Description: Update the remote origin URL for your Git repository.
Snippet:
```
git remote set-url origin <url of your repository>
```

### Preview and Apply Git Patch
Description: Preview and apply a Git patch with various options. See [here](https://git-scm.com/docs/git-apply) for more info.
Snippet:
```
# Display stats of changes in the patch
git apply --stat <patch_file>

# Perform a dry run to detect errors
git apply --check <patch_file>

# Preview patch application with detailed information
git apply --verbose <patch_file> > patch_preview.txt

# Apply the patch and handle whitespace issues
git apply --reject --whitespace=fix <patch_file>

# If necessary, manually apply the patch and create reject files
# git apply <patch_file>
# In case of errors, generate reject files and references for changes not applied
# git apply --reject <patch_file>
```

### Delete GitHub Branch
Description: Delete a branch from GitHub.
Snippet:
```
git push origin --delete <branch_name>
```

### Delete Local Branch
Description: Delete a branch from the local repository.
Snippet:
```
# Delete a local branch that has been fully merged
git branch -d <local_branch>

# Delete a local branch forcefully, including unmerged/unpushed commits
git branch -D <local_branch>
```

### Merge Multiple Commits
Description: Merge multiple commits into a single commit using interactive rebase.
Snippet:
```
# Start an interactive rebase for the last n commits
git rebase -i HEAD~<commit_count>

# In the interactive rebase editor, change 'pick' to 'squash' or 's' for commits you want to merge
# Save and exit the editor
git push origin <branch_name>
```

### List Changed Files Between Commits
Description: List all the changed files between two commits using 'git diff'.
Snippet:
```
git diff --name-only <start-commit>..<end-commit>
```
