\# Merge Strategies



\## Feature Merge Strategy



\- Feature branches must be merged into `main`.

\- Use squash merge for feature branches.

\- Squash merge keeps the main branch history clean.

\- Example: `feature/payments-ui -> main`

\- Merge type: `squash`



\## Hotfix Merge Strategy



\- Hotfix branches must be merged into the affected release branch first.

\- Use regular merge commit for hotfix branches.

\- After merging to the release branch, create a backport or forward-merge pull request to `main`.

\- Example: `hotfix/txn-123 -> release/1.4`

\- Merge type: `merge commit`

\- Then merge: `release/1.4 -> main`



\## Release Merge Strategy



\- Release branches are created from `main`.

\- Stabilization fixes should be merged into the release branch.

\- Final release changes should be merged back into `main`.



\## Conflict Handling



If merge conflict risk is found:



\- identify likely conflicting files

\- recommend syncing the branch with latest source

\- suggest creating a draft pull request early

\- recommend reviewer validation



\## Agent Instructions



When asked for a merge plan, always include:



\- source branch

\- target branch

\- merge type

\- reason for merge type

\- backport or forward-merge steps

\- conflict risk

\- recommended validation checks

