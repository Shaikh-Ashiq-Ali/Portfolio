# Portfolio

Personal portfolio of **Ashiq Ali Shaikh**, a PHP full stack and MERN developer.

**Live:** https://shaikh-ashiq-ali.github.io/Portfolio/

## Stack

Plain HTML, CSS and JavaScript, with no build step and no framework. The rotating 3D shape in the About section uses [three.js](https://threejs.org/), loaded from a CDN.

## Files

| Path | What it is |
|------|------------|
| `index.html` | The whole site: markup, the content data (skills, experience, projects) and the scripts |
| `styles.css` | Nocturne design-system tokens and component classes (colors, type, buttons, cards, tags, dialog) |
| `uploads/` | Profile photo and `resume.pdf`, which the Resume buttons download |

## Editing content

Skills, experience and projects are arrays near the top of the `<script>` in `index.html` (`skillGroups`, `experience`, `projects`). Edit them there and the sections re-render from that data.

A project `details` entry written as `Heading::text` shows a bold heading before the text.

## Run locally

Serve the folder over HTTP. Opening the file directly won't run the module script.

```
python -m http.server 8000
```

Then open http://localhost:8000.

## Deploy

GitHub Pages deploys from the `main` branch, `/ (root)` folder. Pushing to `main` updates the live site.

Pages runs Jekyll by default, and Jekyll leaves out any file or folder whose name starts with `_`. Don't give the site's files or folders names starting with `_`, or add an empty `.nojekyll` file to the repo root.
