# Flo for macOS (Apple Silicon)

This repository is the binary-only download channel for Flo. The application
source repository remains private.

## Download the latest build

- [Latest release page](https://github.com/yevhenpopryha-ship-it/whisper-flow-releases/releases/latest)
- [Download Flo for Apple Silicon (DMG)](https://github.com/yevhenpopryha-ship-it/whisper-flow-releases/releases/latest/download/Flo-latest-arm64.dmg)
- [Download ZIP](https://github.com/yevhenpopryha-ship-it/whisper-flow-releases/releases/latest/download/Flo-latest-arm64-mac.zip)
- [SHA-256 checksums](https://github.com/yevhenpopryha-ship-it/whisper-flow-releases/releases/latest/download/SHA256SUMS.txt)

Requires Apple Silicon and macOS 14 or newer.

## Important macOS warning

Flo is distributed without a paid Apple Developer ID signature or Apple
notarization. Its completed app bundle is ad-hoc signed to seal the packaged
files, but that does not verify the developer or mean Apple scanned the build
for known malware. macOS will therefore warn that the developer cannot be
verified. There is no automatic updater; install each new version manually.

Only continue if you intended to download Flo from this repository:

1. Download the DMG and, if desired, compare its SHA-256 with
   `SHA256SUMS.txt` using `shasum -a 256 ~/Downloads/Flo-latest-arm64.dmg`.
2. Open the DMG and copy `Flo.app` to `/Applications`.
3. Try to open Flo once.
4. If macOS blocks it and you trust the download, open **System Settings →
   Privacy & Security** and click **Open Anyway** for Flo.
5. Grant Microphone and Accessibility permissions when prompted.

The expected warning offers a per-app **Open Anyway** choice. If macOS instead
says Flo is damaged, do not bypass that alert; report the release as defective.
Do not disable Gatekeeper globally and do not use Terminal commands to remove
its protection. Ad-hoc replacements may require those permissions again.

The checksum helps detect a changed or incomplete file, but it is not a
substitute for Apple code signing or notarization.
