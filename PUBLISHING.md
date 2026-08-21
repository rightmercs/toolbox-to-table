# Toolbox to Table Publishing Guardrails

This repository publishes a public website. Treat every tracked file as potentially public.

## Never commit

- Commercial workbook files (`.xlsx`, `.xlsm`)
- Buyer download packages (`.zip`)
- Print-ready handbook PDFs
- Licensed standards, excerpts, scans, tables, or figures
- Customer names, email addresses, receipts, or license records
- Passwords, access tokens, payment data, or private keys

Commercial downloads belong in Payhip. Public pages should link to the Payhip checkout and contain only approved previews, original marketing copy, and product documentation intended for public viewing.

## Product release checklist

1. Verify the workbook and documentation against the intended technical scope.
2. Replace reproduced standards content with original workflows, calculators, checklists, or section-navigation guidance.
3. Confirm the applicable licensed standards are required and are not included.
4. Render and visually inspect every worksheet and document page.
5. Scan formulas for common spreadsheet errors.
6. Update version, changelog, product metadata, screenshots, and website copy.
7. Upload the buyer ZIP to Payhip; never upload it to this repository.
8. Confirm the public product page, checkout link, support page, privacy page, and terms page.
9. Publish through `platform-2.0`, validate, then update `main`.

## Current repository exception

Legacy print-ready handbook PDFs are still present in repository history. `_config.yml` excludes them from the GitHub Pages build, and the site-validation workflow fails if a PDF, workbook, or ZIP reaches the generated site. Removing those legacy files from Git history requires a separately approved history rewrite and coordinated fresh clone.
