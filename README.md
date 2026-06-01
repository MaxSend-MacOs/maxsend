# MaxSend website (GitHub Pages)

Static site for marketing, App Store URLs, and legal pages.

## Pages

| File | URL path | Use in App Store Connect |
|------|----------|---------------------------|
| `index.html` | `/` | Marketing URL (optional) |
| `privacy.html` | `/privacy.html` | **Privacy Policy URL** (required) |
| `terms.html` | `/terms.html` | Reference / support |
| `support.html` | `/support.html` | **Support URL** (required) |

## Publish on GitHub Pages

### Option A — Same repo (`MAXSEND`), `/docs` folder

1. Push the `docs/` folder to GitHub.
2. Repo **Settings → Pages**.
3. **Build and deployment → Source:** Deploy from a branch.
4. **Branch:** `main` (or your default branch), **Folder:** `/docs`.
5. Save. Site goes live at:

   `https://<username>.github.io/MAXSEND/`

### Option B — Dedicated repo (e.g. `maxsend`)

Copy the contents of `docs/` to the root of a new repo named `maxsend.github.io` or any repo with Pages enabled. Then URLs are:

`https://<username>.github.io/maxsend/`

## App Store Connect URLs

After publishing, use (replace with your real GitHub username and repo name):

- **Privacy Policy URL:** `https://<username>.github.io/MAXSEND/privacy.html`
- **Support URL:** `https://<username>.github.io/MAXSEND/support.html`
- **Marketing URL:** `https://<username>.github.io/MAXSEND/`

## Before you go live

1. Replace `support@codewithik.com` in `support.html` with your real support email.
2. Update the App Store link in `index.html` when your app is approved (`https://apps.apple.com/app/idXXXXXXXX`).
3. Preview locally: open `index.html` in a browser, or run `python3 -m http.server 8080` inside `docs/`.

## Design

Purple accent matches the MaxSend app theme. No build step required—plain HTML and CSS.
