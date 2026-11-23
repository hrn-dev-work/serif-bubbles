# Security

This repository is a static page. `index.html` is opened locally or served as a file. It does not run a backend.

## Data

- Dialogue and icons stay in the browser (`localStorage` and in-memory state).
- The page sets `connect-src 'none'`. Do not add analytics, remote fonts, or a fetch of the script.
- There is no account and no environment secret. Do not introduce `NEXT_PUBLIC_*` or a `.env` with credentials.
- Uploaded icons are resized in the browser to a 256px square before storage. They are not uploaded.

## Content Security Policy

`default-src 'none'`, inline script and style only, fonts from `data:`, images from `data:` and `blob:`. Downloads use a blob URL created in the page.

## Font

Zen Maru Gothic is embedded as a WOFF2 data URI under the SIL Open Font License 1.1. The bytes are font data, not a credential. The license text is in the page footer.

## Repository baseline

Layer A files live in `.github/workflows/secret-audit.yml` and `scripts/`. Do not add Dependabot version-update config unless the owner asks.

Install the local hook once per clone:

```bash
cp scripts/pre-commit-secret-check.sh .git/hooks/pre-commit
chmod +x .git/hooks/pre-commit
```
