## My Learning

1. Learned how to use basic terminal commands like `pwd`, `ls -lah`, and `mkdir`.
2. Explored how the OS manages processes, file permissions (`r`, `w`, `x`), and disk storage.
3. Practised converting numbers between binary, decimal, and hex by hand and with Python.

# Mission 6 - Git and GitHub

## Task 6.1 - Basic Git workflow

| Git operation | What it does in your own words |
|---|---|
| Check repository status | Checks which files have been modified, staged, or left untracked (`git status`). |
| Stage selected changes | Marks specific changed files to be included in the next snapshot (`git add`). |
| Create a commit | Permanently records the staged changes with a meaningful summary message (`git commit`). |
| View commit history | Lists the chronological log of previous commits in the repository (`git log`). |

- **Difference between staging and committing:**  
  Staging (`git add`) is like choosing which items to put in a box. Committing (`git commit`) is like sealing and labeling the box so it is officially saved in history.

## Task 6.2 & 6.3 - Branches and Pull Requests

- **What is a branch?**  
  A branch is an isolated workspace where you can safely make changes or test new ideas without affecting the main working version (`main`).
- **What is a Pull Request (PR)?**  
  A Pull Request is a request on GitHub to review, discuss, and merge changes from a feature branch (like `update-about`) into the main branch.
- **Why are they useful?**  
  They allow multiple developers to work on different parts of a project simultaneously without breaking each other's code, ensuring code is reviewed before it becomes part of the main project.
- **PR Status:**  
  Created Pull Request #1 from `update-about` into `main`, reviewed the diff, and merged it into `main`.

## Task 6.4 - Git command glossary

- `git init`: Initialises a brand new Git repository in the current folder.
- `git status`: Displays the status of modified, untracked, and staged files.
- `git add`: Adds file changes to the staging area.
- `git commit`: Saves staged changes as a new commit in the repository history.
- `git log`: Shows the history of past commits.
- `git branch`: Lists branches or creates a new branch.
- `git checkout` / `git switch`: Switches the working directory to another branch.
- `git push`: Uploads local commits to the remote GitHub repository.
- `git pull`: Downloads and merges updates from GitHub into the local repository.

---

## 1. Task / objective

Understand version control, inspect git status, create and push a branch, open and merge a Pull Request on GitHub, and document the collaboration workflow.

## 2. Work completed

Created the `update-about` branch, added the "My Learning" section to root `README.md`, pushed the branch to GitHub, opened and merged Pull Request #1 into `main`, pulled changes back to local `main`, and compiled a Git command glossary.

## 3. Commands / tools used

- `git status`: Checked modified and untracked files.
- `git checkout -b update-about`: Created and switched to the new branch.
- `git add README.md`: Staged the modified root README.
- `git commit -m "..."`: Committed changes locally.
- `git push -u origin update-about`: Published the branch to GitHub.
- GitHub web interface: Created and merged Pull Request #1 into `main`.
- `git checkout main` and `git pull origin main`: Updated local main branch with the merged commit.

## 4. My understanding

Git tracks project versions locally, while GitHub hosts them online for collaboration. Using branches and Pull Requests keeps the main branch stable while features or updates are developed and reviewed.

## 5. Difficulties faced

Initially saved the changes in the wrong README file, which resulted in Git reporting no staged changes to commit for root `README.md`.

## 6. How I resolved them

Appended the "My Learning" section directly to the root `README.md`, staged it, and successfully pushed the commit to GitHub.

## 7. Evidence / files

- `mission-06-git-github/README.md`
- `README.md`
- GitHub Pull Request #1 (merged)

## 8. Commit details

Commit message: `Complete Git and GitHub collaboration mission`

The completed Mission 6 work was committed and pushed to GitHub on the main branch.