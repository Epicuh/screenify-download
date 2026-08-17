# Screenify Android download

This repository hosts the public, tracking-free download page and signed Android
release assets for Screenify.

## Current release

- Version: `1.0.14` (`versionCode 15`)
- Minimum Android version: Android 9 / API 28
- APK SHA-256: `A9F9DA8BE075A2A1B7E74FB398C8A3AB2C45EEF9CDA55C654575A514DEFF7864`
- Android 9–12L compatibility signer SHA-256: `A7394529F660B0FBCEF43EE16F7823F582EE98C883E16BF8912426F9977FF297`
- Android 13+ release signer SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

Version 1.0.14 replaces the beta visualizer's custom spectrum logic with an
adapted CAVA-style FFT, automatic sensitivity, and gravity falloff. The display
uses a GPU-rendered discrete LED matrix while preserving the one-tap connection
flow and platform-targeted signing compatibility from version 1.0.13.

The APK binary is distributed through GitHub Releases rather than committed to
the repository.
