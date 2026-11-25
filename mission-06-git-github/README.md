# Mission 6 — Git and GitHub

## 1. Task / objective
Practice the basic Git workflow (`status`, `add`, `commit`, `log`), create and publish a branch named `update-about`, understand Pull Requests, and build a Git command glossary.

## 2. Work completed
Completed Tasks 6.1 through 6.4:
- **Task 6.1:** Practiced checking status, staging files, committing with a clear message, and viewing commit history.
- **Task 6.2:** Created branch `update-about`, added a "My Learning" section to the root `README.md`, committed it, and pushed `update-about` to GitHub.
- **Task 6.3:** Prepared the `update-about` branch on GitHub for a Pull Request into `main`. Status: **Branch pushed; Pull Request not merged** (left unmerged as instructed unless asked by the instructor to merge).
- **Task 6.4:** Created a one-line glossary of common Git operations.

### Task 6.1 — Understand the basic Git workflow

| Git operation | What it does in your own words |
| :--- | :--- |
| Check repository status (`git status`) | Shows which branch I am on and which files are modified, staged, or untracked. |
| Stage selected changes (`git add <file>`) | Marks specific changed files to be included in the next commit. |
| Create a commit (`git commit -m "..."`) | Saves a permanent snapshot of the staged changes in the Git history with a message. |
| View commit history (`git log --oneline`) | Lists past commits with their short IDs and commit messages. |

**Difference between staging and committing:** Staging (`git add`) only picks which changes you want to include—you can still edit or unstage them before saving. Committing (`git commit`) actually records that snapshot into the repository's history.

### Task 6.3 — Branch and Pull Request explanation
- **What is a branch?** A branch is a separate line of development where you can make changes without touching the `main` branch.
- **What is a Pull Request (PR)?** A Pull Request is a request on GitHub asking to review and merge changes from one branch (like `update-about`) into another branch (like `main`).
- **Why they are useful:** When multiple people work on the same project, branches keep everyone's work separate so they do not overwrite each other, and Pull Requests let teammates review changes before merging them into `main`.
- **PR status:** The `update-about` branch is pushed to GitHub (`origin/update-about`) and ready for a Pull Request at `https://github.com/kartiksharma76053/digital-detective-8006/pull/new/update-about`. It is not merged yet.

### Task 6.4 — Git command glossary

| Git operation | One-line explanation |
| :--- | :--- |
| Initialise a repository (`git init`) | Turns a local folder into a new Git repository. |
| Check status (`git status`) | Shows modified, staged, and untracked files on the current branch. |
| Stage changes (`git add`) | Adds file changes to the staging area before committing. |
| Commit changes (`git commit`) | Saves staged changes as a new snapshot in the repository history. |
| View history (`git log`) | Displays the list of past commits made in the repository. |
| Create or list branches (`git branch`) | Lists existing branches or creates a new branch. |
| Switch branches (`git checkout` / `git switch`) | Moves your working directory to another branch. |
| Publish changes (`git push`) | Uploads local commits and branches to the remote repository on GitHub. |
| Retrieve remote changes (`git pull`) | Downloads and merges the latest commits from GitHub into your local branch. |

## 3. Commands / tools used
- `git status`, `git add`, `git commit`, `git log --oneline` — Basic Git workflow.
- `git checkout -b update-about`, `git checkout main` — Creating and switching branches.
- `git push -u origin update-about` — Publishing the new branch to GitHub.

## 4. My understanding
Git tracks changes safely through staging and committing, while branches and Pull Requests let you test or update features without risking the `main` branch.

## 5. Difficulties faced
No major difficulties.

## 6. How I resolved them
Not applicable.

## 7. Evidence / files
- `mission-06-git-github/README.md`
- Branch `update-about` pushed to GitHub (`origin/update-about`)

## 8. Commit details
Committed with message `"Complete Git and GitHub collaboration mission"` and pushed to `origin/main`.
