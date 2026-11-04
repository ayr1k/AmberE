# 1.3.6 verification

407 regression tests and 2398 bilingual-message checks passed. Both Windows editions passed packaged startup/IPC/map checks, five-theme account expansion checks at normal and large widths, online catalog pagination and log-import UI checks. Synthetic logs cover dependencies, multiple findings, unknown/normal output and stale-report exclusion. Both GitHub Windows build-and-test workflows passed. No new macOS/Linux/FreeBSD 1.3.6 packages or validation are claimed. See [release validation](../prototype/RELEASE-ACCEPTANCE.md).

# Testing

[简体中文](zh-CN/TESTING.md)

See [release validation](../prototype/RELEASE-ACCEPTANCE.md). Run `pnpm test`, `pnpm build`, `pnpm test:sites`, `pnpm release:check` and `pnpm desktop:smoke` in this repository. Microsoft tests are shared-core mock regression coverage; AmberE exposes no Microsoft sign-in. Live third-party providers require separate acceptance.
