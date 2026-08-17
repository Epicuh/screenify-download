## Screenify for Android 1.0.13

Official release-signed Android build for connecting a phone to a Screenify display.

### Changed

- Connecting is now one tap: choose the Orange Pi from Find Device without
  entering a device access code.
- Increased the initial encrypted connection timeout so first-time TLS setup does
  not report a false request failure.
- The app pins the TLS certificate advertised by local device discovery.
- Administrative actions such as updates, orientation, and Wi-Fi management
  remain protected by the admin access code.

### Requirements

- Android 9 or newer
- Notification access for now-playing information
- A Screenify display on the same local network

### Security

- Android application backups are disabled.
- Normal media connection does not transmit an access secret.
- The app pins the Screenify device TLS certificate discovered on the local network.

### Verification

- APK SHA-256: `7CD1723BD523D21F73295F8F7C5440F12EE66DAE47EAD4629F4E93595829AC43`
- Android 9–12L signer SHA-256: `A7394529F660B0FBCEF43EE16F7823F582EE98C883E16BF8912426F9977FF297`
- Android 13+ signer SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

Google Play Protect may still show a first-time caution while the independently
distributed signing identity is new. Version 1.0.13 retains the platform-targeted
signing compatibility introduced in 1.0.12.
