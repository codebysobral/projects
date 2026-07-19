# 8 Commit types with examples

## feat: for new feature

feat(login): add new login area


## fix: for bug fixes

fix(login): prevent crash when password is empty


## docs: for documentation changes

docs(readme): add installation instructions


## style: for code formatting changes (without changing logic)

style(button): format component with prettier


## refactor: for code improvements without changing behavior

refactor(tasks): extract task validation into helper function


## test: for adding or updating tests

test(tasks): add unit tests for task creation


## chore: for maintenance tasks and configuration changes

chore(deps): update project dependencies


## perf: for performance improvements

perf(search): optimize task filtering


## build: for build system or external dependency changes

build(webpack): upgrade webpack version


## ci: for continuous integration changes

ci(github-actions): add automated test workflow


# The relationship between SemVer and Conventional Commit:

* fix -> bug fix (PATCH)

* feat -> new feature (MINOR)

* BREAKING CHANGE or ! -> Changes that break 
compatibility increase (MAJOR)
