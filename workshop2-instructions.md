# Workshop 2 — The Secret Branch

**Mission:** Add your favorite programming language without changing the `main` branch yet.

**You will learn:** branches, `git switch -c`, `git switch`, staging and committing on a branch.

**Estimated time:** 15 minutes · Continue in the same repository from Workshop 1.

## 1. Create a branch

In the terminal, make sure you're inside your `isc-team-profile` repository. Then run:

```bash
git switch -c feature/favorite-programming-language
```

**Why?** A branch lets you develop a change separately from `main`. `-c` means *create*; the command also switches you to that new branch.

Confirm where you are:

```bash
git branch --show-current
```

**Look for:** `feature/favorite-programming-language`.

## 2. Edit the README

Open `README.md`, add this section at the bottom, and replace the example with your own choice:

```markdown
## Favorite Programming Language

Python — because it is easy to start with!
```

If you haven't learned a language yet, choose one you're curious about. Save the file.

## 3. Record the change on your branch

```bash
git status
git add README.md
git commit -m "Add favorite programming language"
```

**Why?** This commit belongs to your feature branch. You haven't added it to `main`.

## 4. See the branch difference

**Before running the next command, predict:** will the new section stay visible in `README.md`?

```bash
git switch main
```

Open `README.md` again.

**Look for:** the favorite-language section is **not** present on `main`.

Now switch back:

```bash
git switch feature/favorite-programming-language
```

**Look for:** the section **reappears**. Your work was not deleted; it's saved on the feature branch.

## Quick questions

1. Why did the section disappear when you switched to `main`?
2. Was your feature commit deleted? **No — it remains in the feature branch's history.**
3. Is your branch on GitHub yet? **Not until you push it in Workshop 3.**

**Mission complete when:** you can switch between `main` and your feature branch and explain why the README changes.

**Keep the feature branch checked out at the end** — you'll push it during Workshop 3.
