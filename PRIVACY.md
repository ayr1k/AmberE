# Privacy and local data

[简体中文](docs/zh-CN/PRIVACY.md)

AmberE does not offer Microsoft sign-in or include a Microsoft Client ID. Third-party passwords are sent to the HTTPS authentication address entered by the user and are not persisted. Saved tokens use Windows user encryption; it does not protect against malicious software running as the same Windows user.

Data is stored separately in `%APPDATA%/AmberE`, with a configurable game-library location. No automatic account transfer occurs. Local account removal does not revoke server-side authorization. Upgrade backups may retain encrypted account records.

Searches and downloads contact game, loader, Java, mod and GitHub providers as requested. Updates use only `ayr1k/AmberE`. No diagnostic reports, logs, worlds or local mod files are automatically uploaded. Optional local-mod identification sends a file hash to Modrinth. Diagnostics use an allowlist; review all logs before sharing. Language packs and backgrounds stay local.

Uninstall preserves game data. Confirmed cleanup targets downloaded updates or old configuration backups, not active accounts or worlds.
