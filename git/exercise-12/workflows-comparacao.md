# Five Differences Between Git Flow and Trunk-Based Development

| Criteria             | Git Flow                                                                                | Trunk-Based Development                                                                  |
| -------------------- | --------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| **Complexity**       | More complex, with multiple long-lived branches.                                        | Simpler, with a single main branch and short-lived feature branches (or direct commits). |
| **Deployment Speed** | Slower, since changes usually go through release branches before production.            | Faster, as changes are integrated and deployed frequently.                               |
| **Ideal Team Size**  | Better suited for medium to large teams working on multiple features simultaneously.    | Best for small to medium teams that collaborate closely and release often.               |
| **Branch Strategy**  | Uses long-lived branches such as `main`, `develop`, `feature`, `release`, and `hotfix`. | Primarily uses a single trunk (`main`) with very short-lived feature branches, if any.   |
| **Merge Frequency**  | Merges happen less frequently and are often larger.                                     | Merges happen frequently and are kept small to reduce conflicts.                         |



# For a team of 2 to 3 people working on an MVP for a quick launch, what workflow should be used?

In a team of two to three people working on an MVP that needs to be launched quickly, the workflow I would recommend is **Trunk-Based Development**, as it allows for fast merges into the production code.

