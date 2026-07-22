# Weekly summary

**Stash** — temporarily saves uncommitted changes to switch context (`stash`, `pop`, `apply`, `drop`).
**Rebase** — rewrites commits onto another base, creates a linear history. Never on commits already shared.
**Tag** — fixed marker on a commit (releases). Lightweight or annotated; needs `push --tags`.
**Conventional Commits** — `type(scope): description` (feat/fix/docs/...). Ties directly into SemVer.
**Workflows** — Git Flow (structured, multiple branches) vs. Trunk-Based (single, short-lived branches, CI/CD). Depends on context.
**Pull Request** — review before merging: description, comments, approval, status.
**Merge (PR)** — merge commit, squash, or rebase — each produces a different final history.
**Thread tying it together:** short branch → clean commits → rebase → PR → merge → tag (if it's a release).
