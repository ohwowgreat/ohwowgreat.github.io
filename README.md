# dogan.education

Personal site for Doğan Arslanoğlu: about, teaching, research, and software, with
links to projects and their repositories.

Live at **[dogan.education](https://dogan.education)** (and at
[ohwowgreat.github.io](https://ohwowgreat.github.io)), served by GitHub Pages.

## Structure

```
index.html      About
teaching.html   Courses
research.html   Teaching After the Feed and the course design workshop
software.html   classroomtools.io, apps, and the repository index
style.css       Shared styles (light and dark)
```

Plain HTML with one shared stylesheet. No build step and no dependencies. Edit,
commit, and push; GitHub Pages redeploys automatically.

## Editing

- **Add a project:** copy an `<li>` inside the relevant section of
  [`software.html`](software.html) and change the link and text.
- **Bio:** the three paragraphs at the top of [`index.html`](index.html).
- **Use a photo instead of the "DA" monogram:** in `index.html`, replace the
  `<div class="avatar">DA</div>` with
  `<img class="avatar" src="portrait.jpg" alt="Doğan Arslanoğlu" />` and drop a
  `portrait.jpg` in this folder.
- **Colors and type:** the variables at the top of [`style.css`](style.css).

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

Then, in the repo's **Settings → Pages**, confirm the custom domain is `dogan.education`
and enable **Enforce HTTPS** once the certificate is issued (can take a few minutes to an hour).
