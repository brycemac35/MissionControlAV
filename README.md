# Mission Control AV — Website

Simple static site: `index.html` + `assets/logo-mark.svg`. No build step, no dependencies to install.

## Before you publish

Open `index.html` and update the placeholder contact details (search for these):
- `hello@missioncontrolav.ca` → your real email (appears twice)
- `+16045550142` / `(604) 555-0142` → your real phone number (appears twice)
- Domain, if you buy one, and the license/WorkSafeBC line in the footer once that's official

## Host it free on GitHub Pages

1. Create a new repo on GitHub, e.g. `missioncontrolav`.
2. Upload `index.html` and the `assets/` folder to the repo root (drag-and-drop on the GitHub web UI works fine, or `git push` if you're comfortable with git).
3. In the repo, go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Set **Branch** to `main` and folder to `/ (root)`, then **Save**.
6. Wait ~1 minute — GitHub will give you a live URL like `https://yourusername.github.io/missioncontrolav/`.

## Custom domain (optional)

If you buy a domain (e.g. missioncontrolav.ca):
1. In **Settings → Pages**, enter it under **Custom domain**.
2. At your domain registrar, add a `CNAME` record pointing to `yourusername.github.io`.
3. GitHub Pages will auto-provision HTTPS after DNS propagates (can take a few hours).

## Making the contact form actually work later

Right now "Request a Quote" and the footer email are `mailto:` links — they open the visitor's email app, no backend needed. If you later want an on-page form that emails you directly, a free service like Formspree or Web3Forms drops in with no server required — let me know when you're ready and I can wire it in.
