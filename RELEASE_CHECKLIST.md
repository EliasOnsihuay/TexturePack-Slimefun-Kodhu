# Release Checklist

Use this before publishing a new version.

## Java Pack

- `pack.mcmeta` is valid JSON.
- `pack.mcmeta` is at the root of the ZIP.
- `pack.png` is at the root of the ZIP.
- Release ZIP opens with 7-Zip.
- Release ZIP passes archive test.
- Version is updated in `VERSION`, `README.md`, `CHANGELOG.md`, `PACK_INFO.md`, and `pack.mcmeta`.

## Bedrock Preview

- `manifest.json` is valid JSON.
- UUIDs are present.
- `pack_icon.png` exists.
- README says this is preview-only.
- `.mcpack` opens as a ZIP and passes archive test.

## GitHub

- Commit documentation updates.
- Push `main`.
- Create release tag.
- Upload Java ZIP.
- Upload Bedrock Preview `.mcpack`.
- Verify release download links.

## Server Hosting

- Upload Java ZIP to MCPacks or another direct ZIP host.
- Put direct URL in `server.properties`.
- Test with at least one clean client.
