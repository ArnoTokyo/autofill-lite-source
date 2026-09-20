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

Autofill Lite 源码归档

Autofill Lite 是一款本地优先的 Electron 招聘表单辅助工具，用于核对并协助填写招聘表单。它使用本地资料库；最终保存、提交、声明及隐私授权始终由用户手动完成。

## 下载

完整的脱敏源码快照为 `autofill-lite-source-public.zip`。压缩包保留原始目录结构，包含 247 个源码、测试、夹具与文档文件。

## 已包含的能力

- 浏览器侧字段匹配、表单控件适配和重复记录工作流。
- 本地资料规范化、资料编辑与职位链接收藏。
- 保守的网站分析、运行时语义候选和可恢复检查点。
- 覆盖核心逻辑及已验证回归路径的单元测试和夹具测试。

## 本公开归档明确不包含

不含任何已填写的个人资料、浏览器 Cookie / 会话、API 密钥、可执行文件、Electron 运行时、依赖目录、备份或诊断输出。示例资料文件仅保留字段结构。

## 安全边界

- 不自动执行最终表单保存或提交。
- 不自动填写同意、隐私、声明及其他敏感提示。
- 对未知或含义不明确的字段保留给用户核对，不擅自猜测。

## 代码来源与发布提示

本项目基于本地 `laoli-job-app` 基线演进。对比结果为：53 个文件逐字节复用、23 个基线文件经过改造、237 个为 Autofill Lite 新增。不含 Autofill Lite.exe、Electron 运行环境和依赖；解压后不能直接自动填写。

本次本地比对未能确认继承基线代码的外部许可证。本公开源码归档用于保留可审阅的工程记录，并不表示所有继承代码均可被独立许可、再分发或再次发布；复用前请自行核对适用授权。

## 校验快照

发布前，224 个 JavaScript 文件均通过语法检查，122/122 个随附的单元/夹具测试通过。这不代表每一个招聘网站均已完成最新的真实页面验证。
