\# Branching Policy



\## Default Branch



\- `main` is the default integration branch.

\- All completed features must be merged into `main` through a pull request.

\- Direct commits to `main` are not allowed.



\## Branch Types



\### Feature Branches



\- Use feature branches for new enhancements.

\- Create feature branches from `main`.

\- Naming pattern: `feature/<short-feature-name>`

\- Example: `feature/payments-ui`



\### Hotfix Branches



\- Use hotfix branches for urgent production or release fixes.

\- Create hotfix branches from the affected release branch.

\- Naming pattern: `hotfix/<ticket-or-issue-id>`

\- Example: `hotfix/txn-123`



\### Release Branches



\- Release branches are created from `main`.

\- Naming pattern: `release/<major.minor>`

\- Example: `release/1.4`



\## Branch Source Rules



\- Features start from `main`.

\- Hotfixes start from the affected `release/\*` branch.

\- Release branches start from `main`.



\## Branch Protection Expectations



\- Pull request required before merge.

\- At least one reviewer approval required.

\- CI checks must pass before merge.

\- Delete feature and hotfix branches after merge.



\## Agent Instructions



When asked for a branching plan, always return:



\- recommended branch name

\- source branch

\- target branch

\- Git commands

\- pull request target

\- merge strategy

\- backport requirement

