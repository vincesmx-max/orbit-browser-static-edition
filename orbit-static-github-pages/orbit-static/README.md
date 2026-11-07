# Orbit Browser — Static Edition

This version is designed for **GitHub Pages only**. It uses plain HTML, CSS, and standard browser JavaScript. There is no Node.js, backend server, database, build step, or package installation.

## Publish on GitHub Pages

1. Upload `index.html`, `styles.css`, `app.js`, and this README to the root of your GitHub repository.
2. Open **Settings → Pages**.
3. Under **Build and deployment**, choose **Deploy from a branch**.
4. Select branch `main` and folder `/(root)`, then save.
5. Wait for the Pages deployment. Your default address will look like `https://YOUR-USERNAME.github.io/REPOSITORY-NAME/`.

Do not enter a custom domain unless you own it and have configured its DNS. You do not need to buy a domain to use the GitHub Pages address.

## What works

- Responsive Orbit landing page and dark space theme
- Search/address field opens a URL or sends a search to Google in a new tab
- Quick links
- Add/remove bookmarks saved in this browser with `localStorage`
- Local display name and light/dark theme preference

## What changed / limitations

- There is no real account system. The local profile is only a display name stored in the current browser. It is not secure, does not sync, and can be cleared by the user.
- There is no admin dashboard or cross-user activity monitoring.
- There is no server-side proxy. Static GitHub Pages cannot fetch arbitrary websites as a secure proxy because of browser same-origin and CORS restrictions. The address field opens websites in a new tab instead.
- Data saved in `localStorage` stays in that browser/device and is not shared between users.

This project intentionally contains no Node.js, Express, SQLite, server code, or external dependencies.
