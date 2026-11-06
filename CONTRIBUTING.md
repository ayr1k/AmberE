# Contributing

[简体中文](docs/zh-CN/CONTRIBUTING.md)

Use Windows x64, Node.js 24 and pnpm 11.25.0. Run from `prototype`:

```sh
pnpm install --frozen-lockfile
pnpm test
pnpm build
pnpm test:sites
pnpm release:check
pnpm desktop:smoke
pnpm desktop
```

`pnpm dev` is a browser preview; real file operations and launches require the desktop app. `pnpm package:installer` builds the x64 NSIS installer. Never test destructive actions against personal instances; use temporary fixtures.


Keep English and Chinese documentation synchronized. Add translation entries for new application text, retain stable keys and preserve placeholders. See the language-pack guide. Do not translate user names, filenames, project descriptions or executable arguments.

Preserve transaction rollback, path checks, trusted download origins, checksums, isolated renderer permissions and secret redaction. Add regression coverage for behavioral changes. Do not include account stores, raw personal logs, credentials, local caches or generated installers in source commits. Report sensitive vulnerabilities through the security policy.

Project-owned changes use MPL-2.0. Preserve all dependency and asset notices. Pull requests should explain the user-visible change, validation and remaining limitations. Do not label simulated UI checks as successful real-game tests.


## 1.3.5 platform builds / 平台构建

See [platform build inputs and verification limits](prototype/PLATFORMS-1.3.5.md). Publish the accepted package bytes unchanged. Keep architecture-specific native map engines and their source manifest; platform artifacts are not interchangeable. No signing credentials or private account data belong in source exports.

## Task delivery and releases

Dot coordinates task chats and reviews their pull requests. Each task PR links downloadable test installers, the tested revision, validation and limitations. The user tests and decides whether to merge. A formal release is requested separately and may combine several merged PRs; it builds official packages from main and synchronizes release notes, bilingual documentation and GitHub Pages.

This repository builds AmberE by default. `pnpm package:installer` creates its installer; `pnpm release:source` exports source. Shared core changes originate in AMBER; retain upstream copyrights and licenses, and preserve AmberE authentication restrictions, application identity, branding and update repository when synchronizing features.
