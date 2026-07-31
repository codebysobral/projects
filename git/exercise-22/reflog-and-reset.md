# reflog-e-reset.md

# Git Reset Comparison

| Reset Type | Commit History | Staging Area | Working Directory | Typical Use |
|------------|----------------|--------------|-------------------|-------------|
| `git reset --soft` | Moves `HEAD` to the target commit | Keeps all changes staged | Keeps all files unchanged | Rewrite commits while preserving staged changes. |
| `git reset --mixed` *(default)* | Moves `HEAD` to the target commit | Clears the staging area | Keeps all file modifications | Unstage changes without losing your work. |
| `git reset --hard` | Moves `HEAD` to the target commit | Clears the staging area | Discards all local changes | Permanently remove commits and uncommitted changes. |

## Commit Recovery with Reflog

I created several commits and then used `git reset --hard HEAD~1` to remove the latest commit from the branch history. Although the commit was no longer visible in the log, it was still recorded in the reflog. I ran `git reflog` to find the commit hash of the removed commit. After locating it, I restored the commit with `git reset --hard <commit-hash>`. This demonstrated that reflog can recover commits that are no longer referenced by the current branch. The commands used were `git reset --hard HEAD~1`, `git reflog`, and `git reset --hard <commit-hash>`.
