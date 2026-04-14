# Cursor global rules (shared)

This repository holds **Cursor project rules** you can reuse on every machine and every repo.

## Use in Cursor (recommended)

1. Open **Cursor Settings** → **Rules, Commands**.
2. Under **Project Rules**, click **+ Add Rule** → **Remote rule (GitHub)**.
3. Paste this repository URL (after you push it to GitHub):

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
