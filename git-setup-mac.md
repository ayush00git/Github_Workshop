# Git Installation & Setup Guide (macOS)

This guide will help you install and configure **Git** on macOS before the workshop.

---

## Step 1: Check if Git is already installed
```bash
git --version
````

If you see a version number, Git is already installed.

---

## Step 2: Install Git

### Option 1: Using Homebrew (Recommended)

Homebrew is a package manager for macOS. If you don’t already have it, install it first:

```bash
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
```

After installation, follow the instructions in the terminal to add Homebrew to your shell path.
For example, run:

```bash
echo 'eval "$(/opt/homebrew/bin/brew shellenv)"' >> ~/.zprofile
eval "$(/opt/homebrew/bin/brew shellenv)"
```

Now install Git:

```bash
brew install git
```

### Option 2: Using Xcode Command Line Tools

```bash
xcode-select --install
```

### Verify Installation

```bash
git --version
```

---

## Step 3: Configure Git

Set your username and email (used in commits):

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
git config --list
```

---

## Step 4: Setup SSH Key (Recommended)

### Generate SSH Key

```bash
ssh-keygen -t ed25519 -C "your-email@example.com"
```

Press **Enter** to accept defaults (saves to `~/.ssh/id_ed25519`).

### Start SSH Agent

```bash
eval "$(ssh-agent -s)"
```

### Add Key to Agent (with Keychain support)

```bash
ssh-add --apple-use-keychain ~/.ssh/id_ed25519
```

### Copy Public Key

```bash
cat ~/.ssh/id_ed25519.pub
```

Now go to **GitHub → Settings → SSH and GPG keys → New SSH key** and paste it.

---

✅ You’re now ready to use Git with GitHub on macOS!
