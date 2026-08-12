## Screenify for Android 1.0.10

Official release-signed Android build for connecting a phone to a Screenify display.

### Requirements

- Android 9 or newer
- Notification access for now-playing information
- A Screenify display on the same local network

### Security

- Android application backups are disabled.
- Device access secrets are protected with Android Keystore.
- The app verifies the Screenify device pairing proof and pins its TLS certificate.

### Verification

- APK SHA-256: `B76D41C8C9E003056B6CB5A27D357452B4C63FF188BC3C2596AD155E2A55BC80`
- Signing certificate SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

If an older debug-signed development APK is installed, Android may require it to
be uninstalled before this release-signed build can be installed.
