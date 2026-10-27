<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# OYYO NotzUP FAQ

## What is OYYO NotzUP?

OYYO NotzUP is the private capture and knowledge app inside [OYYO ONE AI](https://oyyo.one/). It brings audio recording, permitted screen capture, screenshots, scans, file import, text capture, offline transcription, local search, calendar activity and authorized provider connectors into one workspace.

**Local OYYO AI Core — running privately on your device.**

## Is NotzUP only for meetings?

No. It can help with meetings, calls, classes, interviews, voice notes, product walkthroughs, documents, whiteboards, research, saved web references and other material you are allowed to capture.

## Does NotzUP upload my recordings for AI processing?

Supported transcription, extraction, search and generated outputs run on the device. There is no hidden cloud-inference fallback. Optional account sync and storage are separate features that require the user’s choice and remain subject to the plan and privacy policy.

## Do my files, searches or scans leave my device?

Not by default. Recordings, imported files, scans, local searches and supported local-AI results remain on the device. Data leaves only when the user deliberately chooses an online action such as sharing an export, starting an online search, authorizing a connector or creating an encrypted backup. See [Local-First Privacy and Data Control](LOCAL_FIRST_PRIVACY.md).

## Can NotzUP analyze music or create a lyrics draft?

For audio or music you are permitted to analyze, NotzUP can create a tentative lyrics or spoken-word draft and report grounded sound facts such as duration, sample rate, channels, estimated tempo, tonal estimate and dynamic range. Sung-word recognition can be unreliable over instruments or background audio, so review the draft against the original. NotzUP does not fetch or reproduce third-party lyrics catalogs.

## Can NotzUP describe images?

Yes, when a compatible verified local vision pack is installed. Imported images, screenshots and camera scans can produce a scene description, alt text and approved object labels locally on the device.

## Can NotzUP understand a silent video?

Yes. The mobile app samples video frames for local visual analysis, so visible text, scenes, objects, labels and a non-identifying face count can still be produced when the file has no audio. Speech transcription is separate and requires an audible speech track.

## Does NotzUP identify people or guarantee a brand match?

No. Face analysis reports a count, not an identity. Possible names or brands can be suggested from visible text, but they are unverified hints. A user can explicitly start an online search for detected objects or names and should verify the result against the original source.

## Can NotzUP summarize or translate captured material?

Supported sources can produce reviewable summaries, explanations, action items, clean text, Markdown and structured JSON. Installed local language packs can translate supported outputs offline. Users can choose faithful or paragraph-aware natural context; English and Italian include a light playful style, while Italian also offers beta Napoletano and Barese profiles. Every generated result remains tied to its captured source for review.

## Can NotzUP create a real meeting or call summary?

Yes. When the transcript includes speaker turns, NotzUP preserves labels such as Person 1 and Person 2, lets the user correct participant names, and builds structured meeting notes with an overview, topics, key points, concepts and explanations, problems, decisions, risks, open questions and action items. It never invents a participant identity when the source does not provide one. The transcript and every generated section remain editable, copyable, translatable, readable aloud, exportable and shareable.

## Can NotzUP reverse-engineer an image or video into an AI prompt?

Yes, for a file the user owns or is authorized to analyze. Creative Blueprint separates locally observed ingredients from creative suggestions, then creates an editable recreation plan, master generation prompt, negative prompt, personalization notes and test variants. The user can add a brand, product, audience, tone, platform or requested changes. NotzUP does not download social-media links, copy a creator identity or guarantee that a result will become viral. Without real performance data, explanations about attention or virality are clearly labelled as hypotheses to test.

## Are the playful and dialect translations generated in the cloud?

No. The language pack, paragraph processing, supported style profile and approved correction memory run on the device. Napoletano and Barese are experimental local profiles applied after Italian translation, not a claim of complete regional-language coverage. Review the result with a native speaker when accuracy matters. A correction is reused only after the user edits and explicitly approves that exact source, language and style result.

## Can I use NotzUP without an account?

The desktop app includes a limited guest capture mode for evaluation. Account features such as registered-device entitlements, bookings, notifications, connectors and optional sync require sign-in.

## Does every user have a personal booking page?

Yes. A signed-in user can configure a personal public page and shareable link for meetings or appointments. Guests see available times in their own time zone and can choose a slot without creating a NotzUp account. Availability, duration, buffers and minimum notice are controlled by the page owner.

## Can a guest reschedule or cancel a meeting?

Where enabled, the confirmation includes a private management link for that booking. The guest or account owner can use it to reschedule or cancel. An `.ics` calendar file can also be included. Provider calendar synchronization works only after the user authorizes a supported connector and its configuration succeeds.

## Does booking a meeting give NotzUp permission to record it?

No. A booking and a recording are separate actions. Obtain participant consent and follow applicable law and workplace policy before recording.

## What can the Windows app capture?

The Windows app supports microphone recording, permitted screen/window capture, eligible system audio, screenshots, scans, text/links and supported file imports. Availability depends on Windows permissions, device drivers and whether the source application allows capture.

## Can it record every call or protected stream?

No app can truthfully guarantee that. Windows, Android, iOS and the source application may restrict protected audio, cellular calls, VoIP audio or copyrighted media. NotzUP never bypasses operating-system permissions or source-app protections. Obtain participant consent before recording.

## Does it work with Zoom, Google Meet and Microsoft Teams?

NotzUP can capture eligible device audio/screen sources and can connect to supported provider data through the provider’s official authorization flow. Native capture and provider-history import are different features. What is available depends on the operating system, provider scopes, account plan and administrator policy.

## Which files can I import?

The desktop release supports common PDF, Office, OpenDocument, RTF, HTML, Markdown, CSV/TSV, JSON/XML/YAML, caption, image, audio and video formats. Extraction quality depends on the file, embedded text, installed codecs and verified local models.

## Can I play an imported video inside NotzUP?

Supported videos open in the file workspace with video playback controls. Playback still depends on the device decoder and the codecs inside the file. If sound works but the picture is black, keep the original, update the app, and convert a test copy to a widely supported MP4 file using H.264 video and AAC audio.

## How is a saved file organized?

Each source opens in a separate workspace. Available tabs include Overview, Transcript, Visual analysis, Visible text, and Summary and actions. Users can edit, copy or share a section, export one section as Markdown, Excel, text or PDF, create a branded printable PDF, or download a complete ZIP package.

## Is the barcode scanner available on desktop or web?

No. Barcode and QR Inventory is exclusive to the mobile app and is currently available on Android. The web account can manage plans, storage, devices and encrypted files, but it does not turn a desktop browser into the inventory scanner.

## Which plans include Barcode and QR Inventory?

Only Pro and Organization. Free and Plus do not unlock scanning or inventory sessions.

## How does NotzUP prevent accidental barcode scans?

Single-code and manual inventory modes require the user to tap **Scan code**. Controlled automatic scanning starts only after **Start auto scan** is tapped and ends with **Stop auto scan**. No tap means no scan unless that deliberate automatic session is active.

## Can repeated barcodes be counted as inventory?

Yes. Every accepted scan is kept in chronological history, while identical values are grouped and counted. The inventory shows total scans, unique codes and the quantity for each code.

## Can I import an existing product catalog?

Yes. Import a CSV, XLS or XLSX file with a header row. Useful columns include Description, Article ID, Barcode, Quantity, Warehouse or Location, and Unit. Keep barcode cells formatted as text when leading zeroes matter.

## What does the inventory comparison show?

For each catalog line, NotzUP shows expected quantity, scanned quantity, difference and status. Codes absent from the catalog remain visible as unlisted items. The updated quantity column can be mapped into a reviewed warehouse import; NotzUP does not silently modify an external stock system.

## Which inventory exports are available?

Inventory sessions can be exported as CSV, Excel or a branded printable PDF. CSV is suitable for system import, Excel includes detailed and total views, and PDF is designed for review and sign-off. A single scanned code can also be copied or used for a user-initiated online search.

## How do encrypted backups work?

Supported result and inventory backups are encrypted on the device before upload. The cloud receives encrypted data, while the recovery key stays under the user's control and never reaches NotzUP. Original large media files remain local in the current result-backup workflow.

## Why is two-factor authentication required for encrypted backup?

The recovery key controls access to every compatible encrypted backup, so NotzUP requires account two-factor authentication before key setup. This protects sensitive key-management actions even if an account password is exposed.

## What happens if I lose the recovery key?

If every copy of the matching key is lost, existing encrypted backups cannot be recovered by NotzUP, support or the storage provider. Keep at least two protected copies in separate locations and compare the fingerprint when importing a key on another device.

## Can a new phone restore a backup made by another device?

Yes, when the new installation is authorized for the same personal or Organization space and has the matching recovery key. Choose a dated backup from the cloud file manager and restore it as a local copy. Inventory restoration asks before replacing the current local count.

## Do all my devices share the same storage?

Authorized installations draw from the selected workspace pool. Personal and Organization spaces have separate quotas and permissions. Files stored in an Organization space remain governed by Organization membership even when the same user also has personal storage.

## How do I manage cloud storage?

Open Storage in the web account, or **Encrypted backup and cloud storage** in the mobile settings. Select the correct space to review usage, list files, check dates and sizes, download or restore supported backups, and delete an exact file after confirmation. Devices and active account sessions are managed separately.

## Is settings backup the same as content backup?

No. Settings backup contains a restricted set of compatible preferences. Encrypted content backup contains selected results or an inventory. Settings backup never includes recordings, transcripts, credentials, plan grants or recovery keys.

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

Use only the relevant platform store, including the public [Snap Store listing](https://snapcraft.io/oyyo-notzup) for Linux, or the official [GitHub Releases page](https://github.com/vpicciuolo/oyyo-notzup/releases). Snap Store version 1.0.27.0 revision 3 is currently on `latest/edge` and installs with `sudo snap install oyyo-notzup --edge`. Direct builds are official only when the tagged release explicitly lists the same file name, version, architecture, signature status and SHA-256 checksum. Never assume a direct package is signed: the current Windows and Linux direct packages are unsigned, and the macOS test DMG is ad-hoc signed but not notarized.

## Why does Windows show a warning?

The current version 1.0.0 direct MSI and Setup EXE are intentionally unsigned, so Microsoft Defender SmartScreen can identify the publisher as unknown. Confirm the file came from the tagged release and verify its SHA-256 checksum before choosing **More info → Run anyway**. Use the Microsoft Store package when you want the Microsoft-signed route. If a release is described as signed but its signature is missing or invalid, do not continue.

## Why does macOS block the test DMG?

The public macOS `1.0.27.0` universal offline DMG is a functional-test build. It is ad-hoc signed rather than Developer ID signed and has not been notarized by Apple, so Gatekeeper is expected to block its first launch. Verify the official release URL and exact SHA-256 checksum before making any exception. Then follow the [macOS installation guide](INSTALL_MACOS.md), which explains **System Settings → Privacy & Security → Open Anyway**. Never override a warning that says the application is damaged or contains malware.

## How do I give NotzUP microphone or screen permission on macOS?

Open **System Settings → Privacy & Security**. Use **Microphone** for audio-input access and **Screen & System Audio Recording** for permitted screen or system-audio capture. Enable OYYO NotzUP only for the features you intend to use, then quit and reopen the application if macOS requests it. The [macOS installation guide](INSTALL_MACOS.md) contains the full first-run flow.

## How do I get help?

Email [support@oyyo.one](mailto:support@oyyo.one). For non-sensitive bugs, use [GitHub Issues](https://github.com/vpicciuolo/oyyo-notzup/issues). Never attach private recordings, access tokens, passwords or personal information to a public issue.

## Where are the legal documents?

- Privacy Policy: https://oyyo.one/privacy
- Terms of Service: https://oyyo.one/terms
- Security reporting: https://github.com/vpicciuolo/oyyo-notzup/blob/main/SECURITY.md


