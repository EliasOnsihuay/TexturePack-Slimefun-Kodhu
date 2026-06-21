# Troubleshooting

## Pack Is Red Or Incompatible

Use the latest release ZIP. The pack declares a broad format range, but some clients may still show warnings.

## Pack Does Not Download From Server

Check:

- The URL is a direct ZIP URL.
- The ZIP is under the host size limit.
- `pack.mcmeta` is at the ZIP root.
- The server was restarted after editing `server.properties`.

## Items Still Look Vanilla

Check:

- Resource pack order
- OptiFine/CIT Resewn availability
- Client version support
- Slimefun/addon version
- Whether the item comes from an addon included in this pack

## Bedrock Does Not Show Slimefun Items

Expected. Bedrock Preview is not a full Slimefun port.
