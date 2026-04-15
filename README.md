# Cursor global rules (shared)

This repository holds **Cursor project rules** you can reuse on every machine and every repo.

## Use in Cursor (recommended)

1. Open **Cursor Settings** → **Rules, Commands**.
2. Under **Project Rules**, click **+ Add Rule** → **Remote rule (GitHub)**.
3. Paste this repository URL:

   `https://github.com/gilalmogy/cursor-global-rules`

4. Cursor syncs `.mdc` files under `.cursor/rules/` into `.cursor/rules/imported/` in each project.

You can add the same remote rule once per machine; Cursor keeps rules updated from Git.

## Clone into a project manually

If you prefer files on disk:

```powershell
git clone https://github.com/gilalmogy/cursor-global-rules.git
# Copy .cursor/rules/*.mdc into your project’s .cursor/rules/
```

## User Rules (global text)

For preferences that apply everywhere without importing a repo, open **Cursor Settings** → **Rules** → **User Rules** and paste the same workflow bullets, or keep them only in this repo and use **Remote rule** as above.

A copy also exists on disk at `%USERPROFILE%\.cursor\rules\git-milestone-backup.mdc` for reference; Cursor may still require **User Rules** or **Remote rule** in Settings for guaranteed global application.

## Publishing this repo (first time)

Requires GitHub authentication. Either run `gh auth login`, or set `GH_TOKEN` and run:

```powershell
gh repo create cursor-global-rules --public --source . --remote origin --push
```

If the repo already exists, add `origin` and `git push -u origin main`.
