# Cherry-pick, Revert, and Reset

| Command           | What it does                                                                                                                              | When to use                                                                     | Risk level      |
| ----------------- | ----------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------- | --------------- |
| `git cherry-pick` | Copies one or more specific commits from another branch and applies them to the current branch.                                           | Reuse a particular fix or feature without merging the entire branch.            | **Low**         |
| `git revert`      | Creates a new commit that undoes the changes introduced by a previous commit.                                                             | Safely undo changes in shared branches while preserving history.                | **Low**         |
| `git reset`       | Moves the current branch pointer to a different commit. Depending on the mode, it may also modify the staging area and working directory. | Rewrite local history before sharing commits or discard unwanted local changes. | **Medium–High** |
