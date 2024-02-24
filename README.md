# Zone Alerte

We are a safety prevention platform, giving people the opportunity to protect themselves and their loved ones through the solutions we provide to them to report when they are in danger, track their loved ones' trajectories to be aware of their last position, and give parents the ability to properly monitor their children.

## Versioning with Git & Github

### Workflow

We use the Git-flow workflow but modified according to our way of working, which requires any developer working on our solutions to respect the rules set out below.

Which means that we have three main branches including `main`, `staging` and `develop`.

#### Principals Branches

1. `Production` : The production branch is `main`.

`main` contains stable bug-free code, the content of which comes from the merge of the branch `staging`, or from a `hotfix` branch after fixing a bug in production. 

2. `Staging` : Staging or pre-production branch is `staging`, it contains the stable code base ready to push to production.

It contains the codebase ready to move to main for deployment.

- Push & Pull-request: Only the developer designated to do the review, or as the project lead, can push or merge the Pull-request.

- Only the content (Pull-request) coming from the `develop` branch can be pushed to `staging`.

3. `Develop`: This is the development branch, meaning it contains the latest project code updates. It is composed of content from all other working branches. The concept of a working branch is discussed in the following point on Branch Naming.

#### Branch Naming

1. `Feature Branches`: These branches are used for developing new features. Use the prefix feature/. For instance, `feature/login-system`.

2. `Bugfix Branches`: These branches are used to fix bugs in the code. Use the prefix fix/. For example, fix/header-styling.

3. `Hotfix Branches`: These branches are made directly from the production branch to fix critical bugs in the production environment. Use the prefix `hotfix/`. For instance, `hotfix/critical-security-issue`.

When there is a hotfix, the branch would be merged into both main and develop after the fix.

4. `Release Branches`: These branches are used to prepare for a new production release. They allow for last-minute dotting of i’s and crossing t’s. Use the prefix `release/`. For example, `release/v1.0.1`.

5. `Documentation Branches`: These branches are used to write, update, or fix documentation. Use the prefix `docs/`. For instance, `docs/api-endpoints`.

