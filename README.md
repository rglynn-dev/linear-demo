# Linear Demo
Test repo to show linear github integration

## Background
This is my first ticket, I'm changing the readme!
edit

## Usage
This project demonstrates how to use [Linear](https://linear.app) and GitHub
together so that issues, branches, and pull requests stay linked automatically.

### Prerequisites
- A Linear workspace with the [GitHub integration](https://linear.app/docs/github)
  enabled (Linear → Settings → Integrations → GitHub).
- Write access to this GitHub repository.

### Linking a branch to a Linear issue
Linear generates a suggested branch name for every issue (e.g.
`rglynn/dem-3-add-usage-information-to-lunch-learn-readme`). Use it so Linear can
match the branch to the issue:

1. Open the issue in Linear and copy the branch name (`Cmd/Ctrl + Shift + .`, or
   the "Copy branch name" action in the issue menu).
2. Create the branch locally and start work:
   ```bash
   git checkout -b rglynn/dem-3-add-usage-information-to-lunch-learn-readme
   ```

Because the branch name contains the issue identifier (`DEM-3`), Linear links the
branch to the issue automatically and moves the issue to **In Progress**.

### Opening a pull request
1. Push your branch and open a pull request on GitHub.
2. Reference the issue in the PR title or description (e.g. `DEM-3`). Branches
   created from a Linear-suggested name are linked automatically, so this is
   usually already done for you.
3. Linear attaches the PR to the issue and keeps its status in sync:
   - Opening the PR moves the issue to **In Review**.
   - Merging the PR moves the issue to **Done**.

### Referencing issues in commits
Include the issue identifier in commit messages or the PR body to keep the
history connected, for example:

```
git commit -m "docs: add usage section (DEM-3)"
```

Linear surfaces these references on the issue so the whole team can see the work
as it progresses, without leaving GitHub.
