# Assessment feedback remediation report

Date: 2 November 2026
Project: The Cozy Book Café — Part 3

## Changes made in this revision

1. **Form delivery honesty:** the Enquiry form previously displayed a received/success-style message despite having no configured email endpoint. It now opens a pre-addressed email draft, includes the enquiry reference and submitted details, and explains that the visitor must press Send. The Contact form also states this clearly. If `FORM_ENDPOINT` is configured, both forms use it and show server-submission success only after an OK response.
2. **Documentation:** README and changelog updated to distinguish a prepared email draft from a delivered message and to list outstanding evidence requirements.
3. **Static SEO/HTML review:** all five pages have a title, meta description and one H1; local asset/navigation references resolve; image elements have alt attributes; IDs are unique; sitemap XML parses successfully.
4. **JavaScript:** `node --check` passes for `js_assets/script.js`.

## What this ZIP cannot prove or complete on its own

- A working email endpoint requires the owner to create a form service account, configure an endpoint, and submit a real test. The endpoint is intentionally not invented or embedded.
- GitHub commit history cannot be recovered or proved from this ZIP because it contains no `.git` repository. Push the folder to the student's GitHub repository and capture the commits page.
- Deployment must be completed from the owner's hosting account. The sitemap and robots file currently reference `https://frolicking-raindrop-d6cb2b.netlify.app`; confirm that is the final live domain or replace it in both files before redeploying.
- Full live browser testing still requires a browser on the deployed site. A headless browser executable was not available in this environment, so no claim of completed live desktop/mobile browser testing is made.

## Required final evidence

- Real endpoint test result (if automatic delivery is required), or screenshot of the populated mail draft and clear Send instruction.
- GitHub repository URL and commit history screenshot.
- Live HTTPS deployment URL and screenshots of all five pages at desktop and mobile widths.
- Browser console/network check showing no errors, plus working gallery, search/filter, and form validation.
- Live `sitemap.xml` and `robots.txt` from the final deployment domain.
