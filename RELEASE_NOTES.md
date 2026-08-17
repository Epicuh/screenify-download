## Screenify for Android 1.0.14

Official release-signed Android build for connecting a phone to a Screenify display.

### Changed

- Replaced the beta visualizer's custom spectrum processor with a CAVA-inspired
  dual-window FFT, logarithmic bands, automatic sensitivity, integral smoothing,
  gravity falloff, and peak hold.
- The Orange Pi now renders the spectrum as a GPU-driven, discrete OEM-style LED
  matrix at the display refresh rate, including dim cells and the red reference row.
- Added robust 2D fallback rendering for devices where WebGL is unavailable.
- Preserved the one-tap display connection introduced in version 1.0.13.

### Requirements

- Android 9 or newer
- Notification access for now-playing information
- A Screenify display on the same local network

### Security

- Android application backups are disabled.
- Normal media connection does not transmit an access secret.
- The app pins the Screenify device TLS certificate discovered on the local network.

### Verification

- APK SHA-256: `A9F9DA8BE075A2A1B7E74FB398C8A3AB2C45EEF9CDA55C654575A514DEFF7864`
- Android 9–12L signer SHA-256: `A7394529F660B0FBCEF43EE16F7823F582EE98C883E16BF8912426F9977FF297`
- Android 13+ signer SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

Google Play Protect may still show a first-time caution while the independently
distributed signing identity is new. Version 1.0.14 retains the platform-targeted
signing compatibility introduced in 1.0.12.
