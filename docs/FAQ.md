<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# OYYO NotzUP FAQ

## What is OYYO NotzUP?

OYYO NotzUP is a local-first capture and knowledge app. It brings audio recording, screen capture, screenshots, scans, file import, text capture, offline transcription, local search, calendar activity and authorized provider connectors into one workspace.

## Is NotzUP only for meetings?

No. It can help with meetings, calls, classes, interviews, voice notes, product walkthroughs, documents, whiteboards, research, saved web references and other material you are allowed to capture.

## Does NotzUP upload my recordings for AI processing?

Supported transcription, extraction, search and generated outputs run on the device. There is no hidden cloud-inference fallback. Optional account sync and storage are separate features that require the user’s choice and remain subject to the plan and privacy policy.

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

Use only the relevant platform store or the official [GitHub Releases page](https://github.com/vpicciuolo/oyyo-notzup/releases). A direct Windows installer is considered official only when it is Authenticode-signed, its signature identifies **Vincenzo Picciuolo**, and its checksum matches the release notes.

## Why does Windows show a warning?

Do not continue if a production installer is unsigned, the signature is invalid, or the publisher does not match the release notes. New certificates can still build SmartScreen reputation over time, but the Authenticode signature must always validate.

## How do I get help?

Email [support@oyyo.one](mailto:support@oyyo.one). For non-sensitive bugs, use [GitHub Issues](https://github.com/vpicciuolo/oyyo-notzup/issues). Never attach private recordings, access tokens, passwords or personal information to a public issue.

## Where are the legal documents?

- Privacy Policy: https://oyyo.one/privacy
- Terms of Service: https://oyyo.one/terms
- Security reporting: https://github.com/vpicciuolo/oyyo-notzup/blob/main/SECURITY.md


