# dogan.education, full site

A four-page profile site: about, teaching, research, software. Plain HTML with one
shared stylesheet. No build step, no dependencies.

```
index.html      About
teaching.html   Courses
research.html   Teaching After the Feed and the course design workshop
software.html   classroomtools.io, apps, and the GitHub repository index
style.css       Shared styles (light and dark)
```

## Deploying

Point any static host at this directory.

- **Vercel:** import the repository and set the root directory to `site/`.
- **Netlify:** set the publish directory to `site/`.
- **Anything else:** upload the five files as they are.

The single-page site that GitHub Pages serves at dogan.education lives in the
repository root and is not affected by this directory.

## Editing

Each page is one HTML file. To add a project, copy an `<li>` inside the relevant
section and change the link and text. To use a photo instead of the "DA" monogram
on the home page, replace the `<div class="avatar">DA</div>` with
`<img class="avatar" src="portrait.jpg" alt="Doğan Arslanoğlu" />` and drop a
`portrait.jpg` in this folder.
