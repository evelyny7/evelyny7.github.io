# AGENTS.md: rules for AI agents working on evelyny7.github.io

This folder is Evelyn Yeung's public personal site, published at https://evelyny7.github.io.
Anything committed and pushed here becomes public. These rules apply to every agent that edits this folder.
Rules Evelyn wrote herself are listed first in each section and always win over the supporting rules below them.

## Source of truth

- The CV PDF in this folder (`Evelyn_Yeung_Resume_*.pdf`) is the source of truth for CV content.
- Do not invent, embellish, or reword accomplishments, dates, titles, numbers, or employer names. Copy them faithfully. Fixing obvious typos is fine.
- Keep the site's section order the same as the CV: summary, Professional Experience, Education, Extracurricular, Additional Information.
- Profile links: LinkedIn https://www.linkedin.com/in/evelyn1119/ and GitHub https://github.com/evelyny7.

## Never publish

- Grades, salary, visa status, date of birth.
  - Exceptions approved by Evelyn on 2026-11-04: the GMAT score and the undergraduate GPA from the CV may be shown in the Education section, and the residency status from the CV ("US Permanent Resident") may be shown in the header. No other grades or visa details.
- Anything in `private/`: add it to `.gitignore` first, before any other work in that folder.
- Phone numbers, home or street addresses, or any government ID details.
- Reviewer comments, tracked changes, or draft annotations found in source documents (the current CV PDF contains margin comments; never copy them to the site and do not link the PDF while it still contains them).
- Private email addresses. Only the professional email that already appears on the CV may be shown, and only as a plain mailto link.
- Credentials, API keys, tokens, analytics IDs, or anything found in environment variables or config files.
- Files that happen to be in this folder but were not meant for the site (screenshots, notes, downloads) unless Evelyn says to use them.
- Any content about third parties (colleagues, clients, classmates) beyond what the CV already states.

## Ask Evelyn first

- Before any `git push` or any change on GitHub (remotes, branches, settings, Pages configuration). Local edits are fine; publishing is not.
- Before deleting or overwriting a file.
- Before adding a photo, PDF download, or any new personal detail that is not on the CV.
- Before adding third-party scripts, analytics, trackers, fonts loaded from external CDNs, or contact forms.
- Before changing the site's structure (new pages, renamed files, new navigation items) or its visual identity (colors, logo, typography).
- Before removing or shortening CV content, other than items the "Never publish" list already excludes.
- When the CV and the site disagree and it is unclear which is newer.

## Style

- Plain HTML and CSS, clean and minimal. Minimal vanilla JavaScript only where it clearly helps (for example highlighting the current section in the nav). No build step, no frameworks, no external dependencies. Everything must work when `index.html` is opened directly from disk and when served by GitHub Pages.
- Portfolio is a gallery page that links to each project. Each project gets its own page or external link; the gallery shows a tile per project.
- Tone: professional, concise, confident. No exclamation marks, no emoji, no marketing hype. Bullet points mirror the CV's wording.
- Colors: Columbia blue palette. Light Columbia Blue `#B9D9EB` for accents and surfaces, dark Columbia blue `#1D4F91` for headings and primary accents, mid blue `#6CACE4` for highlights, white and soft grays for backgrounds.
- Navigation: one streamlined top bar with anchor links to each section. No dropdowns, no hamburger menus with hidden items.
- Layout: single-page home, responsive, readable at phone width with a 16px side gutter and no horizontal scroll. Use tiles or cards to make sections scannable.
- Accessibility: semantic headings in order, sufficient color contrast, alt text on images, keyboard-reachable links, visible focus states, respect `prefers-reduced-motion`.
- Keep pages self-contained. Styles live inside the page unless the site grows enough to justify a shared stylesheet.

## When you finish

- Tell Evelyn what you changed and what you skipped, including CV items deliberately left off the site and why.
- List every file created or modified.
- Open the page in the browser to check it before reporting.
- Never push to GitHub unless Evelyn explicitly asks in that conversation.
- Keep this file up to date when Evelyn gives new rules.
- No em dashes anywhere on the site or in this file. Use a middle dot, comma, colon, or a new sentence instead.
