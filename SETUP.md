# SETUP.md - Step-by-Step Project Submission Guide

Welcome to KMIT Projects! This guide will walk you through **every single step** to submit your project to the official repository.

> **Note:** If you're confused by any step, refer to [SUPPORT.md](SUPPORT.md) for help resources.

---

## Table of Contents

1. [Prerequisites](#prerequisites)
2. [Create a GitHub Account](#create-a-github-account)
3. [Install Git](#install-git)
4. [Fork the Repository](#fork-the-repository)
5. [Clone Your Fork](#clone-your-fork)
6. [Prepare Your Project](#prepare-your-project)
7. [Commit Your Changes](#commit-your-changes)
8. [Push to GitHub](#push-to-github)
9. [Create a Pull Request](#create-a-pull-request)
10. [Wait for Review](#wait-for-review)

---

## Prerequisites

Before starting, make sure you have:

- ✅ Your project completed and tested
- ✅ A computer with internet connection
- ✅ About 30 minutes to complete this process
- ✅ Basic familiarity with your project files

You will need to create these if you don't have them:

- [ ] GitHub account
- [ ] Git installed on your computer

---

## Create a GitHub Account

### If You Already Have GitHub

Skip this section and go to [Install Git](#install-git).

### If You Don't Have GitHub

1. **Open your web browser** and go to:
   ```
   https://www.github.com
   ```

2. **Click "Sign Up"** button (top-right corner)

3. **Enter your email address** you want to use for GitHub
   - Use a personal email you have access to
   - Example: `your.name@gmail.com`

4. **Create a password**
   - Make it strong (at least 12 characters)
   - Write it down somewhere safe

5. **Choose a username**
   - This will be your GitHub username
   - Example: `johndoe123`
   - Make it professional (you'll use it in projects)
   - Avoid spaces or special characters

6. **Complete verification**
   - GitHub will send an email to verify your account
   - Open the email and click the verification link

7. **Fill in your profile (optional but recommended)**
   - Add your name
   - Add a profile picture
   - Add your location (KMIT, Hyderabad)

✅ **You now have a GitHub account!**

---

## Install Git

### What is Git?

Git is software that helps you manage file versions and work with GitHub.

### For Windows Users

1. **Go to:** https://git-scm.com/download/win

2. **Download the installer** (latest version)

3. **Run the installer**
   - Double-click the downloaded file
   - Click "Yes" when asked "Do you want to allow this app..."
   - Click "Next" through all screens (default options are fine)
   - Click "Install"
   - Click "Finish"

4. **Verify installation**
   - Press `Windows Key + R`
   - Type: `cmd`
   - Press Enter
   - Type: `git --version`
   - You should see: `git version 2.x.x...`

### For macOS Users

1. **Open Terminal**
   - Press `Cmd + Space`
   - Type: `Terminal`
   - Press Enter

2. **Install Git using Homebrew**
   - Type this command and press Enter:
   ```bash
   /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
   ```

3. **After Homebrew installs, type:**
   ```bash
   brew install git
   ```

4. **Verify installation**
   - Type: `git --version`
   - You should see: `git version 2.x.x...`

### For Linux Users (Ubuntu/Debian)

1. **Open Terminal**
   - Press `Ctrl + Alt + T`

2. **Type these commands one by one:**
   ```bash
   sudo apt update
   sudo apt install git
   ```

3. **Verify installation**
   - Type: `git --version`
   - You should see: `git version 2.x.x...`

✅ **Git is now installed!**

---

## Fork the Repository

Forking creates your own copy of the KMIT projects repository.

### Step 1: Open the Repository

1. **Open your web browser**

2. **Go to:**
   ```
   https://github.com/kmit-officialcloud/projects
   ```

3. **You should see:**
   - A folder icon with "kmit-officialcloud/projects" at the top
   - A "Fork" button in the top-right area

### Step 2: Click Fork

1. **Look for the "Fork" button** at the top-right of the page
   - It looks like a fork icon with a number next to it

2. **Click the "Fork" button**

3. **GitHub will ask:**
   - Owner: Select your GitHub username
   - Repository name: Keep as "projects"
   - Description: Leave empty
   - Copy the main branch only: Leave checked

4. **Click "Create fork"**

### Step 3: Verify the Fork

1. **After forking, GitHub will show:**
   ```
   <your-username>/projects
   forked from kmit-officialcloud/projects
   ```

2. **You now have your own copy!**

✅ **Repository forked successfully!**

---

## Clone Your Fork

Cloning downloads your fork to your computer.

### Step 1: Get the Clone URL

1. **Go to your fork** (should still be open in browser)
   ```
   https://github.com/<your-username>/projects
   ```

2. **Click the green "Code" button** (top-right area)

3. **Select "HTTPS"** (should be default)

4. **Click the copy icon** (small icon next to the URL)
   - The URL looks like: `https://github.com/<your-username>/projects.git`

### Step 2: Open Terminal/Command Prompt

**For Windows:**
- Press `Windows Key + R`
- Type: `cmd`
- Press Enter

**For macOS:**
- Press `Cmd + Space`
- Type: `Terminal`
- Press Enter

**For Linux:**
- Press `Ctrl + Alt + T`

### Step 3: Navigate to Your Projects Folder

In Terminal, type:

```bash
cd Desktop
```

Or wherever you want to save the project folder. (Desktop is fine for beginners.)

### Step 4: Clone the Repository

Type this command:

```bash
git clone https://github.com/<your-username>/projects.git
```

Replace `<your-username>` with your actual GitHub username.

Example:
```bash
git clone https://github.com/johndoe123/projects.git
```

### Step 5: Wait for Download

- Git will download the repository
- You should see progress messages
- Wait until it finishes (usually 5-30 seconds)

### Step 6: Navigate Into the Folder

Type:
```bash
cd projects
```

### Step 7: Verify Clone

Type:
```bash
ls
```

You should see folders:
```
SDC-I
RTRP
SDC-II
```

✅ **Repository cloned successfully!**

---

## Prepare Your Project

Now you'll add your project to the correct course folder.

### Step 1: Identify Your Course Folder

Choose the correct folder:

| If Your Course Is | Go To Folder |
|------------------|------------|
| Skill Development Course I | `SDC-I` |
| Real Time Research Projects | `RTRP` |
| Skill Development Course II | `SDC-II` |

### Step 2: Create Your Project Folder

In Terminal, type:

```bash
cd SDC-I
```

(Replace with your course folder if different)

Then create your project folder:

```bash
mkdir your-project-name
cd your-project-name
```

**Important:** Use this naming format:
```
FirstName-LastName-ProjectTitle
```

Example:
```bash
mkdir john-doe-expense-tracker
cd john-doe-expense-tracker
```

### Step 3: Prepare Your Project Files

1. **Find your project on your computer**
   - Open File Explorer / Finder

2. **Copy all your project files**
   - Source code
   - Documentation
   - Screenshots
   - Configuration files
   - etc.

3. **Paste them into your project folder**
   - Navigate to: `Desktop/projects/SDC-I/john-doe-expense-tracker/`
   - Paste all your files here

### Step 4: Create README.md

If you don't have a README.md, create one.

**Windows:**
- Right-click in the folder
- Select "New" → "Text Document"
- Rename to `README.md`

**Mac/Linux:**
- In Terminal, type:
```bash
touch README.md
```

**Add content to README.md:**

Open it with any text editor and add:

```markdown
# Project Title

## Overview
Brief description of your project (2-3 sentences).

## Features
- Feature 1
- Feature 2
- Feature 3

## Technology Stack
- Language: Python 3.9
- Framework: Flask
- Database: SQLite

## Installation

### Prerequisites
- Python 3.8+
- pip

### Setup
1. Clone this repository
2. Install dependencies: `pip install -r requirements.txt`
3. Run: `python main.py`

## Usage
Explain how to use your project.

## Screenshots
[Add screenshots of your project]

## Author
- Name: [Your Name]
- Roll Number: [Your Roll Number]
- Year: [First/Second/Third]

## License
MIT License
```

### Step 5: Create .gitignore

Create a `.gitignore` file to prevent committing sensitive files.

**Windows:**
- Right-click in the folder
- Select "New" → "Text Document"
- Name it `.gitignore` (with the dot)

**Mac/Linux:**
- In Terminal, type:
```bash
touch .gitignore
```

**Add this content:**

```
# Python
__pycache__/
*.py[cod]
venv/
env/
.env

# Node.js
node_modules/
npm-debug.log

# IDE
.vscode/
.idea/

# OS
.DS_Store
Thumbs.db

# Secrets
secrets.json
*.pem
*.key
```

### Step 6: Verify Your Project Structure

Your folder should look like:

```
john-doe-expense-tracker/
├── README.md
├── .gitignore
├── main.py
├── requirements.txt
├── src/
│   ├── app.py
│   └── utils.py
├── screenshots/
│   ├── home.png
│   └── dashboard.png
└── docs/
    └── API.md
```

✅ **Project prepared successfully!**

---

## Commit Your Changes

Committing saves your project with a message.

### Step 1: Open Terminal in Project Folder

Navigate to your project folder in Terminal:

```bash
cd Desktop/projects/SDC-I/john-doe-expense-tracker
```

Or if you're already in the projects folder:

```bash
cd SDC-I/john-doe-expense-tracker
```

### Step 2: Check Status

Type:
```bash
git status
```

You should see all your files listed in red.

### Step 3: Stage All Files

Type:
```bash
git add .
```

This prepares all files for commit.

### Step 4: Verify Staging

Type:
```bash
git status
```

Now your files should be listed in green.

### Step 5: Commit

Type:
```bash
git commit -m "Add Expense Tracker project for SDC-I"
```

Replace the message with your project name.

**Good commit messages:**
- "Add Smart Attendance System (SDC-I)"
- "Add AI Resume Analyzer (RTRP)"
- "Add Weather Application (SDC-II)"

**Bad commit messages:**
- "Add project"
- "changes"
- "fix"

### Step 6: Verify Commit

Type:
```bash
git status
```

You should see:
```
On branch main
nothing to commit, working tree clean
```

✅ **Changes committed successfully!**

---

## Push to GitHub

Pushing uploads your changes to GitHub.

### Step 1: Push to Your Fork

In Terminal, type:

```bash
git push origin main
```

### Step 2: Provide GitHub Credentials (First Time Only)

GitHub may ask for your credentials:

**If using HTTPS:**
- Username: Your GitHub username
- Password: Your GitHub password (or Personal Access Token if you have 2FA)

**If it doesn't ask, that's fine!**

### Step 3: Wait for Upload

Git will show progress:
```
Enumerating objects: 15, done.
Counting objects: 100% (15/15), done.
Writing objects: 100% (15/15), 5.23 KiB | 1.04 MiB/s, done.
...
```

### Step 4: Verify Push

Type:
```bash
git status
```

Should show:
```
Your branch is up to date with 'origin/main'.
```

### Step 5: Verify on GitHub

1. **Go to your fork on GitHub:**
   ```
   https://github.com/<your-username>/projects
   ```

2. **Look for your project folder** under `SDC-I/` (or your course)

3. **Click on it** to see your files

✅ **Changes pushed to GitHub successfully!**

---

## Create a Pull Request

A Pull Request asks the official repository to merge your project.

### Step 1: Go to Your Fork

1. **Open:** https://github.com/<your-username>/projects

2. **Replace `<your-username>`** with your actual GitHub username

### Step 2: Find the Compare & Pull Request Button

1. **Look for a yellow banner** at the top that says:
   ```
   Compare & pull request
   ```

2. **Click the "Compare & pull request" button**

If you don't see it, click "Contribute" button, then "Open pull request"

### Step 3: Fill in the Pull Request Form

You'll see a form with:

#### Title
Fill in:
```
Add [Project Name] - [Course Code]
```

Example:
```
Add Expense Tracker - SDC-I
```

#### Description
Fill in the template provided. It should include:

```
## Project Information

**Project Name:** Expense Tracker

**Course:**
- [X] SDC-I
- [ ] RTRP
- [ ] SDC-II

**Student Name:** John Doe
**Roll Number:** 21K-1234
**Department:** CSE
**Year:** Second Year
**Faculty Guide:** Prof. Jane Smith

## Project Description

A web-based expense tracking application that helps users manage their daily expenses, track spending patterns, and generate reports.

## Features

- [X] User authentication
- [X] Add/Edit/Delete expenses
- [X] Expense categories
- [X] Monthly reports
- [X] Dashboard with statistics

## Technology Stack

- **Language:** Python 3.9
- **Framework:** Flask
- **Database:** SQLite
- **Frontend:** HTML, CSS, JavaScript

## Checklist

- [X] My project builds successfully
- [X] README.md is included and complete
- [X] Documentation is clear
- [X] Screenshots added
- [X] Source code included
- [X] No secrets committed
- [X] No plagiarism
- [X] Project in correct course folder
- [X] Project tested and working
```

### Step 4: Review Before Submitting

**Before clicking "Create pull request":**

✅ Check that:
- [ ] Title is clear and descriptive
- [ ] Course is selected correctly
- [ ] All student information is accurate
- [ ] Description is complete
- [ ] All checklist items are checked
- [ ] No sensitive information is included

### Step 5: Create Pull Request

Click the green **"Create pull request"** button

### Step 6: Your Pull Request is Created!

You'll see a success message with a PR number, like:
```
Pull Request #42
```

✅ **Pull Request created successfully!**

---

## Wait for Review

Your project is now submitted!

### What Happens Next

1. **Faculty reviewers** will be notified
2. **They'll examine** your code and documentation
3. **They may request** changes or ask questions
4. **You may need** to make improvements
5. **Once approved**, your PR will be merged

### Review Timeline

**Expected time:** 3-7 business days

**What you might see:**

✅ **Approved & Merged** — Your project is accepted!

🔄 **Changes Requested** — Reviewers want improvements

❌ **Rejected** — Project doesn't meet requirements

### If Changes Are Requested

1. **Read the comments** on your Pull Request

2. **Make the requested changes** to your local files

3. **Commit again:**
   ```bash
   git add .
   git commit -m "Address review feedback"
   git push origin main
   ```

4. **Your PR automatically updates!**

5. **Reviewers will check again**

### If Merged

🎉 **Congratulations!**

Your project is now part of the official KMIT repository!

---

## Troubleshooting

### Git Commands Not Found

**Problem:** `git: command not found` or `'git' is not recognized`

**Solution:**
- Git is not installed properly
- Reinstall Git from https://git-scm.com/
- Restart your Terminal/Command Prompt

### Authentication Failed

**Problem:** `fatal: Authentication failed` when pushing

**Solution:**
- Check your GitHub password
- If using 2FA, create a Personal Access Token:
  - GitHub Settings → Developer Settings → Personal Access Tokens
  - Use token instead of password

### Remote Already Exists

**Problem:** `fatal: remote origin already exists`

**Solution:**
```bash
git remote remove origin
git remote add origin https://github.com/<your-username>/projects.git
```

### Changes Not Showing on GitHub

**Problem:** Pushed but files don't appear on GitHub

**Solution:**
```bash
git push origin main --force
```

⚠️ **Use `--force` carefully! Only on your own fork.**

### Need More Help?

See [SUPPORT.md](SUPPORT.md) for detailed help resources and contact information.

---

## Summary

You've successfully:

✅ Created a GitHub account
✅ Installed Git
✅ Forked the KMIT repository
✅ Cloned your fork
✅ Prepared your project
✅ Committed your changes
✅ Pushed to GitHub
✅ Created a Pull Request

**Now wait for faculty review!**

---

## Quick Reference

### All Commands in Order

```bash
# Clone your fork
git clone https://github.com/<your-username>/projects.git
cd projects

# Create project folder
cd SDC-I
mkdir your-project-name
cd your-project-name

# Add your files here...

# Commit
git add .
git commit -m "Add project: Your Project Name"

# Push
git push origin main
```

Then create Pull Request through GitHub website.

---

## Next Steps

After submission:

1. **Wait for faculty review** (3-7 days)
2. **Check for comments** on your PR
3. **Make any requested changes**
4. **Your project gets merged!**
5. **Share your achievement!** 🎉

---

## Additional Resources

- [CONTRIBUTING.md](CONTRIBUTING.md) — Detailed contribution guidelines
- [SECURITY.md](SECURITY.md) — Security best practices
- [CODE_OF_CONDUCT.md](CODE_OF_CONDUCT.md) — Community standards
- [SUPPORT.md](SUPPORT.md) — Help and support
- [GitHub Guides](https://guides.github.com/) — Official GitHub help
- [Git Documentation](https://git-scm.com/doc) — Git reference

---

## Questions?

If you're stuck on any step:

1. **Check [SUPPORT.md](SUPPORT.md)** for help resources
2. **Open a GitHub Issue** with your question
3. **Contact your instructor** for academic guidance
4. **Email:** contact@kmit.in

---

<div align="center">

**Good luck with your submission!**

You've got this! 🚀

</div>

---

*Last updated: 2026*
*Maintained by: KMIT Repository Team*
