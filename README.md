<div align="center">

<img src="assets/oyyo-notzup-hero.png" alt="OYYO NotzUP private local AI capture and knowledge workspace" width="100%">

# OYYO NotzUP

## Private capture, audio and music analysis, visual understanding and offline transcription in one workspace

**Capture anything. Understand it locally.**

[![Get it from Microsoft](https://img.shields.io/badge/Microsoft%20Store-Get%20OYYO%20AI%20NotzUP-0078D4?style=for-the-badge&logo=microsoft&logoColor=white)](https://apps.microsoft.com/detail/9NX0604FJ0XN)
[![Windows direct installer](https://img.shields.io/badge/Windows-Direct%20installer%20(unsigned)-2563EB?style=for-the-badge&logo=windows11&logoColor=white)](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.0-windows)
[![Android direct download](https://img.shields.io/badge/Android-Signed%20APK-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.0-android)
[![All verified releases](https://img.shields.io/badge/GitHub-Verified%20Releases-181717?style=for-the-badge&logo=github)](https://github.com/vpicciuolo/oyyo-notzup/releases)

[Download options](docs/DOWNLOADS.md) · [Windows Store](https://apps.microsoft.com/detail/9NX0604FJ0XN) · [Android 1.0.0 pre-release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.0-android) · [Recording-controls demo](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-NotzUP-Android-recording-controls-demo.mp4) · [NotzUP website](https://notzup.com/) · [OYYO ONE AI](https://oyyo.one/) · [Help & FAQ](docs/FAQ.md) · [Support](mailto:support@oyyo.one)

![Windows](https://img.shields.io/badge/Windows-10%20%7C%2011-2563EB?style=for-the-badge&logo=windows11&logoColor=white)
![Local processing](https://img.shields.io/badge/processing-on--device-059669?style=for-the-badge)
![Private core](https://img.shields.io/badge/source-proprietary-111827?style=for-the-badge)

</div>

OYYO NotzUP is the private capture and knowledge workspace inside **[OYYO ONE AI](https://oyyo.one/)** for Windows, macOS, Linux, Android and iOS. Record audio or a permitted screen, save screenshots, scan with the camera, import documents, images, music and video, or keep text and links. Then use on-device intelligence to transcribe speech, draft lyrics or spoken words, analyze music and sound, describe visuals, translate, search, summarize and turn each source into useful, reviewable work. Local originals remain under your control and stay on your device unless you explicitly choose a connected or online feature.

**Local OYYO AI Core — running privately on your device.**

> Official direct downloads appear only on the [GitHub Releases page](https://github.com/vpicciuolo/oyyo-notzup/releases). The Microsoft Store package is signed by Microsoft. Windows 1.0.0 direct EXE/MSI files are intentionally published **unsigned** as a separate manual-install option and can trigger Microsoft Defender SmartScreen. Never trust an installer copied to an unofficial host.

## Why NotzUP

- **More than a screen recorder:** audio, screen, screenshot, scan, file and text capture live together.
- **Private local intelligence:** supported transcription, OCR, search and grounded outputs run on the device, without a hidden cloud-model fallback.
- **A searchable source library:** find relevant transcript passages and return to their timestamped source context.
- **Useful outputs you control:** review summaries, explanations, actions, Markdown and JSON before exporting or sharing.
- **Audio and music understanding:** create review drafts of lyrics or spoken words and inspect duration, sample rate, channels, estimated tempo, tonal estimate and dynamic range.
- **Grounded visual understanding:** use a compatible verified local vision pack for scene descriptions, alt text and approved object labels.
- **Offline translation:** translate supported outputs with installed local language packs.
- **Real provider consent:** connect supported Google, Microsoft, Zoom and Slack services only when you choose.
- **Calendar and bookings:** review authorized calendars and booking activity in the same workspace.
- **Fast access:** desktop controls, tray/menu-bar actions, Android Quick Settings and purpose-built widgets keep capture close.

## Windows features

- Microphone audio recording and eligible Windows system-audio capture
- Screen/window recording through the Windows permission flow
- Screenshot capture and supported local OCR
- Broad PDF, Office, OpenDocument, text, image, audio and video import
- Offline speech transcription with a verified local model
- Review drafts of lyrics or spoken words from audio you are authorized to analyze
- Local music and sound facts including tempo, tonal estimate and dynamic range
- Grounded scene descriptions, alt text and approved object labels with a compatible local vision pack
- Offline translation with installed language packs
- Local transcript search with source context and citations
- Reviewable summaries, explanations, action items, Markdown and JSON
- Local SQLite metadata and OS application-data storage
- System-language detection plus an in-app language selector
- Consent-controlled privacy-safe analytics that excludes captured content

Feature availability depends on the operating system, hardware, source application, provider scopes and installed local models. Mobile operating systems can restrict capture of protected, cellular and third-party app audio.

## Download and verify

The [Download options](docs/DOWNLOADS.md) page is the canonical availability list. It keeps the Store and direct-download routes separate so you can choose the installation method that fits your device.

| Platform | Store channel | Direct GitHub download | Current availability |
| --- | --- | --- | --- |
| Windows 10/11 x64 | [Microsoft Store](https://apps.microsoft.com/detail/9NX0604FJ0XN) | [Setup EXE](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-windows/OYYO-NotzUP-1.0.0-Windows-x64-Setup.exe) · [MSI](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-windows/OYYO-NotzUP-1.0.0-Windows-x64.msi) | **Store available**; direct installers are unsigned and require manual approval on some PCs |
| macOS | Mac App Store | Signed and notarized DMG | In preparation |
| Android | Google Play (closed testing/review) | [Signed arm64 APK](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-AI-NotzUP-Android-1.0.0-arm64-v8a.apk) or [universal APK](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-android/OYYO-AI-NotzUP-Android-1.0.0-universal.apk) | Signed 1.0.0 pre-release available; public Play listing pending |
| iPhone and iPad | Apple App Store | No public sideload package | In preparation |
| Linux x64 | — | AppImage, DEB, RPM and CLI archive | VM validation passed; signing and publication pending |

The Windows Store link is the recommended trusted route. Other Store names become clickable only after the corresponding public listing exists. The Windows direct installers are provided for users who explicitly prefer a traditional setup wizard or MSI and understand that version 1.0.0 is not Authenticode-signed.

### Install Windows from the command line

Windows users can install the same Microsoft-signed Store package without opening the Store UI:

```powershell
winget install 9NX0604FJ0XN --source msstore --accept-package-agreements --accept-source-agreements
```

This command downloads OYYO AI NotzUP directly from Microsoft and avoids the warning shown by the unsigned direct installers.

### Install Windows with the traditional setup wizard

Download the [version 1.0.0 Setup EXE](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-windows/OYYO-NotzUP-1.0.0-Windows-x64-Setup.exe). It is the normal guided installer and includes the required WebView2 runtime for offline installation. The alternative [MSI](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-windows/OYYO-NotzUP-1.0.0-Windows-x64.msi) is intended for traditional or managed deployment.

Version 1.0.0 direct Windows installers are **not Authenticode-signed**. If Microsoft Defender SmartScreen appears, confirm that the file came from this repository, compare its SHA-256 checksum with the release checksum file, select **More info**, verify the displayed app name, and choose **Run anyway** only if you accept the unsigned-install risk. The dialog cannot show HRN INNOVATION TECHNOLOGIES LTD as a verified publisher until a trusted organization-validation certificate is available.

Every direct desktop release will include:

1. A versioned, immutable GitHub Release asset.
2. The signature status and any operating-system warning are disclosed beside the download.
3. SHA-256 checksums and release notes.
4. A statement of supported operating-system versions and architectures.
5. Stable file naming for MSI, EXE, DMG, APK, AppImage, DEB and CLI packages where applicable.

## Quick start

1. Install Windows from the [Microsoft Store](https://apps.microsoft.com/detail/9NX0604FJ0XN), or choose another live package on the [Download options](docs/DOWNLOADS.md) page.
2. For a direct Android APK, compare its SHA-256 checksum and signing-certificate digest with the tagged release. For a direct Windows installer, compare the SHA-256 checksum and review the unsigned-install warning before manually approving SmartScreen.
3. Open NotzUP and approve only the microphone, screen, camera or notification permissions needed for the capture you choose.
4. Allow the verified local speech model to download and pass integrity verification on first use.
5. Select **Capture anything**, choose a source, name the session and start.
6. Stop and save, then review the original, transcript and selected outputs in **Library**.

See the detailed [Getting Started guide](docs/GETTING_STARTED.md) and [desktop installation guide](docs/INSTALL_DESKTOP.md).

## Common workflows

### Record and transcribe a meeting without a bot

Choose **Audio** for microphone capture or **Screen recording** when you need a permitted app/window and eligible system audio. Keep the recording indicator visible, stop and save, then run the verified local transcription model. Always obtain participant consent and follow applicable recording law and workplace policy.

### Turn a document or screenshot into useful notes

Choose **Screenshot**, **Scan** or **Import a file**. Select the outputs you want—such as extracted text, summary, explanation, actions or Markdown—and review the evidence before exporting.

### Analyze audio and music locally

Import audio or music you are permitted to analyze. NotzUP can create a tentative lyrics or spoken-word draft and report grounded sound facts such as duration, sample rate, channels, estimated tempo, tonal estimate and dynamic range. Review every draft against the original: sung-word recognition can be unreliable over instruments or background audio, and NotzUP does not fetch or reproduce third-party lyrics catalogs.

### Describe visuals and translate offline

Open an imported image, screenshot or camera scan with a compatible verified local vision pack to produce a scene description, alt text and approved object labels. Installed language packs can translate supported outputs without sending the captured source to a cloud inference service.

### Summarize any supported source

From the source result, choose the outputs you need: summary, explanation, action items, clean text, Markdown or structured JSON. Each output stays tied to the source so you can review it before exporting or sharing.

### Search your private capture library

Open **Library** and search for a person, phrase, decision or topic. NotzUP searches supported local transcript text and surrounding passages on the device.

### Connect a calendar or content service

Open **Connectors**, select a provider and review the requested permissions. The provider’s OAuth screen controls consent. Available data depends on the scopes and administrator policy for that account.

## Privacy at a glance

- Local recordings and imported media remain on the device unless you explicitly choose an online feature.
- Supported local processing is performed on the device.
- Optional synced storage is separate from local capture and is user controlled.
- Analytics is opt-in/choice controlled and excludes recordings, transcripts, notes, searches, file names, calendar details and account details.
- NotzUP does not silently create provider connections or bypass operating-system capture controls.

[Privacy Policy](https://oyyo.one/privacy) · [Terms of Service](https://oyyo.one/terms) · [Security reporting](SECURITY.md)

## Support

- Product help: [NotzUP FAQ](docs/FAQ.md)
- Email: [support@oyyo.one](mailto:support@oyyo.one)
- Bugs and feature requests without private data: [GitHub Issues](https://github.com/vpicciuolo/oyyo-notzup/issues)
- Security concerns: follow [SECURITY.md](SECURITY.md); do not post secrets, recordings or personal data in a public issue.

## Product and publisher

OYYO NotzUP is developed as part of **[OYYO ONE AI](https://oyyo.one/)** by **[HRN INNOVATION TECHNOLOGIES LTD](https://hrn.ae/)**. NotzUP is not affiliated with Google, Microsoft, Zoom, Slack, OpenAI or Anthropic. Provider names and marks identify optional compatible integrations and remain the property of their respective owners.

**[© 2026 HRN INNOVATION TECHNOLOGIES LTD](https://hrn.ae/)**


