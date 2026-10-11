# Workshop 1 — Your First Git Checkpoint

**Mission:** Complete your ISC team profile and save your first changes with Git.

**You will learn:** repository, `git clone`, `git status`, `git add`, `git commit`, `git log`.

**Estimated time:** 15 minutes · Work in pairs.

## 1. Get your own repository

1. Open the ISC workshop template link provided by the organizers.
2. Click **Use this template → Create a new repository**. Give it a name such as `isc-team-profile` and create it under your own GitHub account.
3. On your repository's GitHub page, click **Code → HTTPS** and copy the repository URL.
4. Open a terminal and run:

   ```bash
   git clone <your-repository-url>
   cd isc-team-profile
   ```

   Replace `<your-repository-url>` with the URL you copied. If you chose another repository name, use that name after `cd`.

**Why?** `git clone` downloads a copy of your GitHub repository onto your computer, including its Git history.

## 2. Make your first change

Open `README.md` in your editor and:

- Replace `??????? ????` with `Systems Club` (don't duplicate `Intelligent`).
- Replace the `???` entries under **Members** with your names.
- Save the file.

**Why?** Your working files have changed, but Git hasn't saved a checkpoint yet.

## 3. See what Git noticed

```bash
git status
```

**Look for:** `README.md` listed as modified.

**Why?** `git status` shows which files have changed and whether they're staged for a commit.

## 4. Stage and commit

```bash
git add README.md
git status
git commit -m "Complete ISC information"
```

- `git add README.md` selects the current README changes for the next commit (staging).
- The second `git status` shows the README under **Changes to be committed**.
- `git commit -m "..."` records a checkpoint in your **local** Git history. The quoted text describes what you changed.

If Git asks who you are, ask an organizer to help you set `user.name` and `user.email`, then retry the commit.

## 5. Check your result

```bash
git status
git log --oneline
```

**Look for:** a clean working tree and a new history entry titled `Complete ISC information`.

## Quick questions

1. What is the difference between `git add` and `git commit`?
2. Is your new commit already on GitHub? **No — not until you push it.**

**Mission complete when:** your README contains your team's names and `git log --oneline` shows your commit.
