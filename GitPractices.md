# My Git Practices

1. Default `staging` branch (pre-release/beta testing)
2. `master` branch (releases only)
3. Branch protection on `master` and `staging`
   1. No direct push
4. Rebase feature branches from `staging`
5. Require review from code owners (if code ownership is present)

## Understanding Issues vs. PRs, Projects vs. Milestones

1. Say you want a piece of work completed. **Open an Issue**. Within this Issue, describe the work you want done (what specifically, how, why, etc.). (A) developer(s) will be assigned to it and (if the desired changes are deemed reasonable) will begin this work on a new branch. A **Pull Request Draft** will be opened to track discussion on the changes.
2. If this Issue is part of a larger *single deliverable across time*, it will be tracked in **this deliverable's Project board**. The Issue will be moved through the completion columns of the Project board as development progresses. 
3. If the Issue is also part of a *single development phase for many deliverables*, its completion will be tracked in **this phase's Milestone**. Its completion will count towards the completion of that Milestone.
4. Once the work is sufficiently complete, the developer(s) will **Request review on the Pull Request** to merge the branch. If the scope of the PR contains the solution scope of the Issue, the PR should be *linked* to the Issue. Reviews will be requested from relevant reviewers/'code owners', who will either a) request changes be made, or b) approve the PR.
5. On approval of the PR, changes can be merged, and both the Issue and the PR are closed. The piece of work is completed.

## Labels

My labels are divided into three sets. *At least one from each set* should be added to each Issue and PR.

*Note:* each label listed here is preceeded by the label set's name (i.e. `Type: New Feature`)

### Scope

The scope of the Issue. Helps to determine which individuals/teams should be assigned to an Issue/PR.

- `Documentation`: Pertains to project documentation.
- `Meta`: Pertains to repository management.
- `Deliverable`/`Development`: Pertains to primary development of features/functionality.
- Other subsystem-specific labels, if needed.

### Type

What type of Issue is it?

- `Bug`: Unwanted/unpredicted/malfunctioning features.
- `New Feature`: Something new/added.
- `Improvement`: Something upgraded.
- `Maintenance`: Post-release tinkering.

### Status

Perhaps the most important label set. Governs completion, and acts as a flag for admins, reviewers, developers, etc. to quickly understand how the Issue/PR is going.

- `Open`: The Issue is open for anyone to tackle. The default status label.
- `Rejected`: At any time, an Issue may be rejected.
- `Assigned`: A developer/developers have been assigned to the Issue and will begin work.
- `In Progress`: The work has begun. PR Draft has been opened.
- `Blocked`: At any time during development, the feature/bugfix may be dependent on some precondition that has not yet been met.
- `Abandoned`: The Issue or PR has been abandoned for some reason.
- `Review Needed`: PR is ready for review by code owners, or Issue should be reviewed by the submitter.
- `Accepted`: Changes have been accepted. The PR is merged, the Issue is closed.