<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Android, iPhone and iPad

## iPhone and iPad

Install OYYO AI NotzUP version 1.0.27 from the official
[Apple App Store](https://apps.apple.com/app/id6826987959). No unofficial IPA is
distributed. iOS uses Apple permission interfaces such as AVFoundation and
ReplayKit. Approve only the microphone, camera, photo, file, notification or
screen permissions needed for the action you start.

## Android

Signed Android 1.0.0 build `1000026` is available from the official
[Android GitHub Release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.0-android).
Use the arm64 APK for most current phones or the universal APK when architecture
compatibility is uncertain. Google Play remains a closed test rather than a
public production channel. Verify the release checksum and signing-certificate
digest before allowing a source install.

Android uses a visible MediaProjection consent sheet for screen capture and a
foreground recording notification while a supported capture is active.

## Mobile capture limits

Mobile operating systems and source applications can restrict protected audio,
cellular calls and audio from other apps. NotzUP does not bypass those controls,
and capture from every source cannot be guaranteed. Always tell participants
and obtain the consent required by law. Authorized connected-service history is
a separate capability from native capture.
