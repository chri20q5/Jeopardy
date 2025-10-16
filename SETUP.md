# 🚀 GitHub Setup Guide

Quick guide to get your HTW Jeopardy game on GitHub!

## 📦 Publishing to GitHub (Private Repository)

### Step 1: Create Repository on GitHub

1. Go to [github.com](https://github.com) and log in
2. Click the **"+"** icon (top right) → **"New repository"**
3. Fill in:
   - **Repository name**: `htw-jeopardy` (or your preferred name)
   - **Description**: "A modern browser-based Jeopardy game with dual-screen support"
   - **Visibility**: ✅ **Private** (check this!)
   - **Initialize**: Leave unchecked (we already have files)
4. Click **"Create repository"**

### Step 2: Push Your Code

Open terminal in the `/home/chri20q5/scripts/Jeopardy` folder and run:

```bash
# Initialize git repository
git init

# Add all files
git add .

# Create first commit
git commit -m "Initial commit: HTW Jeopardy game"

# Add your GitHub repository as remote
# Replace YOUR_USERNAME and YOUR_REPO with your actual values
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Verify

Go to your GitHub repository page - you should see all your files!

---

## 🌐 Optional: Enable GitHub Pages (Make it Live!)

If you want to host it online so others can access via URL:

1. Go to your repository on GitHub
2. Click **Settings** → **Pages** (left sidebar)
3. Under "Source":
   - Branch: `main`
   - Folder: `/ (root)`
4. Click **Save**
5. Wait 1-2 minutes
6. Your game will be live at: `https://YOUR_USERNAME.github.io/YOUR_REPO/`

**Note:** GitHub Pages works even for private repos, but the site itself will be public. If you want truly private, skip this step and just share the files directly.

---

## 👥 Sharing with Others

### Option A: Add Collaborators (Private Repo)
1. Repository → **Settings** → **Collaborators**
2. Click **"Add people"**
3. Enter their GitHub username
4. They can now clone and access the repo

### Option B: Share Files Directly
1. Download `index.html` and `display.html` from your repo
2. Send via email, Dropbox, Google Drive, etc.
3. They just open `index.html` - no GitHub needed!

### Option C: Share via GitHub Pages
If you enabled Pages:
- Just share the URL: `https://YOUR_USERNAME.github.io/YOUR_REPO/`
- Anyone with the link can use it

---

## 🔄 Making Updates

After making changes to your files:

```bash
# Check what changed
git status

# Add changes
git add .

# Commit with a message
git commit -m "Description of what you changed"

# Push to GitHub
git push
```

---

## 📥 Cloning Your Repo (On Another Computer)

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/YOUR_REPO.git

# Navigate into folder
cd YOUR_REPO

# Open index.html in browser - you're ready to play!
```

---

## 🎯 Quick Commands Reference

```bash
# Check status
git status

# Add all changes
git add .

# Commit changes
git commit -m "Your message here"

# Push to GitHub
git push

# Pull latest changes
git pull

# View commit history
git log --oneline
```

---

## 🐛 Common Issues

### "Permission denied" when pushing
- Make sure you're logged into GitHub
- You might need to set up SSH keys or use Personal Access Token

### "Updates were rejected"
Someone else made changes. Pull first:
```bash
git pull
git push
```

### "Pop-up blocked" when using GitHub Pages
- Users need to allow pop-ups for your site
- Or manually open `display.html` in a new window

---

## 💡 Pro Tips

1. **Commit often** - Small, frequent commits are better
2. **Write clear commit messages** - Future you will thank you
3. **Use branches** for experimental features (optional)
4. **Tag releases** - Use `git tag v1.0.0` for versions

---

Need help? Check [GitHub's documentation](https://docs.github.com/) or open an issue in your repo!
