# Practiced Pull Requests

## Pull Requests

- PR #1: https://github.com/codebysobral/cardapio-digital/pull/1
- PR #2: https://github.com/codebysobral/cardapio-digital/pull/2

## Difference Between "Squash and Merge" and "Create a Merge Commit"

**Squash and merge:** combines all the commits from the pull request into a single commit before adding it to the main branch. This keeps the commit history cleaner and more linear.

**Create a merge commit:** keeps all the original commits from the branch and creates an extra merge commit to combine the changes. This preserves the full development history.

When using `git log --oneline --graph`, **Squash and merge** appears as a single commit, while **Create a merge commit** shows the feature branch and the merge commit.
