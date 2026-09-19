# Autofill Lite

Autofill Lite is a local-first Electron helper for reviewing and assisting with recruitment-form data entry. It fills only the current page from a local profile library; final save, submission, declarations and privacy-consent actions always remain manual.

## What is included

- `autofill-plugin/`: browser-side matching, form control adapters, repeat-record workflows and site rules.
- `profile-adapter.js` and `profile-editor.*`: local profile normalization and editing UI.
- `bookmarks.*`: local job-URL library.
- `ai-*.js`, `form-graph.js`, `record-graph.js` and related modules: privacy-bounded site analysis and conservative runtime candidates.
- `tests/`: unit and fixture coverage for core behaviors and verified regression paths.
- `docs/`: code provenance, change record and publishing/privacy boundary.

## What is intentionally excluded

This repository contains no personal profile database, browser cookies, session data, API keys, executable installer, Electron runtime, `node_modules`, generated diagnostics, backups or original local build notes. The `defaults/` directory only holds structure-only examples.

## Local setup

1. Install a compatible Electron/Node development environment.
2. Install the dependencies declared by `package.json`.
3. Copy the sample profile structure from `defaults/` into the application's local data directory and fill it locally. Do not commit that data directory.
4. Start the Electron application using the project's local development command.

The distributed portable application is deliberately not tracked here. Build it locally after reviewing the source and licensing status.

## Safety boundary

- No final form save or submission is automated.
- Consent, privacy, declaration and sensitive prompts are excluded from automatic filling.
- Unknown or ambiguous fields remain for review instead of being guessed.
- Site analysis packets must not contain current field values, query strings, cookies, tokens, sessions or profile values.

## Code provenance

This project began from a local `laoli-job-app` baseline. Exact reuse, adapted modules and project additions are documented in [docs/CODE_PROVENANCE.md](docs/CODE_PROVENANCE.md). The baseline's external licensing status was not established during this local comparison; this repository is therefore prepared as a **private source archive** pending a separate licensing review before any public distribution.

## Verification snapshot

The source's latest included build report records 62/62 regression checks passing for its local source snapshot. This GitHub preparation changes documentation and removes personal/local-data material; it does not claim a fresh runtime verification of every recruitment site.

