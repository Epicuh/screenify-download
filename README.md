# Screenify Android download

This repository hosts the public, tracking-free download page and signed Android
release assets for Screenify.

## Current release

- Version: `1.0.17` (`versionCode 18`)
- Minimum Android version: Android 9 / API 28
- APK SHA-256: `5DAB7C8336263D396D5A6CF92178B1376CFFA8D585C149483176C90E0C532865`
- Android 9–12L compatibility signer SHA-256: `A7394529F660B0FBCEF43EE16F7823F582EE98C883E16BF8912426F9977FF297`
- Android 13+ release signer SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

Version 1.0.17 sends the phone's clean playback-capture PCM over the pinned local
TLS connection and moves spectrum analysis to native CAVA on the Screenify display.
The phone no longer performs continuous FFT work. Bounded queues discard stale
audio instead of building latency, while Screenify display 2.1.37 produces and
paces the 11-band matrix at 60 FPS and caps every LED and peak on-screen.

The APK binary is distributed through GitHub Releases rather than committed to
the repository.
