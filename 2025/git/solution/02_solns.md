# 🚀 Week 4: Git & GitHub Advanced Challenge – #90DaysOfDevOps

Welcome to **Week 4** of the **90 Days of DevOps** challenge! This week dives deep into advanced Git concepts that are **essential for real-world DevOps workflows**.

***

## 📚 What I Learned

✅ By the end of this week, I understood and practiced:

- Collaborating through **Pull Requests**
- Undoing changes using **Reset** & **Revert**
- Using **Stashing** to manage uncommitted work
- Applying **Cherry-picking** for selective commits
- Maintaining a clean commit history using **Rebasing**
- Learning **industry-standard Git Branching Strategies**

***

## 📌 Topics Covered

| Task No. | Topic                       | Description                                 |
|***-|***--|***|
| 1        | Pull Requests               | Team collaboration via PRs                  |
| 2        | Reset & Revert              | Safely undoing changes                      |
| 3        | Stashing                    | Temporarily saving uncommitted work         |
| 4        | Cherry-picking              | Selectively applying specific commits       |
| 5        | Rebasing                    | Clean, linear commit history                |
| 6        | Branching Strategies        | Git Flow, GitHub Flow, Trunk-Based Workflow |

***

## 🧠 Challenge Tasks & Highlights

### 🔹 Task 1: Pull Requests (PRs)
- Created a feature branch and made changes.
- Pushed to GitHub and opened a PR.
- Followed best practices for PR description and review handling.

🔍 _Learned:_ Clear PR titles and comments ease collaboration and improve code quality.

***

### 🔹 Task 2: Reset & Revert
- Practiced `git reset` (soft, mixed, hard) and `git revert`.
- Understood safe vs destructive undo operations.

🔍 _Learned:_  
- `reset` is local and destructive.  
- `revert` is safe and creates a new commit.

***

### 🔹 Task 3: Git Stash
- Stashed uncommitted work before switching branches.
- Used `stash pop` to reapply changes.

🔍 _Learned:_  
- `stash pop` removes the stash after applying.  
- `stash apply` keeps it.

***

### 🔹 Task 4: Cherry-Picking
- Used `git cherry-pick <commit-hash>` to apply specific commits.
- Resolved merge conflicts manually.

🔍 _Learned:_  
Useful for applying hotfixes or critical updates across branches.

***

### 🔹 Task 5: Rebase
- Rebasing feature branch onto updated main.
- Compared `merge` vs `rebase`.

🔍 _Learned:_  
Rebase keeps the history clean, merge preserves context.  
Use `rebase` before merging to avoid noisy commit graphs.

***

### 🔹 Task 6: Branching Strategies
- Explored and simulated:
  - **Git Flow**
  - **GitHub Flow**
  - **Trunk-Based Development**

🔍 _Learned:_  
- **GitHub Flow** is simple and CI/CD-friendly.  
- **Trunk-Based Development** supports rapid releases.  
- **Git Flow** is good for release-based projects.

***

## 📝 How to Submit

```bash
git add .
git commit -m "Completed Git & GitHub Advanced Challenge"
git push origin main
