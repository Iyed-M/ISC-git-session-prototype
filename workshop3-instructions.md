# Mission 3 — Share Your Work on GitHub

**Learn:** `git push`, Pull Requests, merge, `git pull`

### Instructions

1. Make sure you're on the branch created in Workshop 2.

   `git branch --show-current`

2. Push your branch to GitHub.

   `git push -u origin feature/favorite-programming-language`

3. Open your repository on GitHub.

4. Click **Compare & pull request** to create a Pull Request from `feature/favorite-programming-language` into `main`.

5. Give your Pull Request a title:

   `Add favorite programming language`

6. Open the **Files changed** tab and review your modifications.

7. Click **Merge pull request**, then confirm the merge.

8. Return to your terminal and switch to `main`.

   `git switch main`

9. Download and integrate the latest changes from GitHub.

   `git pull`

10. Open `README.md` and verify that your favorite programming language now appears on `main`.

### Questions

- What's the difference between `git commit` and `git push`?
- Why do we create a Pull Request instead of immediately modifying `main`?
- Why did we need `git pull` after merging on GitHub?
