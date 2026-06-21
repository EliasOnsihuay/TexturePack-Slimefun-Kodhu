# Troubleshooting

## The Java Pack Does Not Load

Check these first:

1. Make sure `pack.mcmeta` is at the root of the ZIP.
2. Make sure you are using `TexturePack-Slimefun-Kodhu-v0.1.1.zip`.
3. If using a server, make sure `server.properties` points to a direct ZIP URL.
4. If hosting on GitHub, do not use the normal web page URL as `resource-pack`.
5. Upload the ZIP to MCPacks or another direct pack host and use the generated URL.

## ViaVersion Notes

ViaVersion lets newer or older clients join a server, but it does not fully convert Java resource pack formats.

The client version still decides:

- Whether `pack_format` is accepted.
- Whether overlays are supported.
- Whether custom item model formats are supported.
- Whether CIT/OptiFine/CIT Resewn features are available.

## Slimefun Version Notes

Slimefun itself is a Java server plugin. The server may run an older Minecraft version, but players can join with newer clients through ViaVersion. In that case, the resource pack must still be compatible with the player client.

This pack uses `pack_format: 6` with `supported_formats: 6-500` as a best-effort universal Java setup.

## Bedrock Does Not Work Like Java

This is expected.

Bedrock Edition does not support Java resource pack features such as:

- Java custom item model overrides
- Java `pack.mcmeta` overlays
- OptiFine/CIT Resewn `.properties`
- Slimefun Java custom item behavior

The `.mcpack` is only a preview/import package. Full Bedrock support would require a separate Bedrock addon or Geyser custom item mapping workflow.
