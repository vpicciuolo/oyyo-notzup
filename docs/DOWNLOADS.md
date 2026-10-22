<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Download OYYO NotzUP

This page lists every official OYYO NotzUP installation channel. Store packages and direct packages are separate distribution routes, and their signature status is stated beside each download.

**Local OYYO AI Core — running privately on your device.**

## Current availability

OYYO NotzUP is available for Windows from the official [Microsoft Store](https://apps.microsoft.com/detail/9NX0604FJ0XN). A traditional Windows Setup EXE and MSI are also available on the [Windows 1.0.0 GitHub Release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.0-windows); those two direct installers are intentionally unsigned and can trigger SmartScreen. A signed Android 1.0.0 pre-release is available on the public [Android GitHub Release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.0-android); Google Play certification is still in progress. macOS, iOS and Linux production packages are not public yet. Do not install a copy hosted outside this repository, the relevant platform Store, or [notzup.com](https://notzup.com/).

| Platform | Store installation | Direct installation | Status |
| --- | --- | --- | --- |
| Windows 10/11 x64 | [Get OYYO AI NotzUP from Microsoft Store](https://apps.microsoft.com/detail/9NX0604FJ0XN) | [Setup EXE](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-windows/OYYO-NotzUP-1.0.0-Windows-x64-Setup.exe) · [MSI](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-windows/OYYO-NotzUP-1.0.0-Windows-x64.msi) | **Available**; direct installers are unsigned and may require manual SmartScreen approval |
| macOS | Mac App Store link appears here after review | `OYYO-NotzUP-macOS-universal.dmg` | Requires Apple Developer ID signing and notarization |
| Android | Google Play link appears here after review | [arm64-v8a APK](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-AI-NotzUP-Android-1.0.0-arm64-v8a.apk) · [universal APK](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-AI-NotzUP-Android-1.0.0-universal.apk) | Signed 1.0.0 pre-release; Play closed testing/review in progress |
| iPhone and iPad | Apple App Store link appears here after review | Not offered as a public sideload package | In preparation |
| Linux x64 | — | `OYYO-NotzUP-Linux-x86_64.AppImage` and `.deb` | In preparation |
| Command line | — | Windows, macOS and Linux CLI archives | In preparation |

## Windows

The free Microsoft Store route uses an MSIX package signed and hosted through Microsoft. The public listing is live:

**[Download OYYO AI NotzUP from Microsoft Store](https://apps.microsoft.com/detail/9NX0604FJ0XN)**

Or install the same Microsoft-signed Store package from a terminal:

```powershell
winget install 9NX0604FJ0XN --source msstore --accept-package-agreements --accept-source-agreements
```

Windows Package Manager identifies this package as **OYYO AI NotzUP**, Store product ID `9NX0604FJ0XN`. Microsoft remains the download and signing channel for this command.

GitHub Releases also offers these direct Windows formats:

- **MSIX** for a packaged Windows installation.
- **[Setup EXE](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-windows/OYYO-NotzUP-1.0.0-Windows-x64-Setup.exe)** for the normal guided desktop installation.
- **[MSI](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-windows/OYYO-NotzUP-1.0.0-Windows-x64.msi)** for traditional or managed deployment.

The Store package and direct MSI/EXE installers are different distribution channels. Microsoft Store certification does not automatically sign a separately hosted MSI or EXE. The version 1.0.0 MSI and EXE have Authenticode status `NotSigned`, so Windows can show Microsoft Defender SmartScreen and identify the publisher as unknown. Their hashes are published in [the Windows release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.0-windows).

For the simplest traditional installation, download the Setup EXE. If SmartScreen appears:

1. Confirm that the address is `github.com/vpicciuolo/oyyo-notzup` and that the file name is `OYYO-NotzUP-1.0.0-Windows-x64-Setup.exe`.
2. Compare the file's SHA-256 hash with `SHA256SUMS-windows.txt` in the same release.
3. Select **More info** in SmartScreen.
4. Confirm the app name and choose **Run anyway** only if you accept the unsigned-install risk.

The Store or WinGet route remains recommended when you want a Microsoft-signed installation without this warning.

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
3. Review the disclosed signature status. Windows 1.0.0 direct installers are unsigned; the Android APKs are signed.
4. Compare the file's SHA-256 hash with `SHA256SUMS.txt` in the same release.
5. Delete the file and contact [support@oyyo.one](mailto:support@oyyo.one) if any check fails.

PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 -Path '.\OYYO-NotzUP-1.0.0-Windows-x64-Setup.exe'
Get-AuthenticodeSignature -FilePath '.\OYYO-NotzUP-1.0.0-Windows-x64-Setup.exe' |
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
- Direct binaries include checksums, release notes and an explicit signature-status disclosure.
- Unsigned builds are clearly separated from the Microsoft-signed Store channel and require an informed manual choice.
- Every release identifies the supported operating-system versions and architectures.
- Older versions remain on their tagged release page unless removed for a security or legal reason.

[NotzUP website](https://notzup.com/) · [OYYO ONE AI](https://oyyo.one/) · [Release history](https://github.com/vpicciuolo/oyyo-notzup/releases) · [Support](mailto:support@oyyo.one)

