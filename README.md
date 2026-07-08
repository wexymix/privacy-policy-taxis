# Privacy Policy (GitHub Pages)

This repository contains a minimal privacy policy page intended to be published via GitHub Pages.

How to publish as a private repo and get a URL

1. Create a new private repository on GitHub (for example, `privacy-policy-<app>`).
2. From this folder, initialize git, add files and push:

```bash
cd privacy-policy-github
git init
git add .
git commit -m "Add privacy policy page"
git branch -M main
git remote add origin git@github.com:YOUR_USERNAME/REPO_NAME.git
git push -u origin main
```

3. On GitHub, go to the repository Settings → Pages and choose the `main` branch (root) as source. Save.

4. The published URL will usually be:

- For a user/org project site: `https://YOUR_USERNAME.github.io/REPO_NAME/`

Notes:
- GitHub Pages sites are public by URL even if the repository is private in some account plans; verify access settings.
- Alternatively you can use the `gh` CLI to create a private repo and push in one step:

```bash
gh repo create REPO_NAME --private --source=. --remote=origin --push
gh pages enable --branch main --path /
```

Replace `YOUR_USERNAME` and `REPO_NAME` with your values.
