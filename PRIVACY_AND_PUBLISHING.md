# Privacy and publishing boundary

## Local-only data

Keep the following outside source control:

- completed candidate profile JSON;
- saved job URLs and folders;
- browser sessions, cookies, tokens and API keys;
- site-analysis packets, error diagnostics and backups;
- packaged application binaries and generated release files.

## Before sharing a branch or archive

1. Search for phone numbers, email addresses, identity-card patterns and personally identifying profile text.
2. Replace all test fixture values with generic examples where a personal record was used.
3. Verify that no `autofill-lite-data/` directory, archive, executable or `node_modules/` directory is staged.
4. Confirm that final-save and submit controls remain outside automation scope.

## Distribution status

This repository is prepared as a private archive. The local comparison did not establish a redistribution licence for inherited baseline files. Do not make it public without resolving that question.

