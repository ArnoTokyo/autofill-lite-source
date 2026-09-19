# Autofill Lite source archive

Autofill Lite is a local-first Electron helper for reviewing and assisting with recruitment-form data entry. It uses a local profile library; final save, submission, declarations and privacy-consent actions remain manual.

## Download

The complete privacy-screened source snapshot is available as [autofill-lite-source-public.zip](autofill-lite-source-public.zip). It contains 247 source, fixture, test and documentation files while preserving the original directory structure.

## Included capabilities

- Browser-side field matching, form-control adapters and repeat-record workflows.
- Local profile normalization, profile editing and local job-URL bookmarks.
- Conservative site analysis, runtime semantic candidates and resumable checkpoints.
- Unit and fixture coverage for core and verified regression paths.

## Excluded from this public archive

No completed profile, browser cookie/session, API key, executable, Electron runtime, dependency directory, backup or diagnostic output is included. Sample profile files are structure-only.

## Safety boundary

- No final form save or submission is automated.
- Consent, privacy, declaration and sensitive prompts are excluded from automatic filling.
- Unknown or ambiguous fields remain for review instead of being guessed.

## Provenance and publication notice

This project began from a local `laoli-job-app` baseline. The comparison identifies 53 byte-identical reused files, 23 adapted baseline files and 237 Autofill Lite additions. See [CODE_PROVENANCE.md](CODE_PROVENANCE.md), [CHANGELOG.md](CHANGELOG.md), [PRIVACY_AND_PUBLISHING.md](PRIVACY_AND_PUBLISHING.md) and [NOTICE.md](NOTICE.md).

The inherited baseline's external licence was not established during the local comparison. This public source archive is shared as a documented engineering record, not as a claim that all inherited code is independently licensable for redistribution. Review the applicable permissions before reuse or republication.

## Verification snapshot

Before publication, all 224 JavaScript files passed syntax validation and all 122 included unit/fixture tests passed. This is not a claim of fresh live-site verification for every recruitment form.
