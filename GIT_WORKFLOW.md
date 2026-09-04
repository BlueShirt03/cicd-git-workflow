# Git Workflow Standardization 

## Repository

GitHub Repository: https://github.com/BlueShirt03/cicd-git-workflow.git

---

## Overview

This repo uses the Feature Branch Workflow to support reliable CI practices

Development work is completed on separate branches instead of directly on the 'main' branch. Changes are then submitted through Pull Requests (PR), reviewed, and approved before being merged into 'main'.

---

## Branching Strategy 

the 'main' branch represents the stable version of the project. 

Developers should not make normal development changes directly on 'main'. Instead, a new breanch should be created from 'main' for each feature, bug fixes, or documentation change.

After the work is completed, the branch shoud be pushed into GitHub and submitted through a PR,

### Branch Naming Conventions 

Branches should use lowercase names with words separated by hyphens.

The following prefixes are used:

- feature/ - New features or projects functionality
- bugfix/ - Bug fixes
- docs/ - Documentation changes


Examples:

- feature/project-setup
-  bugfix/fix-validation
-  docs/git-workflow

Using consisent branch names will ensure that ability to understand the purpose of each branch.

---

## Commit Message Standards

This repo follows the Conventional Commits standard.

Commit messages should follow this format:

type: short description

Common commit types include:

- feat: - Adds new functionality
- fix: - Fixes a bug
- docs: - Documentation changes
- test: - Adds or updates tests
- refactor: - Restructures code without changing its behavior
- chore: - Maintenance or configuration changes


Examples:

- feat: add user login
- fix: correct input validation
- docs: expand project README
- docs: add Git workflow documentation
- test: add validation tests
- chore: update project configuration

Commits messages should be clear, concise, and accurately describe the change being made.

---

## Pull Request Process

All changes to the 'main' branch must be submitted through a PR. 

The sandard PR process is:

1. Start from the latest version of main.
2. Create a new feature, bug fix, or documentation branch.
3. Make the required changes on the new branch.
4. Stage the changes with Git.
5. Commit the changes using Conventional Commit standards.
6. Push the branch to GitHub.
7. Open a Pull Request targeting the main branch.
8. Request a code review.
9. Address any reviewer comments or requested changes.
10. Receive the required approval.
11. Merge the Pull Request into main.
12. Delete the completed branch when it is no longer needed.

This process prevents unreviewed work from being directly integrated into the stabel branch.

---

## Code Review Process 

Pull Request require at least one approving review before they can be merged into 'main'.

a reviewer should examine the proposed changes before approving before approving PR.

Reviewers should verify that:

- The changes match the intended purpose of the branch.
- The code or documentation is clear and organized.
- Branch naming conventions are followed.
- Commit messages follow the defined standard.
- The changes do not introduce unnecessary problems.
- The Pull Request is ready to be integrated into main.

If problems are found, the reviewer can leave comments or request changes.

Any required changes should be completed and resolved conversation should be addressed before the Pull Request is merged.

---

## Merge Approval Process

The 'main' branch is protected using GitHub repo rules.

the following protections are configured:

- Pull Requests are required before merging into main.
- At least one approving review is required.
- Pull Request conversations must be resolved before merging.
- Force pushes to main are blocked.
- Deletion of the protected main branch is restricted.
- Additional approval for unattributed Copilot pull requests

Once all required conditions are satisfied, the Pull Request can be merged into main.