<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Download OYYO NotzUP

This page lists every official OYYO NotzUP installation channel. A button or package name becomes a download link only after that Store listing or signed release has passed its release gate.

**Local OYYO AI Core — running privately on your device.**

## Current availability

OYYO NotzUP is in release preparation. A signed Android 1.0.0 pre-release is available on the public [GitHub Release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.0-android); Google Play certification is still in progress. Windows, macOS, iOS and Linux direct production packages are not public yet. Do not install an unsigned build or a copy hosted outside this repository, the relevant platform Store, or [notzup.com](https://notzup.com/).

| Platform | Store installation | Direct installation | Status |
| --- | --- | --- | --- |
| Windows 10/11 x64 | Microsoft Store link appears here after certification | `OYYO-NotzUP-Windows-x64.msix`, `.msi`, and `.exe` release assets | Store MSIX in preparation; direct MSI/EXE require a valid production signature |
| macOS | Mac App Store link appears here after review | `OYYO-NotzUP-macOS-universal.dmg` | Requires Apple Developer ID signing and notarization |
| Android | Google Play link appears here after review | [arm64-v8a APK](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-AI-NotzUP-Android-1.0.0-arm64-v8a.apk) · [universal APK](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-AI-NotzUP-Android-1.0.0-universal.apk) | Signed 1.0.0 pre-release; Play closed testing/review in progress |
| iPhone and iPad | Apple App Store link appears here after review | Not offered as a public sideload package | In preparation |
| Linux x64 | — | `OYYO-NotzUP-Linux-x86_64.AppImage` and `.deb` | In preparation |
| Command line | — | Windows, macOS and Linux CLI archives | In preparation |

## Windows

The free Microsoft Store route uses an MSIX package that Microsoft signs and hosts after certification. The public listing will be linked here when it is live.

GitHub Releases will also offer direct formats when their separate release gates pass:

- **MSIX** for a packaged Windows installation.
- **MSI** for managed and traditional desktop deployment.
- **EXE** for the guided desktop installer.

The Store package and direct MSI/EXE installers are different distribution channels. Microsoft Store certification does not automatically sign a separately hosted MSI or EXE.

## macOS

The Mac App Store listing will be linked here after review. A direct universal DMG will be published only after it is signed with the approved Apple Developer ID, notarized by Apple and verified on supported Intel and Apple silicon devices.

## Android

The Google Play listing will be linked here after review. The signed Android 1.0.0 pre-release is available from the [tagged GitHub Release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.0-android): use the [arm64-v8a APK](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-AI-NotzUP-Android-1.0.0-arm64-v8a.apk) for most current phones or the larger [universal APK](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-AI-NotzUP-Android-1.0.0-universal.apk) when architecture compatibility is uncertain. Watch the [real recording-controls demonstration](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-NotzUP-Android-recording-controls-demo.mp4) for the Android consent flow, screen and microphone foreground services, floating control, and persistent notification controls.

The published APKs use Android signature scheme v2. Verify the release checksum and signing-certificate SHA-256 digest `903bf05e2578775a0c66e85f540b6dd36cf6f55c5d9f1f3896eb72b6ad18c15b`. The APK signature must match future direct updates; never install an APK copied to another host.

## iPhone and iPad

The Apple App Store is the supported public installation route. OYYO does not publish an unofficial iOS sideload package.

## Linux and CLI

Linux GUI releases are planned as an AppImage and DEB package. CLI archives will be labeled by operating system and architecture. Each direct package will include a SHA-256 checksum.

## Verify a direct download

1. Open the matching entry on the [GitHub Releases page](https://github.com/vpicciuolo/oyyo-notzup/releases).
2. Confirm the asset name, version, operating system and architecture.
3. Verify the platform signature or notarization result where applicable.
4. Compare the file's SHA-256 hash with `SHA256SUMS.txt` in the same release.
5. Delete the file and contact [support@oyyo.one](mailto:support@oyyo.one) if any check fails.

PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 -Path '.\OYYO-NotzUP-Windows-x64.msi'
Get-AuthenticodeSignature -FilePath '.\OYYO-NotzUP-Windows-x64.msi' |
  Format-List Status, StatusMessage, SignerCertificate, TimeStamperCertificate
```

macOS:

```bash
shasum -a 256 OYYO-NotzUP-macOS-universal.dmg
spctl --assess --type open --context context:primary-signature -vv OYYO-NotzUP-macOS-universal.dmg
```

Linux or Android package checksum:

```bash
sha256sum OYYO-NotzUP-Linux-x86_64.AppImage
sha256sum OYYO-AI-NotzUP-Android-1.0.0-arm64-v8a.apk
sha256sum OYYO-AI-NotzUP-Android-1.0.0-universal.apk
```

## Release policy

- Store links are published only after the listing is public.
- Direct binaries are published only after signature, checksum, malware-scan and installation tests pass.
- Preview and unsigned builds stay clearly separated from production downloads.
- Every release identifies the supported operating-system versions and architectures.
- Older versions remain on their tagged release page unless removed for a security or legal reason.

[NotzUP website](https://notzup.com/) · [OYYO ONE AI](https://oyyo.one/) · [Release history](https://github.com/vpicciuolo/oyyo-notzup/releases) · [Support](mailto:support@oyyo.one)

