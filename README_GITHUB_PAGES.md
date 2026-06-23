# Publish on GitHub Pages

This folder is ready to publish as a static site.

## Files to upload

- `index.html`
- `CNAME`
- `assets/mockup-60-power-licks-infos.jpg`
- `assets/roger-benet-live.jpg`

## GitHub Pages setup

1. Create a new GitHub repository, for example `60-power-licks-landing`.
2. Upload the files from this folder to the repository root.
3. In GitHub, open `Settings` > `Pages`.
4. Under `Build and deployment`, choose `Deploy from a branch`.
5. Select the `main` branch and `/root`, then save.
6. In `Custom domain`, enter `us.rogerbenet.com`.
7. In your domain DNS, point only the `us` subdomain to GitHub Pages.

## DNS record for the subdomain

Create this `CNAME` record:

```txt
Type: CNAME
Name/Host: us
Target/Points to: YOUR-GITHUB-USERNAME.github.io
```

Replace `YOUR-GITHUB-USERNAME` with your exact GitHub username.

Do not change the root records for `rogerbenet.com` if Hotmart is currently serving
`rogerbenet.com/60powerlicks` and `rogerbenet.com/10powerlicks`.
