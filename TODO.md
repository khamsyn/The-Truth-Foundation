# Task Plan: Clean CSS and Link Files

## Information Gathered
- HTML file (`index.html`) contains sections with IDs and classes: header, .profile, nav, .footer, #MenuBtn, main, #home, .home-row, #about, .sub-heading, .divider, .sub-para, .about-col, .img-col, .info-col, .icon-list-col, .icon-list, #fact, #skill, .skill-row, .skill-box, .skill-info, #resume, .resume-row, .resume-cols, .my-info, .my-edu, #portfolio, .port-row, .port-item, .port-img, .port-info, #service, #contact, .contact-row, .contact-left, .contact-right, .icon-box, .icon, .info, .map.
- CSS file (`style.css`) has rules for these, but some are unused based on HTML structure.
- Unused CSS rules identified:
  - `#fact .fact-row` and all its sub-rules (HTML has no `.fact-row` in `#fact`).
  - `#skill .skill-outer-line` and `.skill-inner-line` (not present in HTML).
  - `#resume .pro-exp` and `.sp-box` (not in HTML).
  - `#service .service-row` and all its sub-rules (HTML uses `.skill-row` instead).
  - `.download-cv` (not in HTML).
  - Some selectors in `.my-edu` like `span + p` (no spans in HTML).

## Plan
1. Remove unused CSS rules from `style.css` to clean it up.
2. Rename the CSS file to `styles.css` for better naming, and update the link in `index.html` to reflect the new name (interpreting "renaming it in css" as renaming the CSS file itself).
3. Verify the changes by checking the files.

## Dependent Files to Edit
- `style.css`: Remove unused rules.
- `index.html`: Update the CSS link href to `styles.css`.

## Followup Steps
- Test the website to ensure styles still work after cleanup.
- Confirm no broken styles.
