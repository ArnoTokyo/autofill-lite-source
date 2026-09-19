# Code provenance and project improvements

## Comparison basis

- **Current source:** `Autofill-Lite-v0.1.7-portable/resources/app`
- **Baseline:** `laoli-job-app/resources/app`
- **Method:** matching relative paths, SHA-256 comparison for direct reuse, then code-path and file-tree comparison for differences.
- **Excluded from the count:** `node_modules`, backup files and local build/runtime artifacts.

| Result | Files |
| --- | ---: |
| Current source examined | 313 |
| Baseline source examined | 113 |
| Same relative path and same SHA-256 | 53 |
| Same relative path but changed | 23 |
| Present only in Autofill Lite | 237 |
| Present only in the baseline | 37 |

These classifications describe the two supplied local snapshots only. They do not establish authorship, copyright ownership or licence rights.

## Direct reuse from the baseline

The exact-copy group consists mainly of mature generic control support and static lookup data:

- Date-picker framework and handlers, including Ant, Element, iView, native, Phoenix, split-year-month and related adapters.
- Most generic select-adapter modules, including Ant, Bootstrap, iView, Material, Next, Semantic and Vuetify support.
- Generic browser helpers such as HTML cleanup, Electron text bridge and interactive-form runtime.
- Static taxonomy data for Bank of Communications, 51job and Zhaopin.

The complete exact-reuse inventory is reproducible from the relative-path/SHA-256 comparison; it is not relabeled as original work in this repository.

## Adapted baseline modules

These files keep the baseline path but have non-identical content. They are inherited foundations with Autofill Lite modifications, not wholesale new code.

| Area | Representative files | Improvement made in Autofill Lite |
| --- | --- | --- |
| Electron shell | `main.js`, `index.html`, `renderer.js`, `styles.css`, `package.json` | Reoriented the app from a general job-management desktop UI to a local-first form-assistance shell, profile library and diagnostics surface. |
| Field matching | `element-matcher.js`, `field-dictionary.js`, `data-matcher.js` | Strengthened semantic labels, readonly handling, date recognition and safer ambiguity handling. |
| Form execution | `form-handler.js`, `fill-engine.js`, `experience-handler.js` | Added controlled-input verification, repeat-record ownership, delayed readback, stage handling and partial-completion reporting. |
| Workflow routing | `special-site-workflow.js`, `private/private-special-sites.js`, `site-loader.js` | Added bounded local workflows and section navigation for supported recruitment routes without enabling final submission. |
| UI component support | `site-templates.js`, `select-adapter/adapters/{ant-main,custom,element,phoenix}.js` | Expanded practical adapter capabilities and selection verification for real form widgets. |
| Runtime integration | `electron-adapter.js`, `utils.js`, `manifest.json` | Connected the browser-side core to local profile, diagnostics and Electron runtime boundaries. |

## Autofill Lite additions

The following paths do not appear in the compared baseline snapshot and represent the current project's added architecture:

| Added capability | Main paths |
| --- | --- |
| Local profile library and normalization | `profile-adapter.js`, `profile-editor.*`, `defaults/` |
| Local bookmark library | `bookmark-store.js`, `bookmarks.*` |
| Safety-first semantic analysis and optional API boundary | `ai-*.js`, `site-analysis-ai-input.js`, `semantic-site-candidate-lifecycle.js`, `site-support-diagnostic.js` |
| Conservative recovery and completion state | `autofill-plugin/content/{checkpoint-core,checkpoint-runtime,completion-resolver,input-adapter}` |
| Form and record graph model | `autofill-plugin/content/{form-graph,record-graph,location-resolver,select-capability-resolver,site-analysis-collector}` |
| Bank of Communications knowledge layer | `autofill-plugin/core/bankcomm-lessons.js` |
| Test coverage | `tests/` (122 source-only test files in this snapshot) |
| Fixtures and review documentation | `fixture/`, `BUILD_REPORT.md`, project documentation |

## Deliberately not carried forward from the baseline

The original baseline includes broad job-management and content modules, such as interview tools, knowledge-base content, exam links, generic assistant screens and resume-editor assets. Those baseline-only modules are absent from Autofill Lite's source tree. Their removal reflects the narrower local recruitment-form assistance scope; it does not imply they were recreated.

## Privacy and publication assessment

The original local source included a personal runtime profile and project-specific test examples. This repository replaces profile defaults with structure-only examples and normalizes residual test/demo values. It excludes all runtime data, backups, binary artifacts and diagnostics. Because the baseline licence is not established, the repository should remain private until licensing is reviewed.

