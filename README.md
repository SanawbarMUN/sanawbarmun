# SanawbarMUN — standalone website preview

Open `index.html` in Chrome, Edge, Safari or Firefox to view the website. No installation, login, or paid subscription is needed.

## What works
- Fully responsive homepage following the provided design reference
- Dropdown menus for committees and resources
- Eight individual committee pages with chair photo slots, bios, topics, and resource links
- Program, Resources, Registration and FAQ pages
- Countdown and smooth scrolling / reveal animations
- External links open in a new tab

## Change conference information for next year
Open `content.js` in a text editor. Edit the fields in `window.SANAWBAR_CONTENT`:
- `year`, `datesLabel`, `dateStart`, `venue`, `theme`
- `logo`: web URL or relative local image path (`assets/logo.png`)
- `photo`: web URL or local image path (`assets/conference.jpg`)
- `secretary`, `committees`, `program`, `resources`, `faq`
- For chair photographs, set `photo:'assets/chair-name.jpg'` and place that file in `assets`.
- To publish a background guide, add e.g. `{title:'Background Guide',url:'https://...'}` to that committee's `resources` list.
- `registration`: set to an approved school registration-form URL.

The preview has sample committee names, agendas, statistics and an illustrative schedule; verify and replace before publishing. The sample 2027 date is used **only** to demonstrate the countdown, not an announced conference date. The crest is a temporary vector emblem, not the official school logo.

## Free hosting
**GitHub Pages:** Create a school-owned public repository, upload these files to the root, then go to repository Settings → Pages → Deploy from a branch → main / (root). The published URL will be of the form `https://SCHOOL-ORG.github.io/REPO/`. Keep a teacher as organization owner and invite future student editors as collaborators. No paid AI builder is required.

**Cloudflare Pages:** Upload this folder using Direct Upload or connect the GitHub repository and set no build command; static files can be published as-is.

## Important limitations
This is a real working **public website prototype**, not yet an authenticated editing dashboard. Students can edit its content for free by changing `content.js` through GitHub's web editor and committing changes. A secure point-and-click CMS can be added later; it needs an authentication configuration and must be tested before offering it to students. It would be inaccurate to claim an admin login works at this stage.

Avoid placing private student details in a public repository. Use school-approved external registration forms for personal data. Use only images you have permission to publish.

The displayed Google Fonts require internet access; offline browsers will use the included serif/sans-serif fallbacks.
