# 🧪 **Classroom Activity: Git Collaboration Simulation**

## 🎯 **Objective**

Practice essential Git collaboration skills in a team setting:

- ✅ Creating and managing a shared repository
- ✅ Cloning repositories and creating feature branches
- ✅ Pushing changes and understanding Pull Requests
- ✅ Resolving merge conflicts (optional)
- ✅ Logging Git-based contributions to a timesheet

---

## 👥 **Group Setup**

- Form student groups of **3 members**
- Assign roles:
  - 🧑 Repository Owner (creates and manages repo)
  - 👩‍💻 Collaborators (contribute via branches)

---

## 👤 **Repository Owner Instructions**

### 🧱 Step 1: Create a Shared Repository

1. Log into GitHub.
2. Click **New Repository**:
   - Name: `Git-Practice-TeamAlpha`
   - Set to **Private**
   - Check `✔️ Add a README file`

> 🧠 A README file provides an initial commit and context for your team.

---

### 🧑‍🤝‍🧑 Step 2: Add Collaborators

1. Go to **Settings → Collaborators**
2. Add teammates by their GitHub usernames.
3. Grant **Write access**

> 🧠 Write access allows others to push changes to the repository.

---

### 🔗 Step 3: Share the Repo

You don’t need to send the repo URL manually—since you’ve invited your collaborators, they will be notified via GitHub/email.  
Still, it’s good to note down the repo URL for reference or troubleshooting.

---

## 👥 **Collaborator Instructions**

### 🧭 Step 1: Accept the Invitation

- Accept the GitHub invite via email or your GitHub dashboard.

---

### 📥 Step 2: Clone the Repository

#### ✅ What does “clone” mean?

Cloning a repo means **creating an exact copy of the repository on your local computer**.  
You can now edit files and make changes locally.

📣 **Important:** Even the **repository owner** must clone it too. Creating the repo on GitHub doesn't automatically put it on their machine.

Command:

```bash
git clone https://github.com/owner-name/Git-Practice-TeamAlpha.git
```

> 🧠 Cloning sets the stage for local development.

---

## 🧩 **Practice HTML Tasks**

Create a collaborative 3-page website:

| Member      | Task                                   |
|-------------|----------------------------------------|
| Member 1    | `index.html` – homepage                |
| Member 2    | `about.html` – group details           |
| Member 3    | `contact.html` – email contacts        |

> 🚨 If your group has 2 members, combine tasks or save `contact.html` for later.

📝 **Instructions:**
- Each member downloads the assigned HTML file from GitHub (via browser or terminal).
- Move it into the cloned repo folder.
- Personalize and edit the file with relevant content.
- Save and prepare for commit.

---

## 🌿 **Git Workflow Explained**

### 🧠 What is a Branch?

A branch is like a personal workspace—it lets you work on new features or files **without affecting others’ code or the main version**.

Why branches matter:
- Keeps individual contributions separate.
- Prevents overwriting team members' work.
- Allows smoother integration later.

---

### 🔀 Step 1: Create Your Branch

Each student creates a uniquely named branch, like:

```bash
git checkout -b feature-aboutPage
```

> 🧠 This command creates and switches to a new branch.

---

### ✍️ Step 2: Make Your Edits

Use a code editor (VS Code, Sublime, etc.) to update your HTML file.

---

### 📦 Step 3: Stage and Commit Your Work

After editing:

```bash
git add .
git commit -m "Added about.html with team details"
```

- `git add .` stages all changes
- `git commit` saves a snapshot of your progress

---

### ☁️ Step 4: Push to GitHub

```bash
git push origin feature-aboutPage
```

✅ After pushing:
- Visit GitHub in a browser.
- Click on “Branches” tab to **view all teammates’ branches** and work in progress.

---

### 🔃 Step 5: Create a Pull Request (PR)

🔎 **Why switch to your branch online first?**

So GitHub knows which branch you're proposing to merge. The student who worked on the branch initiates this.

🧠 What is a “Pull Request”?

It’s a request to merge your branch into the `main` branch.
Think of it as: “I’m ready to add my page—can someone review it and approve?”

#### Steps:

1. On GitHub, switch to your branch.
2. Click **Compare & pull request**
3. Add a short description.
4. Click **Create pull request**

---

### ✅ Step 6: Review & Merge

🧠 What is a “Merge”?

Merging is taking the changes from one branch and adding them into another—usually `main`.

Clarifications:
- PRs can be merged one by one.
- Every branch gets individually merged.
- Students review each other's PRs before merging.

### After Merge:
Everyone (not just the PR creator) must run:

```bash
git pull origin main
```

🎯 Why?

This updates your local project with **the new merged content**, giving you access to the full collaborative site—`index.html`, `about.html`, and `contact.html`.

---

## 💢 **Bonus: Merge Conflict Demo (Optional)**

Conflict example:

1. Two students edit the exact same line of `index.html` on different branches.
2. Each pushes and opens a PR.
3. GitHub detects a **merge conflict**.
4. Teammates must resolve the conflict manually:
   - GitHub shows which lines are in conflict.
   - Decide which version to keep or combine.
   - Edit the file, save, commit, and re-push.

> 🧠 Conflict resolution is a vital real-world skill!

---

## 📝 Timesheet Logging

Update the official **Excel Timesheet Template** — to record the Git collaboration journey:

🎯 Students should log this in-class acitivty:

- Every commit made
- Branch name used
- Commit message
- Date and time
- Task type (attendance, research, dev, etc.)

You are required to update it in real time during the session.

---

