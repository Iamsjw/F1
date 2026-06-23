# Git & GitHub Guide for UpasthitiX

This guide explains how to easily manage and upload your code changes to GitHub without having to manually delete and upload files.

---

## Step 1: Install Git (If you haven't already)
1. Download Git for Windows from **[git-scm.com](https://git-scm.com/)** and install it using the default settings.
2. Open your terminal/command prompt and run these two commands to configure your details:
   ```bash
   git config --global user.name "Your Name"
   git config --global user.email "your-email@example.com"
   ```

---

## Step 2: Connect this Folder to GitHub (One-Time Setup)
Since your project is already on GitHub:

1. Open your terminal in this project folder (`d:\UPASTHITIX\For csv\csv-main`).
2. Initialize Git in this folder:
   ```bash
   git init
   ```
3. Copy your repository URL from GitHub (e.g., `https://github.com/username/repository.name.git`).
4. Link this local folder to your online GitHub repository:
   ```bash
   git remote add origin https://github.com/your-username/your-repo-name.git
   ```
5. Fetch the files from GitHub so the local and remote folders are in sync:
   ```bash
   git pull origin main
   ```
   *(Note: Replace `main` with `master` if your default branch on GitHub is named master).*

---

## Step 3: Your Everyday Workflow (Only 3 Simple Commands)
Whenever you make edits and want to update GitHub, just open your terminal in this folder and run:

1. **Stage your changes** (tells Git to bundle all edited files):
   ```bash
   git add .
   ```
2. **Commit your changes** (saves the bundle with a short note explaining what you changed):
   ```bash
   git commit -m "Your description of the changes"
   ```
3. **Push your changes** (instantly uploads the edits to GitHub):
   ```bash
   git push origin main
   ```
   *(Note: Replace `main` with `master` if your branch is master).*

---

## Tips & Troubleshooting

* **Checking Status**: Run `git status` at any point to see which files have been modified.
* **Authentication**: The first time you run `git push`, a window will pop up asking you to sign in to GitHub to authorize the upload. Just log in through that window.
