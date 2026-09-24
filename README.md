# Sadman Shawraz — personal research website

A responsive, static website for GitHub Pages. No installation, build step, JavaScript, external fonts, or third-party assets are required.

## Preview
Open `index.html` in a browser. For a local server, run `python3 -m http.server 8000` inside this folder, then visit http://localhost:8000.

## Publish to the existing GitHub Pages repository
1. Keep a backup or branch of the current repository.
2. Copy the **contents** of this folder into the root of `shawraz.github.io`, replacing `index.html` and `README.md`. Include `thoughts.html`, `assets/`, `CNAME`, `.nojekyll`, `robots.txt`, and `sitemap.xml`.
3. Commit the files to the branch already used by GitHub Pages. The existing `CNAME` is preserved as `shawraz.com`; the redesign does not require DNS changes.
4. Check the repository's Pages deployment, then open https://shawraz.com and test the Thoughts page and résumé link.

The old CSS, JavaScript, and images are no longer referenced and may remain in the repository. Existing GitHub Actions workflows, if any, should be preserved. This deliverable has not been deployed.

## Edit content
- `index.html`: introduction, research, contributions, publications, education, and contact details.
- `thoughts.html`: your future writing page.
- `assets/style.css`: colors (at the top), typography, layouts, mobile styles, and print styles.
- `assets/llama.svg`: original vector llama illustration; editable without image software.
- `assets/Sadman-Shawraz-Resume.pdf`: supplied 2026 résumé, linked for viewing and download. This original PDF includes your phone number and location. Replace the file with a public-facing version if desired.

All content is plain HTML and can be edited directly using GitHub's file editor. Change the footer year as needed. The contact link opens the visitor's email app; it does not use a form service.

## Add your first thought
In `thoughts.html`, replace the entire `<section class="empty-notebook" ...>...</section>` with an article like this. Duplicate the article for future notes, newest first; use unique IDs and real publication dates. Example placeholders below are editing instructions and are not published on the site.

```html
<article class="thought-entry" id="your-note-slug">
  <time datetime="2026-09-24">September 24, 2026</time>
  <h2>Your title</h2>
  <p>Your opening thought goes here.</p>
  <p>Continue your writing here.</p>
</article>
```

## Content sources and editorial decisions
- Main source: the supplied `Resume_2026_Sadman_Shawraz.pdf`; research summaries are paraphrased, with no invented experimental outcomes or performance claims.
- Current nanobody work is presented as ongoing, synthetic, and animal-free. The llama is a conceptual illustration, not an experimental diagram.
- PNAS article verified against https://pubmed.ncbi.nlm.nih.gov/41481458/ and linked at https://doi.org/10.1073/pnas.2527869123.
- Cell Reports article verified against the final-publication update at https://pubmed.ncbi.nlm.nih.gov/40747431/ and the lab publication list https://www.bieniasz-hatziioannou.org/publications; linked at https://doi.org/10.1016/j.celrep.2025.116142.
- The RHAU manuscript remains explicitly in preparation, following the résumé; it is not counted as a published article.
- The Thoughts page has an honest empty state rather than invented writing.

## Accessibility and maintenance
Semantic landmarks, a skip link, visible keyboard focus, descriptive links, native keyboard-accessible contribution disclosures, scalable text, reduced-motion support, and mobile layouts are included. Content and navigation work without JavaScript. No tracking or analytics are installed.

## Verification
Source checks passed for internal links and fragment targets, referenced assets, image alt text, unique IDs, and page landmarks. Main text color pairs meet WCAG AA contrast (4.72:1 or higher). Responsive layouts are included, but browser rendering and keyboard interaction could not be tested in this environment: the local preview was blocked by browser security. Review the site on a desktop and phone before publishing.
