# Portfolio - Abdel Moujib Begdouri Terraf

Static one-page portfolio, deployed to GitHub Pages from `master`.

## Structure

```
index.html                          main page (must stay at the root for GitHub Pages)
projects/
  education-dashboard.html          case study: Dashboard for Educational Equality
  clustering-dashboard.html         interactive clustering dashboard linked from the case study
assets/img/
  profile/                          portrait
  logos/                            company / project logos and the Mini Me chat avatar
  projects/<project>/               cover image and figures for each project
  archive/                          images not used by any page (kept for later)
.github/workflows/                  deployment (deploy.yml injects the Gemini key for Mini Me)
```

## Adding a project

1. Put its images in `assets/img/projects/<project-name>/`.
2. Add a `<div class="project reveal">` card in the `#projects` section of `index.html`.
   A `.cover` without an `<img>` shows its text as a placeholder.
3. Add the project to the Mini Me knowledge base (`PROJECTS` in the chat script) so the assistant can answer about it.

Use forward slashes in paths: backslashes break on GitHub Pages.
