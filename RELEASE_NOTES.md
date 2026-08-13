## Screenify for Android 1.0.11

Official release-signed Android build for connecting a phone to a Screenify display.

### Fixed

- Fixed Android's `App not installed` error when upgrading from the earlier
  development-signed Screenify APK.
- Added a cryptographically verified signing-certificate lineage from the old
  development identity to Screenify's permanent release identity.
- Preserves installed Screenify app data during the authorized key transition.

### Requirements

- Android 9 or newer
- Notification access for now-playing information
- A Screenify display on the same local network

### Security

- Android application backups are disabled.
- Device access secrets are protected with Android Keystore.
- The app verifies the Screenify device pairing proof and pins its TLS certificate.

### Verification

- APK SHA-256: `115167DAC7DDA3D49CAC34EB911BAD4AA9D453A61A06F568D800E33BB4A10B38`
- Signing certificate SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

Google Play Protect may still show a first-time caution while the independently
distributed signing identity is new. Version 1.0.11 fixes the separate Android
signature mismatch that caused installation to fail after approval.
