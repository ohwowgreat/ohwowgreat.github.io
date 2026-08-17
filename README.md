# dogan.education

Personal site for Doğan Arslanoğlu: about, teaching, research, and software, with
links to projects and their repositories.

Live at **[dogan.education](https://dogan.education)** (and at
[ohwowgreat.github.io](https://ohwowgreat.github.io)), served by GitHub Pages.

## Structure

```
index.html      About, with overview tables for the three sections
teaching.html   Courses
research.html   Teaching After the Feed and the course design workshop
software.html   classroomtools.io, apps, and the repository index
style.css       Shared styles
```

Plain HTML with one shared stylesheet, in the visual language of
[classroomtools.io](https://classroomtools.io). No build step and no
dependencies. Edit, commit, and push; GitHub Pages redeploys automatically.

## Editing

Entries are table rows, not a data file. Each page repeats the top bar and the
sidebar, so a nav change has to be made in all four.

- **Add a project:** copy a `<tr>` inside the relevant `<table class="list">` in
  [`software.html`](software.html) and change the name, tagline, and status. The
  headline projects repeat in the Software table on [`index.html`](index.html);
  add it there too if it belongs on the front page.
- **Status dot:** `<span class="dot live">`, `dot testing`, or `dot dev`, with the
  matching word in the `state` span beside it. An entry with no public URL keeps
  its name as plain text instead of a link.
- **Bio:** the two paragraphs at the top of [`index.html`](index.html).
- **Courses:** each course is a `<section>` in [`teaching.html`](teaching.html)
  with an `id` that the front page links to.
- **Colors and type:** the top of [`style.css`](style.css).

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
