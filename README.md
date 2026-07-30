# findtime.net

Static site: landing + the legal/support pages Apple and Google require for app review.

URLs the apps link to (must stay stable):

- `findtime.net/legal/privacy` → `legal/privacy.html`
- `findtime.net/legal/terms` → `legal/terms.html`
- `findtime.net/support` → `support.html`

## Deploy (GitHub Pages, free)

1. Push this folder as repo `findtime-site` (public), enable **Settings → Pages → Deploy from branch → main /(root)**.
2. Add file `CNAME` containing `findtime.net`.
3. At the DNS provider for findtime.net: `A` records for apex → GitHub Pages IPs (185.199.108.153, .109., .110., .111.) or `CNAME www → dog279.github.io` + apex ALIAS.
4. GitHub Pages serves extensionless URLs (`/legal/terms` → `legal/terms.html`) automatically.

Cloudflare Pages / Netlify work identically (drag-and-drop the folder).

Before review: create the `support@findtime.net` mailbox or alias — both legal pages and the
App Store support URL use it.
