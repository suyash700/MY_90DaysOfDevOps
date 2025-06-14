# 🚀 Week 4: Git & GitHub Challenge – 90 Days of DevOps

This repository documents my progress for **Week 4** of the [#90DaysOfDevOps](https://github.com/LondheShubham153/90DaysOfDevOps) challenge by **Shubham Londhe Bhaiya**. This week was all about **practicing Git, GitHub, and understanding branching strategies**, along with a bonus task on **SSH Authentication**.

---

## ✅ Tasks Covered

### 🔹 Task 1: Fork and Clone the Repository

- Forked the [main repo](https://github.com/LondheShubham153/90DaysOfDevOps) to my GitHub account.
- Cloned the fork locally:
  ```bash
  git clone https://github.com/suyash700/90DaysOfDevOps.git
  cd 90DaysOfDevOps/2025/git/01_Git_and_Github_Basics

🔹 Task 2: Initialize Git & Create a File

mkdir week-4-challenge
cd week-4-challenge
git init
echo "Hi, I'm suyash. I am learning Git & DevOps!" > info.txt
git add info.txt
git commit -m "Initial commit: Add info.txt with introductory content"

🔹 Task 3: Configure Remote with PAT & Push Changes

git remote add origin https://suyash700:<your-PAT>@github.com/suyash700/90DaysOfDevOps.git
# or update if origin exists
git remote set-url origin https://suyash700:<your-PAT>@github.com/suyash700/90DaysOfDevOps.git
git branch -M main
git push -u origin main
git pull origin main

🔹 Task 4: View Commit History
git log

🔹 Task 5: Branching and Pull Requests
git branch feature-update
git switch feature-update


# Updated the file
echo "I'm excited to explore DevOps tools like Docker, K8s !" >> info.txt
git add info.txt
git commit -m "Feature update: Updated info.txt with more personal info"
git push origin feature-update


🧠 Task 6: Why Branching Strategies Matter
Branching strategies help in:

Isolating features and bug fixes

Facilitating parallel development

Reducing merge conflicts

Enabling proper code reviews

Keeping the main branch production-ready

🎯 Bonus: SSH Authentication

ssh-keygen -t ed25519 -C "suyashdahx@"
# Added public key to GitHub -> Settings -> SSH and GPG keys
git remote set-url origin git@github.com:suyash700/90DaysOfDevOps.git
git push origin feature-update


