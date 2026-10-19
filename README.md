# GitHub Pages — WhisperMobile alpha landing page

1. Upload `index.html` and `site-config.js` to a GitHub repository, at its Pages publishing root.
2. Edit `site-config.js` so `WHISPERMOBILE_PORTAL_URL` points to `https://YOUR-WINDOWS-SERVER-HOST/alpha/`.
3. Enable Pages in repository settings and enforce HTTPS.
4. Do NOT publish server configuration, database, passwords, private account data, model files or secret keys to GitHub.

GitHub Pages hosts **only a static landing page**. For account creation and login, the visitor is directed to the professionally styled matching portal served by the Windows server through Caddy. This is intentional: GitHub Pages documentation discourages handling passwords and other sensitive transactions on Pages, and also prohibits commercial SaaS hosting. The actual alpha account database stays in SQLite on the Windows PC.
