# Contributing

This is a practice repo: the goal is to walk through a real contribution,
start to finish. Follow these steps exactly once, then you'll know the
workflow for every other open source project.

## The exercise

Add your name to [CONTRIBUTORS.md](CONTRIBUTORS.md) by opening a pull request.

## Step by step

1. **Fork this repo.** Click "Fork" at the top of the GitHub page. This makes
   your own copy under your account.

2. **Clone your fork** to your machine (replace `YOUR-USERNAME`):
   ```bash
   git clone https://github.com/YOUR-USERNAME/first-oss-contribution.git
   cd first-oss-contribution
   ```

3. **Create a branch** for your change — never commit directly to `main`:
   ```bash
   git checkout -b add-my-name
   ```

4. **Edit `CONTRIBUTORS.md`** and add one line at the bottom of the list, in
   this exact format:
   ```markdown
   - [Your Name](https://github.com/your-handle) - short intro (school, interests, whatever)
   ```
   Only add your line. Don't edit or remove anyone else's.

5. **Commit your change:**
   ```bash
   git add CONTRIBUTORS.md
   git commit -m "Add [Your Name] to contributors"
   ```

6. **Push your branch:**
   ```bash
   git push origin add-my-name
   ```

7. **Open a pull request** on GitHub: go to your fork, click "Compare & pull
   request", and submit it against this repo's `main` branch.

## What happens next

- A bot will comment welcoming you — that's normal, not spam.
- An automated check verifies your change only touches `CONTRIBUTORS.md`, only
  adds a line (doesn't change existing ones), and matches the required format.
- If everything checks out, your PR merges automatically. If not, you'll get a
  comment explaining what to fix, and a maintainer will follow up.

Once merged, your name is permanently in this repo's history. That's a real
open source contribution — congratulations.

Want to keep going? See [docs/finding-your-first-issue.md](docs/finding-your-first-issue.md)
for how to find a real project to contribute to next.
