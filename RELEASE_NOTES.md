## Screenify for Android 1.0.20

Official release-signed Android build for connecting a phone to a Screenify display.

### Changed

- Pixel-aligns the colored SETTINGS “S” with the SCREENIFY “S” using measurements
  from the original 1080×2340 screenshots.
- Replaces the font-based help close character with a centered vector X.
- Restores APK update checks through a published, integrity-pinned release manifest.
- Retains the TLS-pinned device-management and low-latency visualizer paths.

### Requirements

- Android 9 or newer
- Notification access for now-playing information
- A Screenify display on the same local network

### Security

- Android application backups are disabled.
- Normal media connection does not transmit an access secret.
- The app pins the Screenify device TLS certificate discovered on the local network.

### Verification

- APK SHA-256: `43D1481BA87BC92769B3CD3B82F92D71989DD85144DDD500A535D3558F296A76`
- Android 9–12L signer SHA-256: `A7394529F660B0FBCEF43EE16F7823F582EE98C883E16BF8912426F9977FF297`
- Android 13+ signer SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

Google Play Protect may still show a first-time caution while the independently
distributed signing identity is new. Version 1.0.20 retains the platform-targeted
signing compatibility introduced in 1.0.12.
