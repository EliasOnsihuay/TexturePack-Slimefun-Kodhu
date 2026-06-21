# Hosting And Server Setup

TexturePack Slimefun Kodhu v0.1.1 has two release packages:

- Java Edition: `TexturePack-Slimefun-Kodhu-v0.1.1.zip`
- Bedrock preview: `TexturePack-Slimefun-Kodhu-Bedrock-Preview-v0.1.1.mcpack`

## Recommended Distribution

| Use case | Recommended file | Notes |
|---|---|---|
| Personal Java use | `TexturePack-Slimefun-Kodhu-v0.1.1.zip` | Put it in `.minecraft/resourcepacks`. |
| Java server use | `TexturePack-Slimefun-Kodhu-v0.1.1.zip` | Upload it to a direct resource-pack host and set it in `server.properties`. |
| GitHub release | Both release files | Good for downloads, docs, credits, and version history. |
| Bedrock personal use | `TexturePack-Slimefun-Kodhu-Bedrock-Preview-v0.1.1.mcpack` | Preview/import package only, not full Slimefun support. |
| Bedrock server/world use | Not recommended as full support | Slimefun is Java-only; Bedrock needs separate mapping/addon work. |

## Java Server Hosting With MCPacks

MCPacks can host Minecraft resource packs for servers. The site states that the maximum resource pack size is 95 MB and that the generated link can be used in `server.properties`.

This pack is about 15 MB, so it is small enough for MCPacks.

Steps:

1. Go to `https://mc-packs.net/`.
2. Upload `TexturePack-Slimefun-Kodhu-v0.1.1.zip`.
3. Copy the generated direct pack URL.
4. Open your Java server `server.properties`.
5. Set:

```properties
resource-pack=PASTE_MCPACKS_URL_HERE
resource-pack-prompt=TexturePack Slimefun Kodhu v0.1.1 is recommended for the full Slimefun texture experience.
require-resource-pack=false
```

Optional:

```properties
require-resource-pack=true
```

Use `true` only if every player must use the pack to join.

## SHA-1 Hash

Some server setups also use `resource-pack-sha1`.

If your host gives you a SHA-1 value, put it here:

```properties
resource-pack-sha1=PASTE_SHA1_HERE
```

If no SHA-1 is provided, many modern servers can still load the pack with only `resource-pack`.

## GitHub Setup

Use GitHub for:

- Source documentation
- Credits
- Changelog
- Issues and credit corrections
- Release downloads

Recommended GitHub release assets:

- `TexturePack-Slimefun-Kodhu-v0.1.1.zip`
- `TexturePack-Slimefun-Kodhu-Bedrock-Preview-v0.1.1.mcpack`

Do not rely on a normal GitHub page URL for `server.properties`. Java servers need a direct downloadable ZIP URL. A host like MCPacks is simpler for server resource-pack delivery.

## Bedrock Notes

The Bedrock package is experimental.

Bedrock does not fully support Java resource pack features like:

- Java custom item model overrides
- `pack.mcmeta` overlays
- CIT/OptiFine/CIT Resewn `.properties`
- Java Slimefun custom item behavior

For Bedrock preview/import testing, use:

```text
TexturePack-Slimefun-Kodhu-Bedrock-Preview-v0.1.1.mcpack
```

This can be imported into Minecraft Bedrock as a resource pack preview. It will not reproduce Java Slimefun custom item model behavior by itself.

## Personal And Server Use

This pack is intended for:

- Personal use
- Private servers
- Community servers
- Public server resource-pack use with credits preserved

Keep `CREDITS.md`, `ATTRIBUTION.md`, `LICENSE.md`, and `NOTICE.md` with public releases.
