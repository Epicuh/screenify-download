## Screenify for Android 1.0.17

Official release-signed Android build for connecting a phone to a Screenify display.

### Changed

- Replaces phone-side FFT analysis with a low-latency stereo PCM stream to native
  CAVA on the Screenify display.
- Keeps music playing through the phone, connected speakers, Bluetooth, or earbuds;
  playback capture is a parallel analysis tap and does not reroute the audio.
- Protects the audio stream with the already paired, certificate-pinned TLS channel.
- Uses 10 ms capture chunks, a bounded 80 ms phone queue, stale-frame rejection,
  TCP no-delay, and server-side backpressure dropping to prevent latency buildup.
- Screenify display 2.1.37 paces 11-band output at 60 FPS, keeps levels on-screen,
  supervises the native process, and includes the exact patched CAVA source.

### Requirements

- Android 9 or newer
- Notification access for now-playing information
- A Screenify display on the same local network

### Security

- Android application backups are disabled.
- Normal media connection does not transmit an access secret.
- The app pins the Screenify device TLS certificate discovered on the local network.

### Verification

- APK SHA-256: `5DAB7C8336263D396D5A6CF92178B1376CFFA8D585C149483176C90E0C532865`
- Android 9–12L signer SHA-256: `A7394529F660B0FBCEF43EE16F7823F582EE98C883E16BF8912426F9977FF297`
- Android 13+ signer SHA-256: `91D68FB62E91ED14CF7A605113154BBE9FF85696B5CF50352CD518BFCB69FA70`

Google Play Protect may still show a first-time caution while the independently
distributed signing identity is new. Version 1.0.17 retains the platform-targeted
signing compatibility introduced in 1.0.12.
