# dogan.education

Personal homepage for Doğan Arslanoğlu — a single, self-contained page linking to
educational projects, research, and classroom tools.

Live at **[dogan.education](https://dogan.education)** (and at
[ohwowgreat.github.io](https://ohwowgreat.github.io)), served by GitHub Pages.

## Editing

Everything is in [`index.html`](index.html) — one file, inline CSS, no build step.
Edit it, commit, and push; GitHub Pages redeploys automatically.

- **Add a project:** copy an `<li>` inside the relevant `<section>` and change the link + text.
- **Use a photo instead of the “DA” monogram:** replace the `<div class="avatar">DA</div>`
  with `<img class="avatar" src="portrait.jpg" alt="Doğan Arslanoğlu" />` and drop a
  `portrait.jpg` in this folder.
- **Bio / role line:** edit the `.intro` paragraph and the `.role` line near the top.

## Custom domain (dogan.education)

The [`CNAME`](CNAME) file tells GitHub Pages to serve the site at `dogan.education`.
For it to resolve, add these DNS records at your domain registrar:

| Type  | Name  | Value                       |
|-------|-------|-----------------------------|
| A     | @     | 185.199.108.153             |
| A     | @     | 185.199.109.153             |
| A     | @     | 185.199.110.153             |
| A     | @     | 185.199.111.153             |
| CNAME | www   | ohwowgreat.github.io        |

Then, in the repo’s **Settings → Pages**, confirm the custom domain is `dogan.education`
and enable **Enforce HTTPS** once the certificate is issued (can take a few minutes to an hour).
