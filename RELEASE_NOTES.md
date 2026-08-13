## Screenify for Android 1.0.12

Official release-signed Android build for connecting a phone to a Screenify display.

### Fixed

- Corrected the signing migration for Android 9 through Android 12L by retaining
  the exact original signer on those platform versions.
- Android 13 and newer use Screenify's permanent release signer with a
  cryptographically verified lineage from the original signer.
- Raised the Android version code to 13 to prevent a same-version update rejection.
- Preserves installed Screenify app data across the authorized transition.

### Requirements

- Android 9 or newer
- Notification access for now-playing information
- A Screenify display on the same local network

### Security

- Android application backups are disabled.
- Device access secrets are protected with Android Keystore.
- The app verifies the Screenify device pairing proof and pins its TLS certificate.

### Verification

- APK SHA-256: `AF0C0D0EF2E4BAC2475346E74506231CE78918A8EDACC2FCD6691BCBF5F05D68`
- Android 9–12L signer SHA-256: `A7394529F660B0FBCEF43EE16F7823F582EE98C883E16BF8912426F9977FF297`
- Android 13+ signer SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

Google Play Protect may still show a first-time caution while the independently
distributed signing identity is new. Version 1.0.12 fixes the separate Android
platform compatibility issue that could cause installation to fail after approval.
