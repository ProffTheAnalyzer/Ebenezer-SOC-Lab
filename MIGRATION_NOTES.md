# Google Sites migration notes

**Source:** Uploaded Google Takeout archive, Drive/EB-Practice-Lab-Export/SOC Portfolio.  
**Imported edition:** `PUBLISHED` only; October 30, 2026 export.  
**Destination:** Candidate import into public `ProffTheAnalyzer/Ebenezer-SOC-Lab`, pending review.  
**Original site:** https://www.ebpracticelab.org/

## What was included

- All 8 published lab write-ups, split into standalone Markdown README files.
- 150 referenced screenshots in their original lab order, grouped into `screenshots/` beside each lab.
- Home and About content as additional references and six original site assets.
- A blank Wazuh lab file to fill in with your future screenshots and a reusable lab template.

## What was intentionally excluded

- The original `DRAFT` Google Sites HTML files and duplicated JPG assets.
- Large Google Sites page wrappers, JavaScript and CSS, which aren't necessary for Markdown documentation.
- Any live extraction of KQL from screenshots: not reliable; author queries separately once reviewed.

## Content and safety checks

- The published and draft versions have the same extracted page text and duplicate image bytes; the published version was selected intentionally.
- All 150 screenshot references in the published Project Page have corresponding local JPG files.
- This package has not been pushed to the user's public GitHub repository.
- Screenshot thumbnails were reviewed for broad grouping, **not** every pixel for secrets or private data. Please inspect screenshots carefully before any public GitHub commit.
- Source prose contains a repeated **Phase 1 / Phase 2: Static Header Analysis** heading and other wording that may merit later editing. For fidelity, the migration avoids making technical corrections without explicit review.
- The original Google Sites text includes security conclusions (for example, around phishing and Conditional Access) that were **not independently verified** in this migration.

## Publishing workflow

The local file structure is ready for an import. Keep the existing GitHub LICENSE, and merge the package content into the repository on a review branch after inspecting sensitive screenshots. Do not replace the entire repository root without checking existing files.


## Wazuh update (October 30–31, 2026)

The Wazuh lab in this repository is a completed **initial setup and telemetry collection** write-up with 17 screenshots. The successful installation image has the generated password redacted. Sysmon, custom detection rules, and active response tests are not yet documented as completed.
