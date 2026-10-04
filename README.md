# Wedding invitation

Create and share a personalised wedding invitation page.

- `Public/index.html` — form for creating or editing an invitation
- `Public/invite.html` + `Public/themes.css` — the shared invitation page, served at `/i/<link-name>`
- `netlify/functions/save.js` — `POST /api/save`, stores an invitation in Netlify Blobs
- `netlify/functions/get.js` — `GET /api/get?slug=...`, returns an invitation (without its edit token)
