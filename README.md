# GIT-PUSH

A lightweight, one-click Windows automation tool designed to streamline your Git workflow. Say goodbye to repetitive typing of `git add`, `git commit`, and `git push` commands!

---

## ✨ Features

* **One-Click Workflow:** Automates the entire staging, committing, and pushing process in seconds.
* **Custom Commit Messages:** Prompts you to enter your commit message directly from the command window.
* **Branch Awareness:** Automatically pushes your changes to the currently connected remote branch.
* **Zero Dependencies:** Built purely using Windows Batch scripting (`.bat`) — no extra installations or heavy software required.

---

## 🛠️ How It Works

The batch script performs the following Git operations sequentially:
1. `git status` — Checks for modified or untracked files.
2. `git add .` — Stages all your changes.
3. `git commit -m "Your Message"` — Commits changes with your custom message.
4. `git push origin <branch>` — Pushes the commit to your connected repository.

---

## 🚀 Getting Started & Installation

### 1. Prerequisites
Make sure you have **Git** installed on your system and added to your system Environment Variables (PATH). Also, ensure your local repository is already connected to a remote GitHub/GitLab repository.

### 2. Setup
1. Clone or download this project into your local machine.
2. Place the `.bat` script inside the root directory of your project repository.

---

## 💻 Usage

1. Double-click the `.bat` file (or run it from your command prompt / terminal).
2. When prompted, type your **commit message** and press `Enter`.
3. Sit back and watch your code get successfully pushed to the remote repository!

```bat
:: Example of what the terminal looks like
Enter your commit message: fixed login bug and updated styling
[3 operations running...]
Successfully pushed to origin/main!
