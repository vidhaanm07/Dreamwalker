# Push this to GitHub

## Option A: GitHub CLI (fastest)

```bash
cd dreamwalker
git init -b main
git add .
git commit -m "Initial commit: Dreamwalker 3D"
gh repo create dreamwalker --public --source=. --remote=origin --push
```

Then open **Settings → Pages**, set Source to **GitHub Actions**. The game goes live at
`https://<your-username>.github.io/dreamwalker/` within a minute or two.

## Option B: Plain git

1. Create an empty repo named `dreamwalker` on github.com (no README, no license).
2. Run:

```bash
cd dreamwalker
git init -b main
git add .
git commit -m "Initial commit: Dreamwalker 3D"
git remote add origin https://github.com/<your-username>/dreamwalker.git
git push -u origin main
```

3. **Settings → Pages → Source: GitHub Actions.**

## Option C: No command line

1. Create a new repo on github.com.
2. Click **Add file → Upload files** and drag in everything from this folder
   (including the `.github` folder).
3. Commit, then enable **Settings → Pages → Source: GitHub Actions**.

## Before you publish

- Replace `YOUR NAME` in `LICENSE`.
- Replace `<your-username>` in `README.md`.
