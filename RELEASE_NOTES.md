## Screenify for Android 1.0.15

Official release-signed Android build for connecting a phone to a Screenify display.

### Changed

- Fixed the root cause of bursty visualizer updates: playback capture no longer
  waits for a 4,096-sample read before processing each hop.
- Sends each source frame once at its native cadence instead of combining an
  immediate path with a separate timer that resent duplicate frames.
- Reuses FFT windows and buffers, removing continuous per-frame allocation and
  trigonometric setup from the audio thread.
- Screenify display 2.1.30 removes the duplicate slow envelope and peak hold,
  while retaining short interpolation between real audio frames for fluid motion.
- Centered the idle "No music is playing" screen in portrait display mode.

### Requirements

- Android 9 or newer
- Notification access for now-playing information
- A Screenify display on the same local network

### Security

- Android application backups are disabled.
- Normal media connection does not transmit an access secret.
- The app pins the Screenify device TLS certificate discovered on the local network.

### Verification

- APK SHA-256: `1A0862D231A346BF1A3D66D99ED56B5F20E828A957DF4F8422C3EC6F04B10DB3`
- Android 9–12L signer SHA-256: `A7394529F660B0FBCEF43EE16F7823F582EE98C883E16BF8912426F9977FF297`
- Android 13+ signer SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

Google Play Protect may still show a first-time caution while the independently
distributed signing identity is new. Version 1.0.15 retains the platform-targeted
signing compatibility introduced in 1.0.12.
