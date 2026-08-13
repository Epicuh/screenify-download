# Screenify Android download

This repository hosts the public, tracking-free download page and signed Android
release assets for Screenify.

## Current release

- Version: `1.0.12` (`versionCode 13`)
- Minimum Android version: Android 9 / API 28
- APK SHA-256: `AF0C0D0EF2E4BAC2475346E74506231CE78918A8EDACC2FCD6691BCBF5F05D68`
- Android 9–12L compatibility signer SHA-256: `A7394529F660B0FBCEF43EE16F7823F582EE98C883E16BF8912426F9977FF297`
- Android 13+ release signer SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

Version 1.0.12 uses Android's platform-targeted signing rotation: Android 9–12L
receives the original signer for maximum update compatibility, while Android 13+
receives Screenify's permanent release signer and its verified certificate lineage.

The APK binary is distributed through GitHub Releases rather than committed to
the repository.
