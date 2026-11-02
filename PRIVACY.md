# Privacy and local data

[简体中文](docs/zh-CN/PRIVACY.md)

AmberE does not offer Microsoft sign-in or include a Microsoft Client ID. Third-party passwords are sent to the HTTPS authentication address entered by the user and are not persisted. Saved tokens use Windows user encryption; it does not protect against malicious software running as the same Windows user.

Data is stored separately in `%APPDATA%/AmberE`, with a configurable game-library location. No automatic account transfer occurs. Local account removal does not revoke server-side authorization. Upgrade backups may retain encrypted account records.

Searches and downloads contact game, loader, Java, mod and GitHub providers as requested. Updates use only `ayr1k/AmberE`. No diagnostic reports, logs, worlds or local mod files are automatically uploaded. Optional local-mod identification sends a file hash to Modrinth. Diagnostics use an allowlist; review all logs before sharing. Language packs, backgrounds and themes stay local. Theme exports contain visual preferences and referenced images only; review image rights and personal details before sharing.

Uninstall preserves game data. Confirmed cleanup targets downloaded updates or old configuration backups, not active accounts or worlds.

Trial copies and change-recovery snapshots stay in the selected local game library. Copies may include worlds when explicitly selected; configuration snapshots can contain personal data written by games or mods. They are not automatically uploaded or included in preference-template exports. Template JSON contains questionnaire preferences only; review it before sharing. Global quick search searches local instances/actions and sends no search query to a server.

## Home modules (1.2.0)

The play journal is local and enabled by default. Its calendar settings let you disable, export or clear it. It records instance identifiers and observed runtime, which may include idle time; concurrent instance durations add together. Missing observations are marked incomplete. Old launch records carry unknown duration. Exported history contains instance identifiers and timestamps: review before sharing.

News refresh is manual by default. Optional automatic refresh runs while its module is mounted and the document is visible, at most every 30 minutes. Requests reach `launchercontent.mojang.com`; opening general articles uses the system browser. Article text is not translated automatically and remote HTML is never executed. News and release-note caches remain local. Screenshot browsing reads local PNGs; Copy image writes the selected image to the system clipboard. No screenshot is uploaded. Storage analysis caches estimates locally and does not delete files automatically.

## Download connections (1.2.2)

Automatic source selection and manual connection diagnostics contact public Minecraft and BMCLAPI endpoints; diagnostics also contact Modrinth and Fabric. Requests send ordinary connection metadata (including your IP address and a launcher user-agent), not account tokens, instance names or local paths. Automatic selection caches a source choice for ten minutes without geolocation. Supported file downloads may use BMCLAPI and its public CDN nodes; third-party servers apply their own privacy policies. Account authentication is never routed through the download mirror. The copied diagnostic summary contains service names, statuses and elapsed times only. Partial files and task recovery records remain in the local game library.

## Local modpack import (1.2.3)

Selected archives and import choices are retained in the new instance’s `.amber-setup` folder to support recovery. Archives, embedded configuration files and worlds are not uploaded by the importer. MRPACK downloads contact the permitted content hosts in its manifest; game, Java and loader preparation contact their normal providers. Import reports contain relative file names and pack metadata. Backups of the instance may include this retained content; review it before sharing.
