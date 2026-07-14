\# Pull Request Rules



\## General PR Rules



\- Every branch must be merged through a pull request.

\- Pull request title must clearly describe the change.

\- Pull request body must include summary, validation, and risk.

\- At least one reviewer approval is required.

\- CI checks must pass before merge.



\## PR Title Format



\### Feature PR



Format: `Feature: <short feature description>`



Example: `Feature: Add payments UI`



\### Hotfix PR



Format: `Hotfix: <ticket id> - <short fix description>`



Example: `Hotfix: TXN-123 - Fix transaction timeout`



\## PR Body Template



Summary:



\- What changed



Validation:



\- Tests run

\- Build status

\- Deployment or smoke test result



Risk:



\- Low / Medium / High



Rollback:



\- Revert PR or redeploy previous version



\## Reviewer Guidance



\- Feature PRs should be reviewed by the owning application team.

\- Hotfix PRs should include one application reviewer and one release approver.

\- High-risk PRs should be marked as draft until validation is complete.



\## Agent Instructions



When asked to create a PR plan, always return:



\- PR title

\- PR target branch

\- recommended reviewers

\- validation checklist

\- risk level

\- rollback note

