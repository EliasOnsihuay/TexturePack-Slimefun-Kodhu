# Changelog

## v0.1.1

Hotfix release after real-world testing.

### Fixed

- Changed Java `pack_format` from `16` to `6` and declared supported range `6` to `500` for better best-effort loading on older Java clients.
- Corrected documentation around ViaVersion: the server version does not guarantee resource-pack compatibility for every client.
- Stopped presenting Bedrock as full support. Bedrock is now documented as an experimental preview/import package only.

### Notes

- Java Edition remains the real supported target.
- Bedrock cannot fully use Java Slimefun CIT/custom model/overlay behavior without a Bedrock-specific addon or mapping workflow.

## v0.1

Initial public version of TexturePack Slimefun Kodhu.

### Added

- Slimefun base resource pack content.
- 21 addon namespaces.
- Compatibility overlays for newer Minecraft resource pack formats.
- Updated `pack.png`.
- `README.md` for GitHub.
- `ADDONS.md` with included addon counts.
- `CREDITS.md` with maintainer and original source credits.
- `LICENSE.md`, `NOTICE.md`, `DISCLAIMER.md`, `ATTRIBUTION.md`, `SOURCE_PACKS.md`, and `PACK_INFO.md` for public distribution.
- `HOSTING.md` with Java server, Bedrock, GitHub, and personal-use hosting instructions.

### Fixed

- `pack.mcmeta` now uses valid JSON for Elias "Ki3f" Onsihuay Carrillo.
- Version metadata added as `v0.1`.

### Notes

- Original texture rights remain with their authors.
- The pack is configured for MC 26.1.2+ while keeping broad compatibility metadata for older versions.
