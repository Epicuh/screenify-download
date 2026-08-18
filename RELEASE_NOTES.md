## Screenify for Android 1.0.16

Official release-signed Android build for connecting a phone to a Screenify display.

### Changed

- Separated continuous playback capture from FFT analysis so audio capture never
  stalls behind rendering work.
- Analysis consumes the newest complete sample window and skips stale intermediate
  work after a scheduler delay instead of transmitting a late burst.
- Reuses the pinned TLS connection and drains bridge responses so visualizer frames
  do not pay for a new TCP/TLS handshake.
- Caches compact artwork payloads so unchanged album art is not decoded and
  recompressed on the visualizer's timing path.
- Screenify display 2.1.32 caps every LED and peak inside the physical canvas,
  permanently hides the cursor, and prevents background printing services from
  taking display CPU time.

### Requirements

- Android 9 or newer
- Notification access for now-playing information
- A Screenify display on the same local network

### Security

- Android application backups are disabled.
- Normal media connection does not transmit an access secret.
- The app pins the Screenify device TLS certificate discovered on the local network.

### Verification

- APK SHA-256: `C725F42500AB3FE521C2A54DE14036E68E540FBA1A9021D2A77490B8723F4038`
- Android 9–12L signer SHA-256: `A7394529F660B0FBCEF43EE16F7823F582EE98C883E16BF8912426F9977FF297`
- Android 13+ signer SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

Google Play Protect may still show a first-time caution while the independently
distributed signing identity is new. Version 1.0.16 retains the platform-targeted
signing compatibility introduced in 1.0.12.
