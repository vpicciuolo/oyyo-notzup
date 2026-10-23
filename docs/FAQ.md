<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# OYYO NotzUP FAQ

## What is OYYO NotzUP?

OYYO NotzUP is the private capture and knowledge app inside [OYYO ONE AI](https://oyyo.one/). It brings audio recording, permitted screen capture, screenshots, scans, file import, text capture, offline transcription, local search, calendar activity and authorized provider connectors into one workspace.

**Local OYYO AI Core — running privately on your device.**

## Is NotzUP only for meetings?

No. It can help with meetings, calls, classes, interviews, voice notes, product walkthroughs, documents, whiteboards, research, saved web references and other material you are allowed to capture.

## Does NotzUP upload my recordings for AI processing?

Supported transcription, extraction, search and generated outputs run on the device. There is no hidden cloud-inference fallback. Optional account sync and storage are separate features that require the user’s choice and remain subject to the plan and privacy policy.

## Can NotzUP analyze music or create a lyrics draft?

For audio or music you are permitted to analyze, NotzUP can create a tentative lyrics or spoken-word draft and report grounded sound facts such as duration, sample rate, channels, estimated tempo, tonal estimate and dynamic range. Sung-word recognition can be unreliable over instruments or background audio, so review the draft against the original. NotzUP does not fetch or reproduce third-party lyrics catalogs.

## Can NotzUP describe images?

Yes, when a compatible verified local vision pack is installed. Imported images, screenshots and camera scans can produce a scene description, alt text and approved object labels locally on the device.

## Can NotzUP summarize or translate captured material?

Supported sources can produce reviewable summaries, explanations, action items, clean text, Markdown and structured JSON. Installed local language packs can translate supported outputs offline. Every generated result remains tied to its captured source for review.

## Can I use NotzUP without an account?

The desktop app includes a limited guest capture mode for evaluation. Account features such as registered-device entitlements, bookings, notifications, connectors and optional sync require sign-in.

## What can the Windows app capture?

The Windows app supports microphone recording, permitted screen/window capture, eligible system audio, screenshots, scans, text/links and supported file imports. Availability depends on Windows permissions, device drivers and whether the source application allows capture.

## Can it record every call or protected stream?

No app can truthfully guarantee that. Windows, Android, iOS and the source application may restrict protected audio, cellular calls, VoIP audio or copyrighted media. NotzUP never bypasses operating-system permissions or source-app protections. Obtain participant consent before recording.

## Does it work with Zoom, Google Meet and Microsoft Teams?

NotzUP can capture eligible device audio/screen sources and can connect to supported provider data through the provider’s official authorization flow. Native capture and provider-history import are different features. What is available depends on the operating system, provider scopes, account plan and administrator policy.

## Which files can I import?

The desktop release supports common PDF, Office, OpenDocument, RTF, HTML, Markdown, CSV/TSV, JSON/XML/YAML, caption, image, audio and video formats. Extraction quality depends on the file, embedded text, installed codecs and verified local models.

## What does “local intelligence” mean?

It means the supported model or extractor runs on your device. NotzUP verifies trusted downloadable model assets by size and cryptographic hash before use. Some optional capabilities can remain unavailable until their redistributable model and runtime pass the release gate.

## Is offline transcription available?

Yes, after the verified local speech model is installed. The first model download needs an internet connection; transcription then runs locally for supported formats and languages.

## Can I search recordings and transcripts?

Yes. Library search works on supported local transcript text and surrounding passages. Where timing data exists, results preserve source context and citations so you can return to the original moment.

## Which languages are supported?

The app follows the operating-system language by default and includes an in-app selector. Multilingual interface coverage and speech-language behavior vary by release; unsupported regional variants fall back safely to their base language or English. The Store listing declares only languages that have completed release QA.

## How do notifications work?

Account and booking events appear in NotzUP’s notification center. On supported registered devices, and when system permission is granted, eligible events can also appear as operating-system notifications. Selecting a booking notification routes to Calendar/Bookings rather than an unrelated page.

## Where should I download NotzUP?

Use only the relevant platform store or the official [GitHub Releases page](https://github.com/vpicciuolo/oyyo-notzup/releases). Direct builds are official only when the tagged release explicitly lists the same file name, version, architecture, signature status and SHA-256 checksum. Never assume a direct package is signed: the current Windows and Linux direct packages are unsigned, and the macOS test DMG is ad-hoc signed but not notarized.

## Why does Windows show a warning?

The current version 1.0.0 direct MSI and Setup EXE are intentionally unsigned, so Microsoft Defender SmartScreen can identify the publisher as unknown. Confirm the file came from the tagged release and verify its SHA-256 checksum before choosing **More info → Run anyway**. Use the Microsoft Store package when you want the Microsoft-signed route. If a release is described as signed but its signature is missing or invalid, do not continue.

## Why does macOS block the test DMG?

The public macOS `0.1.0-alpha.1` DMG is a functional-test build. It is ad-hoc signed rather than Developer ID signed and has not been notarized by Apple, so Gatekeeper is expected to block its first launch. Verify the official release URL and exact SHA-256 checksum before making any exception. Then follow the [macOS installation guide](INSTALL_MACOS.md), which explains **System Settings → Privacy & Security → Open Anyway**. Never override a warning that says the application is damaged or contains malware.

## How do I give NotzUP microphone or screen permission on macOS?

Open **System Settings → Privacy & Security**. Use **Microphone** for audio-input access and **Screen & System Audio Recording** for permitted screen or system-audio capture. Enable OYYO NotzUP only for the features you intend to use, then quit and reopen the application if macOS requests it. The [macOS installation guide](INSTALL_MACOS.md) contains the full first-run flow.

## How do I get help?

Email [support@oyyo.one](mailto:support@oyyo.one). For non-sensitive bugs, use [GitHub Issues](https://github.com/vpicciuolo/oyyo-notzup/issues). Never attach private recordings, access tokens, passwords or personal information to a public issue.

## Where are the legal documents?

- Privacy Policy: https://oyyo.one/privacy
- Terms of Service: https://oyyo.one/terms
- Security reporting: https://github.com/vpicciuolo/oyyo-notzup/blob/main/SECURITY.md


