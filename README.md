# Screenify Android download

This repository hosts the public, tracking-free download page and signed Android
release assets for Screenify.

## Current release

- Version: `1.0.15` (`versionCode 16`)
- Minimum Android version: Android 9 / API 28
- APK SHA-256: `1A0862D231A346BF1A3D66D99ED56B5F20E828A957DF4F8422C3EC6F04B10DB3`
- Android 9–12L compatibility signer SHA-256: `A7394529F660B0FBCEF43EE16F7823F582EE98C883E16BF8912426F9977FF297`
- Android 13+ release signer SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

Version 1.0.15 removes the visualizer's capture and transport stalls. Playback
audio is analyzed at its native frame cadence, redundant sends are eliminated,
and FFT working memory is reused instead of rebuilt every frame. Paired with
Screenify display 2.1.30, the LED matrix now reacts promptly without the stacked
slow envelopes that made the previous CAVA release feel delayed and choppy.

The APK binary is distributed through GitHub Releases rather than committed to
the repository.
