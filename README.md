# Get latest Minecraft Jar file from Mojang

## NOTE

this was made for the purposes of pulling some files from the game to automatically modify, and build a resourcepack from it, NOT to illegally download and play Minecraft.

## Inputs

### `mcversion`

**Optional** (*default:* `latest`) The Minecraft version to download (defaults to latest release)

If `mcversion` is `latest` or `release`, the latest release (not snapshot) version is downloaded

If `mcversion` is `latest-snapshot`, `latest-snapshot`, or `snapshot`, the latest snapshot version is downloaded

Otherwise, `mcversion` is expected to be a version string, like `1.16.3`, `1.16.4-pre1`, `20w30a`, `a1.0.4`, `c0.0.11a` or `rd132211`. (the last 3 are very old versions, so the string may look a little odd)

### `filename`

**Optional** (*default:* `minecraft-<version>.jar`) The name of the file to save to. (if no file extension is provided, it will be set as .jar)

## Outputs

### `jarfilename`

the name of the jar file downloaded (provided for when `mcversion` is `latest`, `snapshot` or similar)

### `minecraftversion`

the version of minecraft that was downloaded (provided for when `mcversion` was set to latest or snapshot)

## To extract the jar

I don't include that in this action, because essentially it's just a zip file. You can you an unzipping tool to unzip the downloaded jar. I have yet to test it for this, but the [zip action](https://github.com/marketplace/actions/create-zip-file) does its job well.
