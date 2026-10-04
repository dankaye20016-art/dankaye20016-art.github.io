# Dan Kaye portfolio site

Static engineering portfolio for Dan Kaye (Penn MEAM, class of 2030), hosted on GitHub Pages at https://dankaye20016-art.github.io from the `main` branch root. Plain HTML and CSS, no build step, no framework. `.nojekyll` turns off Jekyll processing.

## Structure

- `index.html`: homepage. One large image per project, each with a caption row (title, one factual line, years). Links to the project page.
- `projects/*.html`: one page per project. Layout: back link, h1, one-sentence lede, facts row (`dl.facts`), hero image, then prose sections in the order problem → decisions → result → what changed. Images go in `figure.figure` (single) or `div.pair` (two side by side). Ends with a `nav.next` linking previous and next projects.
- `about.html`: short bio, skills, competitions and leadership list.
- `assets/site.css`: all styles. Light-only on purpose: every image has a white background so parts appear to float.
- `assets/img/<project>/`: images, trimmed to the part with a small white margin.

## Design rules (from Dan's feedback)

- Images are the emphasis: large, on pure white, no tinted boxes, borders or cards.
- Plain header: name, "Mechanical Engineering, University of Pennsylvania", nav links. No taglines or slogans.
- No status badges or marketing labels. Captions are factual.
- Restraint: one sans (Geist), Geist Mono only for small metadata.

## Content rules

- Confident, plain language. Never invent facts, numbers, tests or processes Dan hasn't confirmed.
- Say what Dan personally owned on team projects.
- The ball joints on BikePack anchors are purchased clamps; don't imply he designed them.
- Walter P Moore work is cleared for the portfolio. Describe it as modeling and documentation, not structural design.
- Penn Electric Racing work is not on the site yet; check with Dan before adding anything, since the team may limit what can be posted.

## Adding a project

1. Trim images to a white background and put them in `assets/img/<project>/`.
2. Copy an existing page in `projects/`, replace the text and images, and update the `nav.next` links on the neighboring pages.
3. Add a `work-item` block to `index.html` in the right order.

## Pending

- Resume PDF and contact email (Dan to provide); a Resume link goes in the nav once the PDF exists.
- Higher-resolution renders (at least 1920 px wide) to replace the current ~750 px ones.
- Drone: what caused the ESC failure and what Dan would change.
- BikePack: slider animation loop.
- Penn Electric Racing project page.
