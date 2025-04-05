# 🧠 Activity Keeper

Automated daily commits to keep that glorious GitHub contribution graph green. Because sometimes you're grinding off-platform... and GitHub doesn't need to know you're bingeing coffee and not code.

## 🔧 What It Does

- Runs a daily GitHub Actions workflow
- Updates a simple file (`last_update.txt`) with the current timestamp
- Commits and pushes it to this repo
- Keeps your contribution streak alive while you do... literally anything else

## 📅 Schedule

The workflow runs every day at **09:00 UTC**.

You can also trigger it manually using the `Run workflow` button in the Actions tab (for those "oops, I missed it" moments).

## 🤖 How It Works

- Uses GitHub Actions
- Runs a shell script to update a file
- Commits only if there are changes (avoids spamming)
- Pushes like a good little bot

## 🛠️ Setup (if you fork this)

1. Clone the repo
2. Edit `.github/workflows/daily-update.yml` to set your name/email:
    ```yaml
    git config --global user.name 'Your Name'
    git config --global user.email 'your-email@example.com'
    ```
3. Push and enable GitHub Actions

## 🙃 Why?

Because contribution graphs don't care *what* you commit—just *that* you commit.

---

> "If a commit falls in the forest and GitHub doesn't log it, did it even happen?" — Ancient Developer Proverb
