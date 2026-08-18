# Screenify Android download

This repository hosts the public, tracking-free download page and signed Android
release assets for Screenify.

## Current release

- Version: `1.0.16` (`versionCode 17`)
- Minimum Android version: Android 9 / API 28
- APK SHA-256: `C725F42500AB3FE521C2A54DE14036E68E540FBA1A9021D2A77490B8723F4038`
- Android 9–12L compatibility signer SHA-256: `A7394529F660B0FBCEF43EE16F7823F582EE98C883E16BF8912426F9977FF297`
- Android 13+ release signer SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

Version 1.0.16 separates continuous playback capture from spectrum analysis.
The analyzer always consumes the newest complete window instead of replaying stale
work after a scheduler delay. Persistent TLS connections, cached artwork payloads,
and smaller bridge responses remove avoidable transport stalls. Paired with
Screenify display 2.1.32, the matrix holds the panel's refresh cadence, keeps every
LED and peak on-screen, and permanently hides the kiosk cursor.

The APK binary is distributed through GitHub Releases rather than committed to
the repository.
