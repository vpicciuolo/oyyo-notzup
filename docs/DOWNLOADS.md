<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Download OYYO NotzUP

This page lists every official OYYO NotzUP installation channel. Store packages and direct packages are separate distribution routes, and their signature status is stated beside each download.

**Local OYYO AI Core — running privately on your device.**

## Current availability

OYYO NotzUP is available for Windows from the official [Microsoft Store](https://apps.microsoft.com/detail/9NX0604FJ0XN) and for Linux from the public [Snap Store listing](https://snapcraft.io/oyyo-notzup) on the `latest/edge` channel. A traditional Windows Setup EXE and MSI are also available on the [Windows 1.0.0 GitHub Release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.0-windows); those two direct installers are intentionally unsigned and can trigger SmartScreen. A universal macOS `0.1.0-alpha.1` functional-test DMG is available on the [macOS test release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v0.1.0-alpha.1-macos); it is ad-hoc signed, not notarized by Apple and requires an informed Gatekeeper override. Signed Android 1.0.0 build `1000026` is available on the public [Android GitHub Release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.0-android). The same build has been submitted to Google Play closed testing; public production access is not yet available. Linux x86-64 GUI and CLI packages are available on the [Linux 1.0.27.0 GitHub Release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.27.0-linux). macOS and iOS production Store packages are not public yet. Do not install a copy hosted outside this repository, the relevant platform Store, or [notzup.com](https://notzup.com/).

| Platform | Store installation | Direct installation | Status |
| --- | --- | --- | --- |
| Windows 10/11 x64 | [Get OYYO AI NotzUP from Microsoft Store](https://apps.microsoft.com/detail/9NX0604FJ0XN) | [Setup EXE](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-windows/OYYO-NotzUP-1.0.0-Windows-x64-Setup.exe) · [MSI](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-windows/OYYO-NotzUP-1.0.0-Windows-x64.msi) | **Available**; direct installers are unsigned and may require manual SmartScreen approval |
| macOS 10.15+; Intel or Apple silicon | Mac App Store link appears here after review | [Universal `0.1.0-alpha.1` test DMG](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v0.1.0-alpha.1-macos/OYYO-NotzUP-0.1.0-alpha.1-macOS-universal-test.dmg) | **Test pre-release available**; ad-hoc signed, not notarized, manual Gatekeeper approval required |
| Android | Google Play link appears here after review | [arm64-v8a APK](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-AI-NotzUP-Android-1.0.0-arm64-v8a.apk) · [universal APK](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-AI-NotzUP-Android-1.0.0-universal.apk) | Signed 1.0.0 build 1000026; the same build is in Play closed-test review |
| iPhone and iPad | Apple App Store link appears here after review | Not offered as a public sideload package | In preparation |
| Linux x64 | [Get OYYO NotzUP from the Snap Store (`latest/edge`)](https://snapcraft.io/oyyo-notzup) | [AppImage](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.27.0-linux/OYYO-NotzUP-1.0.27.0-Linux-x86_64.AppImage) · [DEB](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.27.0-linux/OYYO-NotzUP-1.0.27.0-Linux-x86_64.deb) · [RPM](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.27.0-linux/OYYO-NotzUP-1.0.27.0-Linux-x86_64.rpm) · [Snap](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.27.0-linux/OYYO-NotzUP-1.0.27.0-Linux-x86_64.snap) | **1.0.27.0 direct release**; build, tests, checksums, package metadata and virtual-display launch passed; physical permission QA remains |
| Command line | — | [Linux x86-64 CLI archive](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.27.0-linux/OYYO-NotzUP-CLI-1.0.27.0-Linux-x86_64.tar.gz) | **1.0.27.0 available**; CLI help and checksum verification passed |

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

The [macOS `0.1.0-alpha.1` test release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v0.1.0-alpha.1-macos) contains a universal DMG for Intel and Apple silicon Macs running macOS 10.15 or later. The build completed universal compilation, ad-hoc code-signature verification, DMG verification and a launch smoke test on a GitHub-hosted Mac. It has **not** been signed with an Apple Developer ID and has **not** been notarized by Apple. It is provided only for informed functional testing.

Download both files:

- [OYYO-NotzUP-0.1.0-alpha.1-macOS-universal-test.dmg](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v0.1.0-alpha.1-macos/OYYO-NotzUP-0.1.0-alpha.1-macOS-universal-test.dmg)
- [SHA256SUMS-macos.txt](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v0.1.0-alpha.1-macos/SHA256SUMS-macos.txt)

Before opening the DMG, verify it:

```bash
shasum -a 256 OYYO-NotzUP-0.1.0-alpha.1-macOS-universal-test.dmg
```

The result must be `1cfb137867c6c452df3f8461e3c6d5ce90c1dc6bd4d852095021d564b905d8eb`. If it differs, delete the download and contact support.

Double-click the verified DMG, drag **OYYO NotzUP** to **Applications**, eject the image, and launch the installed application. Because this test build is not notarized, macOS may block the first launch. Only after checking the release URL and SHA-256 value, try opening it once and then use **System Settings → Privacy & Security → Open Anyway**. Never override a warning that says the application is damaged or contains malware.

See [Install and run OYYO NotzUP on macOS](INSTALL_MACOS.md) for permission setup, first capture, troubleshooting, updating and uninstalling. The production direct-download build will replace this test route after Apple Developer ID signing, notarization and physical-device QA. The Mac App Store listing will be linked here only after Apple review.

## Android

The Google Play listing will be linked here after review. Signed Android 1.0.0 build `1000026` is available from the [tagged GitHub Release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.0-android): use the [arm64-v8a APK](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-AI-NotzUP-Android-1.0.0-arm64-v8a.apk) for most current phones or the larger [universal APK](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-AI-NotzUP-Android-1.0.0-universal.apk) when architecture compatibility is uncertain. Watch the [real recording-controls demonstration](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-NotzUP-Android-recording-controls-demo.mp4) for the Android consent flow, screen and microphone foreground services, floating control, and persistent notification controls.

Build `1000026` SHA-256:

- arm64-v8a: `790e22fc9e76941cfa6dfa490c5f95434fe018644dad1427f453292da8ed8881`
- universal: `639a4c9220c251dca440b2e97ebbec787605aab91bf6fbd097f6ff21d649d829`

The published APKs use Android signature scheme v2. Verify the release checksum and signing-certificate SHA-256 digest `903bf05e2578775a0c66e85f540b6dd36cf6f55c5d9f1f3896eb72b6ad18c15b`. The APK signature must match future direct updates; never install an APK copied to another host.

## iPhone and iPad

The Apple App Store is the supported public installation route. OYYO does not publish an unofficial iOS sideload package.

## Linux and CLI

The public [Snap Store listing](https://snapcraft.io/oyyo-notzup) provides both
the graphical app and the `oyyo-notzup.cli` command. Version 1.0.0 is currently
published to `latest/edge` while physical Linux permission QA continues:

```bash
sudo snap install oyyo-notzup --edge
```

Snaps installed from the Store receive automatic updates. The direct Snap below
is a separate unsigned preview artifact and requires `--dangerous`; prefer the
Store installation unless you specifically need the downloaded package.

Linux x86-64 AppImage, DEB, RPM, Snap and standalone CLI packages are available
from the [version 1.0.27.0 Linux release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.27.0-linux).
The DEB and RPM include `oyyo-notzup-cli`; the Snap exposes
`oyyo-notzup.cli`. Clean VM installation and runtime checks passed, including
the confined Snap GUI. These direct packages are not distribution-store or
code signed. Verify them with the published
[SHA-256 manifest](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.27.0-linux/SHA256SUMS-linux.txt).
Physical Linux audio, camera, screen-capture and portal testing still remains.
See the
[Linux installation guide](INSTALL_LINUX.md) and
[distribution-channel plan](LINUX_DISTRIBUTION.md).

## Verify a direct download

1. Open the matching entry on the [GitHub Releases page](https://github.com/vpicciuolo/oyyo-notzup/releases).
2. Confirm the asset name, version, operating system and architecture.
3. Review the disclosed signature status. Windows and Linux 1.0.0 direct packages are unsigned; the macOS test DMG is ad-hoc signed and not notarized; the Android APKs are signed.
4. Compare the file's SHA-256 hash with the checksum manifest in the same release.
5. Delete the file and contact [support@oyyo.one](mailto:support@oyyo.one) if any check fails.

PowerShell:

```powershell
Get-FileHash -Algorithm SHA256 -Path '.\OYYO-NotzUP-1.0.0-Windows-x64-Setup.exe'
Get-AuthenticodeSignature -FilePath '.\OYYO-NotzUP-1.0.0-Windows-x64-Setup.exe' |
  Format-List Status, StatusMessage, SignerCertificate, TimeStamperCertificate
```

macOS:

```bash
shasum -a 256 OYYO-NotzUP-0.1.0-alpha.1-macOS-universal-test.dmg
spctl --assess --type open --context context:primary-signature -vv OYYO-NotzUP-0.1.0-alpha.1-macOS-universal-test.dmg
```

Linux or Android package checksum:

```bash
sha256sum OYYO-NotzUP-1.0.27.0-Linux-x86_64.AppImage
sha256sum OYYO-NotzUP-1.0.27.0-Linux-x86_64.deb
sha256sum OYYO-NotzUP-1.0.27.0-Linux-x86_64.rpm
sha256sum OYYO-AI-NotzUP-Android-1.0.0-arm64-v8a.apk
sha256sum OYYO-AI-NotzUP-Android-1.0.0-universal.apk
```

## Release policy

- Store links are published only after the listing is public; pre-stable channels such as Snap `latest/edge` are labeled explicitly.
- Direct binaries include checksums, release notes and an explicit signature-status disclosure.
- Unsigned and non-notarized test builds are clearly separated from signed Store or production channels and require an informed manual choice.
- Every release identifies the supported operating-system versions and architectures.
- Older versions remain on their tagged release page unless removed for a security or legal reason.

[NotzUP website](https://notzup.com/) · [OYYO ONE AI](https://oyyo.one/) · [Release history](https://github.com/vpicciuolo/oyyo-notzup/releases) · [Support](mailto:support@oyyo.one)

