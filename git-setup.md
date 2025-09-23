# Git Installation & Setup Guide

This guide will help you install and configure **Git** on your system before the workshop.

---

## 🖥️ Step 1: Check if Git is already installed
```bash
git --version
```

---

## 💻 Step 2: Install Git

### Windows
1. Download Git from [git-scm.com](https://git-scm.com/download/win).
2. Run the installer and choose default settings.
3. Verify installation:
```bash
git --version
```

---

## ⚙️ Step 3: Configure Git
```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
git config --list
```

---

## 🔑 Step 4: Setup SSH Key (Recommended)
```bash
ssh-keygen -t ed25519 -C "your-email@example.com"
eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_ed25519
cat ~/.ssh/id_ed25519.pub
```
Then add the key in **GitHub → Settings → SSH and GPG keys**.

---

✅ You’re now ready to use Git with GitHub!
