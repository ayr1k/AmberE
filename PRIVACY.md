# Privacy and local data

[简体中文](docs/zh-CN/PRIVACY.md)

AmberE does not offer Microsoft sign-in or include a Microsoft Client ID. Third-party passwords are sent to the HTTPS authentication address entered by the user and are not persisted. Saved tokens use Windows user encryption; it does not protect against malicious software running as the same Windows user.

Data is stored separately in `%APPDATA%/AmberE`, with a configurable game-library location. No automatic account transfer occurs. Local account removal does not revoke server-side authorization. Upgrade backups may retain encrypted account records.

Searches and downloads contact game, loader, Java, mod and GitHub providers as requested. Updates use only `ayr1k/AmberE`. No diagnostic reports, logs, worlds or local mod files are automatically uploaded. Optional local-mod identification sends a file hash to Modrinth. Diagnostics use an allowlist; review all logs before sharing. Language packs, backgrounds and themes stay local. Theme exports contain visual preferences and referenced images only; review image rights and personal details before sharing.

Uninstall preserves game data. Confirmed cleanup targets downloaded updates or old configuration backups, not active accounts or worlds.

Trial copies and change-recovery snapshots stay in the selected local game library. Copies may include worlds when explicitly selected; configuration snapshots can contain personal data written by games or mods. They are not automatically uploaded or included in preference-template exports. Template JSON contains questionnaire preferences only; review it before sharing. Global quick search searches local instances/actions and sends no search query to a server.
