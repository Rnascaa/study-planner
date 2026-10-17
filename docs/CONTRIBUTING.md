# Contributing Guide

Thanks for taking the time to contribute! This guide explains how we write commits, name branches, and ship changes, so the project history stays clean and easy to follow.

## Table of Contents

- [Commit Messages](#-commit-messages)
- [Branch Naming](#-branch-naming)
- [Workflow Per Issue](#-workflow-per-issue)
- [Pull Request Rules](#-pull-request-rules)
- [Quick Checklist](#-quick-checklist)

---

## Commit Messages

We follow the [Conventional Commits](https://www.conventionalcommits.org/) specification.

**Format:**

```
type: short description
```

| Prefix      | Use for                                   |
| ----------- | ----------------------------------------- |
| `feat:`     | A new feature                             |
| `fix:`      | A bug fix                                 |
| `docs:`     | Documentation changes, README             |
| `chore:`    | Setup, configuration, routine tasks       |
| `refactor:` | Code cleanup without changing behavior    |
| `test:`     | Adding or fixing tests                    |
| `style:`    | Code formatting only, no logic changes    |

**Examples:**

```
feat: add user registration endpoint
fix: handle expired JWT token
docs: add research summary
chore: set up docker configuration
```

> **Tip:** Write all commit messages in **English** and keep the description short, lowercase, and in the imperative mood (e.g. "add", not "added").

---

## Branch Naming

> **Never commit directly to `main`.**
> One issue = one branch.

**Format:**

```
type/short-description
```

Use the same `type` prefixes as commit messages, and separate words with hyphens.

**Examples:**

```
feat/auth-jwt
docs/research-summary
chore/docker-setup
```

---

## Workflow Per Issue

### 1. Start from an up-to-date `main`

```bash
git checkout main
git pull
git checkout -b docs/research-summary
```

### 2. Do the work, then commit and push

```bash
git add .
git commit -m "docs: add research summary"
git push -u origin docs/research-summary
```

### 3. Open a Pull Request

1. Go to the repository on GitHub.
2. Click **Compare & pull request**.
3. In the PR description, write `Closes #1` (use the number of the issue you are working on).
4. Submit the PR.

### 4. Merge

Choose **Squash and merge** to keep the `main` history tidy.

When the PR is merged:

- ✅ The linked issue is closed automatically.
- ✅ Its card on the project board moves to **Done**.

---

## Pull Request Rules

- The PR title follows the commit format, e.g. `feat: add user registration endpoint`.
- The description includes `Closes #<issue-number>`.
- One PR should address one issue only.
- Keep PRs small and focused so they are easy to review.

---

## ✅ Quick Checklist

Before opening a PR, make sure that:

- [ ] I branched from the latest `main`
- [ ] My branch name follows `type/short-description`
- [ ] My commit messages follow Conventional Commits
- [ ] My PR description contains `Closes #<issue-number>`
- [ ] My changes are limited to a single issue