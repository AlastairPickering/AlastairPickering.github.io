# Alastair Pickering — homepage portrait v18

An editable Quarto website for an ecological research, software and professional portfolio.

## 1. Install Quarto

Download and install Quarto from:

https://quarto.org/docs/get-started/

Optional but recommended: edit the site in VS Code or RStudio.

## 2. Preview locally

Open a terminal in this folder and run:

```bash
quarto preview
```

Quarto will open a local preview and refresh it whenever you save a file.

## 3. Edit the content

The main files are:

- `index.qmd` — homepage
- `work.qmd` — selected portfolio
- `research.qmd` — research themes
- `software.qmd` — applications
- `publications.qmd` — publication list
- `experience.qmd` — scientific and business experience
- `about.qmd` — biography and contact
- `projects/` — individual case studies
- `styles.css` — visual styling
- `_quarto.yml` — navigation and site settings

Replace `images/profile-placeholder.svg` with a professional portrait, then change the image path in `about.qmd`.

## 4. Create the GitHub repository

The simplest permanent address is:

`AlastairPickering.github.io`

Create a public repository with that exact name, copy these files into it, and push to the `main` branch.

## 5. Publish

The included GitHub Action publishes the rendered site to the `gh-pages` branch whenever you push to `main`.

After the first successful action:

1. Open the repository on GitHub.
2. Go to **Settings → Pages**.
3. Choose **Deploy from a branch**.
4. Select the `gh-pages` branch and `/ (root)`.
5. Save.

The site should then appear at:

`https://alastairpickering.github.io`

## 6. Recommended first edits

1. Replace the profile placeholder.
2. Add one strong figure or screenshot to each project page.
3. Replace generic GitHub-profile links with direct repository links.
4. Add complete publication references and DOIs.
5. Check every Streamlit link while logged out.
6. Decide whether the public contact email should remain visible.
7. Add a downloadable two-page CV once it has been adapted for this audience.

## Privacy

The starter intentionally excludes the home address and mobile number shown in the supplied CV.


## Hero motion

The homepage currently uses four animated SVG scenes:

- `images/hero-forest.svg`
- `images/hero-elephant.svg`
- `images/hero-gibbon.svg`
- `images/hero-technology.svg`

They cross-fade and slowly scale using CSS, so the hero is animated immediately and does not rely on external assets.

These are intentionally temporary. For a photographic version, replace the hero with a compressed, muted video reel and retain one of the SVGs as the fallback image. A practical target is a 12–20 second, 1920×1080 MP4 kept below roughly 8–12 MB.


## Version 3 changes

- Replaced all generated illustrations with real photography.
- Rebuilt the homepage as one valid raw HTML block.
- Removed the nested Quarto fenced divs that produced `The following string was found in the document: :::` warnings.
- Added slow cross-fading and panning across forest, elephant, gibbon and computational imagery.
- Added `IMAGE-CREDITS.md`.


## Version 4 changes

- Replaced the design-brief wording with a proper homepage headline.
- Expanded the site to use up to 94% of the viewport and a maximum width of 1720px.
- Removed several small, cluttered homepage sections.
- Rebuilt the homepage around three large project features.
- Added real PAMalytics screenshots from the published documentation.
- Used PAMalytics itself as the computational hero scene instead of generic technology imagery.


## Version 5 corrections

- Removed the invalid nested `<main>` element.
- Neutralised Quarto's page-column grid on the homepage.
- Replaced viewport-only width calculations with one consistent centred frame.
- Removed all absolute positioning from PAMalytics screenshots.
- Replaced fixed 700–760px content heights with responsive aspect ratios.
- Reduced headline scaling and allowed all text blocks to grow naturally.
- Added explicit tablet and mobile stacking rules.


## Version 6 corrections

- Scoped the full-width Quarto overrides to the homepage only.
- Restored a centred 1280px content area for all inner pages.
- Removed Quarto's automatic page-title blocks.
- Retained the authored page headings such as “Selected work”.
- Added consistent desktop and mobile side margins.


## Version 7 correction

- Removed invalid `title: false` values from Quarto front matter.
- Retained automatic-title suppression through CSS.
- Kept a valid string title only where required by the About template.


## Version 8 correction

- Rebuilt the YAML front matter of every `.qmd` file explicitly.
- Restored valid string titles required by Quarto.
- Kept the generated title blocks hidden through CSS.
- Checked every page for both opening and closing YAML delimiters before packaging.


## Version 9 structure

The site now contains only:

- Home
- Research
- Experience
- Contact

Research and Experience use the same full-width visual system as the homepage and cover a broader proportion of the work. Contact consolidates email, LinkedIn, GitHub, Google Scholar and live applications.


## Version 10 changes

- Removed all headline statistics and quantitative business claims.
- Removed the forest-plot count from prominent copy.
- Rewrote the alva material in qualitative terms.
- Removed the homepage and Experience metric blocks entirely.


## Version 11 changes

- Removed language that framed ecology as a pivot away from alva.
- Made the shared methodological thread explicit across both careers.
- Reframed alva as an AI-led system for turning intangible signals into measurable, manageable evidence.
- Connected that directly to the ecological modelling and scientific software work.


## Version 12 changes

- Removed the explicit “consistent approach” label.
- Removed the company name from the principal positioning.
- Reframed the commercial background as fifteen years founding, scaling and exiting an AI analytics business.
- Connected that experience to the ecological work through the substance of the copy rather than an announced slogan.


## Version 13 changes

- Refined the Experience page to remove overly explicit or slogan-like wording.
- Reworked the commercial-to-research connection so it reads naturally rather than being announced.
- Reduced hero, section and card heading sizes across the site.
- Retained the existing layout and visual system.


## Version 14 changes

- Reduced homepage hero heading size.
- Reduced Research, Experience and Contact hero heading sizes.
- Left section and card headings unchanged.
- Tightened maximum hero text width for better balance.


## Version 15 changes

- Set all hero headings to a maximum of 3.5rem on desktop.
- Set all hero headings to a maximum of 2.8rem on mobile.
- Added explicit final CSS overrides so earlier rules cannot supersede these values.


## Version 16 changes

- Restored a full, named account of the alva career on the Experience page.
- Removed outdated quantitative claims while retaining substantive responsibilities and achievements.
- Expanded every major research section with the question, method, contribution and practical relevance.
- Added fuller descriptions of forest forecasting, functional traits, ecosystem services, PAMalytics,
  elephant bioacoustics, gibbon monitoring and field ecology.


## Version 17 changes

- Added the supplied field photograph as a local site asset.
- Replaced the generic Experience-page business image with the personal field photograph.
- Added a personal introduction panel to the Contact page using a tighter crop.
- Retained the project and wildlife imagery on the Research page.


## Version 18 changes

- Moved the personal field photograph to the homepage.
- Used it once only.
- Removed it from the alva section on Experience.
- Removed the repeated version from Contact.
- Added a compact homepage introduction linking to Experience.
