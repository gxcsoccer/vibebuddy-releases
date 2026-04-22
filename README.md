# VibeBuddy Releases

Public release artifacts for [VibeBuddy](https://github.com/gxcsoccer/vibebuddy)
— a macOS desktop pet companion for Claude Code.

This repo only hosts:
- **Release DMGs** under [Releases](https://github.com/gxcsoccer/vibebuddy-releases/releases)
- **`appcast.xml`** at <https://gxcsoccer.github.io/vibebuddy-releases/appcast.xml>
  for Sparkle auto-updates

The source code lives in the private repo `gxcsoccer/vibebuddy`. This
public mirror exists so Sparkle (which can't authenticate against
private GitHub repos) can fetch the appcast and download DMGs.

## Install

Download the latest DMG from
[Releases](https://github.com/gxcsoccer/vibebuddy-releases/releases/latest)
→ open → drag VibeBuddy to Applications. Launch from Applications.

Two flavors per release:

- `VibeBuddy-X.Y.Z.dmg` — release build (recommended for daily use)
- `VibeBuddy-X.Y.Z-debug.dmg` — debug build (Debug HUD enabled, for
  testers reporting issues)

Both are Developer ID signed + Apple notarized + stapled.

## Auto-update

Once installed, the app checks for updates daily (and on demand via
menubar → Check for updates…). Updates are EdDSA-signed by Sparkle.
