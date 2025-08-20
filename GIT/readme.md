# Git

- [Git documentation](https://git-scm.com/book/en/v2/Getting-Started-About-Version-Control)

---

Here’s the difference 👇

---

## 🔹 **Git**

* A **tool** (version control system).
* Installed on your computer.
* Lets you track changes, create branches, and manage code history.
* Works completely **offline** (you don’t need internet).
* Example commands: `git init`, `git add`, `git commit`, `git branch`, `git merge`.

---

## 🔹 **GitHub**

* A **platform/service** that hosts Git repositories online.
* Built on top of Git.
* Lets teams **collaborate**, share, and contribute code remotely.
* Provides extra features: pull requests, issues, actions (CI/CD), project boards, etc.
* Alternatives: GitLab, Bitbucket.

---

### ⚡ Analogy

* **Git** = The engine of a car (does the actual version control).
* **GitHub** = The garage where you store/share your car with others.

---

✅ In short:

* **Git = local version control tool**.
* **GitHub = cloud hosting + collaboration for Git repos**.

Do you want me to also explain **how Git and GitHub work together in a typical workflow** (like cloning, pushing, pulling)?


## 🔹 Git has 3 areas

1. **Working Directory** – your actual project files.
2. **Staging Area (Index)** – a "waiting room" where you put changes before committing.
3. **Repository (History)** – the permanent commit history.

---

## 🔹 Staging

When you edit a file, it’s only in the **working directory**.
To prepare it for commit, you must **stage it**:

```bash
git add <file>
```

Now the file is in the **staging area** → ready to be committed.

Example:

```bash
git add file1.txt
```

---

## 🔹 Committing

When you commit, Git takes whatever is in the **staging area** and saves it permanently in the **repository**:

```bash
git commit -m "Added new feature"
```

---

## 🔹 Unstaging

If you staged something by mistake, you can **unstage it** (move it back to working directory):

```bash
git reset HEAD <file>
```

Example:

```bash
git reset HEAD file1.txt
```

Now the file is still modified, but no longer staged.

---

## 🔹 Discarding changes

* If you also want to **discard changes** in the working directory:

  ```bash
  git checkout -- <file>
  ```
* If you want to discard **all changes**:

  ```bash
  git reset --hard
  ```

---

### ⚡ Quick Mental Model

* **Edit** → changes are in **working directory**
* **Stage (`git add`)** → moves changes to **staging area**
* **Commit (`git commit`)** → moves staged changes into **repo history**
* **Unstage (`git reset HEAD`)** → move back from staging to working directory

---

---

## 🔹 Basic Git Knowledge

* **What Git is**: A distributed version control system (tracks changes in code, works offline, supports branching).
* **Repository (repo)**: A project folder tracked by Git.
* **Commit**: A snapshot of your changes.
* **Branch**: A separate line of development.
* **Merge**: Combines changes from one branch into another.
* **Remote**: A version of your repo stored on GitHub/GitLab/Bitbucket, etc.
* **Clone**: Downloading a repo from a remote.
* **Pull**: Getting latest changes from remote to local.
* **Push**: Sending your commits from local to remote.
* **Conflict**: When Git can’t auto-merge changes → requires manual resolution.

---

## 🔹 Most Used Git Commands

### 📌 Setup

```bash
git config --global user.name "Your Name"
git config --global user.email "your@email.com"
```

### 📌 Starting a project

```bash
git init                     # Initialize new repo
git clone <repo-url>         # Copy remote repo locally
```

### 📌 Tracking changes

```bash
git status                   # Show changed files
git add <file>               # Stage file for commit
git add .                    # Stage all changes
git commit -m "Message"      # Commit staged changes
```

### 📌 Branching & merging

```bash
git branch                   # List branches
git branch <name>            # Create new branch
git checkout <name>          # Switch branch
git checkout -b <name>       # Create & switch to new branch
git merge <branch>           # Merge branch into current one
```

### 📌 Remote (GitHub, GitLab, etc.)

```bash
git remote -v                # Show remotes
git push origin <branch>     # Push commits to remote
git pull origin <branch>     # Fetch + merge latest changes
git fetch                    # Download changes without merging
```

### 📌 Undoing changes

```bash
git reset --hard             # Reset all changes (dangerous!)
git checkout -- <file>       # Discard local changes in file
git revert <commit>          # Undo commit (safe, creates new commit)
```

---

👉 Quick workflow you’ll use most often:

1. `git status` → check what changed
2. `git add .` → stage changes
3. `git commit -m "message"` → save snapshot
4. `git push origin branch-name` → upload changes

---
