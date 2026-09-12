# Contributing to WorldRun

Thanks for your interest in contributing! This guide is meant to be simple and beginner-friendly.

## 1) Find an issue

1. Go to the [Issues](https://github.com/jv-ransika/WorldRun/issues) page.
2. Start with issues labeled `good first issue` or `help wanted` when available.
3. Read the full issue description before you start.

Tip: If no issue looks like a fit, open a new issue with your idea before writing code.

## 2) Claim an issue

To avoid duplicate work, leave a comment on the issue like:

> I’d like to work on this.

If someone is already assigned or actively working on it, pick a different issue (or ask if collaboration is welcome).

## 3) Fork and clone

1. Fork this repository to your GitHub account.
2. Clone your fork locally:

```bash
git clone https://github.com/<your-username>/WorldRun.git
cd WorldRun
```

3. (Recommended) Add the main repository as `upstream` so you can sync later:

```bash
git remote add upstream https://github.com/jv-ransika/WorldRun.git
```

## 4) Create a branch

Create a new branch from the latest `dev` branch:

```bash
git checkout dev
git pull upstream dev
git checkout -b <branch-name>
```

`main` is the stable branch. Use `dev` for active contribution work unless a maintainer asks for a different target branch.

### Branch naming convention

Use short, descriptive names:

- `feat/<issue-number>-short-description`
- `fix/<issue-number>-short-description`
- `docs/<issue-number>-short-description`
- `chore/<issue-number>-short-description`

Example: `docs/4-finalize-contributing-guide`

## 5) Keep pull requests small and focused

Please keep each PR focused on one issue or one clear problem.

- ✅ Good: one feature, one bug fix, or one docs improvement
- ❌ Avoid: mixed unrelated changes in the same PR

Smaller PRs are easier to review and merge quickly.

## 6) Commit message guidance

Write clear commit messages in the imperative style (what the commit does).

- `docs: finalize CONTRIBUTING.md`
- `fix: handle empty world-state update`
- `feat: add basic entity movement endpoint`

If useful, include the issue number in the body:

```text
Closes #<issue-number>
```

## 7) Testing expectations

Before opening a PR:

- Run relevant tests for the area you changed.
- If you changed behavior, add or update tests when test infrastructure exists.
- If no automated tests exist yet for that area, include clear manual verification steps in your PR description.

Do not submit changes that you have not verified.

## 8) Open a pull request

When your branch is ready:

1. Push your branch to your fork.
2. Open a PR against `jv-ransika/WorldRun:dev`.
3. Reference the issue (for example: `Closes #4`).
4. Add a clear summary:
   - what changed
   - why it changed
   - how you tested it

## 9) Screenshots or recordings

Include screenshots or short recordings when your change affects:

- UI/visual output
- animation or simulation behavior visible in the frontend
- anything where visual confirmation helps reviewers

For backend-only or docs-only changes, screenshots are usually not needed.

## 10) Where to ask questions

If you are unsure, ask early:

- Comment on the issue you are working on
- Open a new issue with a clear question

Maintainers would rather answer early questions than review work that goes in the wrong direction.

## Project context

Before larger contributions, read:

- [README.md](README.md)
- [docs/PROJECT_PRINCIPLES.md](docs/PROJECT_PRINCIPLES.md)

These documents explain the project direction and current non-goals.
