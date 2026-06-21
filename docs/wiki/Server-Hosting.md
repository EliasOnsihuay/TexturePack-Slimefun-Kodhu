# Server Hosting

## Recommended Java Setup

Upload `TexturePack-Slimefun-Kodhu-v0.1.1.zip` to a direct resource-pack host such as MCPacks.

MCPacks: `https://mc-packs.net/`

Then configure `server.properties`:

```properties
resource-pack=PASTE_DIRECT_ZIP_URL_HERE
resource-pack-prompt=TexturePack Slimefun Kodhu v0.1.1 is recommended for Slimefun textures.
require-resource-pack=false
```

If you want to force the pack:

```properties
require-resource-pack=true
```

## SHA-1

If your host provides SHA-1:

```properties
resource-pack-sha1=PASTE_SHA1_HERE
```

## GitHub Links

GitHub release links are good for downloads, but normal GitHub page URLs are not ideal for `server.properties`. Prefer a direct ZIP host for servers.
