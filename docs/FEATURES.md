<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# OYYO NotzUP features

OYYO NotzUP is a private capture and knowledge workspace for audio, video, images, documents, screens, conversations and everyday ideas. Supported transcription, OCR, visual understanding, summarization, translation and search run on the authorized device. Online account, storage, sharing, notification and booking features are separate and user controlled.

## Capture and import

- Record microphone audio with a visible capture state.
- Record an eligible screen or app window where the operating system permits it.
- Take a photo, scan a page or save a screenshot.
- Import supported audio, video, image, document, text and Markdown files.
- Keep the original local source associated with its extracted results.
- Use Android widgets, Quick Settings tiles and floating controls for faster access.

File support depends on the operating system and the codecs or document readers available on that device. Protected streams, cellular calls and another app's private audio may be unavailable even on a paid plan.

## One workspace for each file

Each saved source opens in its own organized workspace. Available tabs depend on the source:

- **Overview:** source information, available results and recommended next action.
- **Transcript:** editable speech-to-text output.
- **Visual analysis:** scene, object, label and non-identifying face-count observations.
- **Visible text:** OCR output from images, pages and sampled video frames.
- **Summary and actions:** a reviewable local summary and extracted follow-up items.
- **Meeting notes:** speaker-labelled turns, overview, topics, concepts, problems, decisions, risks, questions and action items for calls and meetings.
- **Creative Blueprint:** an editable recreation plan and grounded generation prompt for user-owned images and videos.

The user can select and copy part of a section, edit the whole section, share one result, or export it as Markdown, Excel, text or PDF. A complete ZIP keeps the original and generated results together. The branded printable PDF combines the useful sections into one document.

## On-device speech and media understanding

- Download and verify the local core engine automatically after first launch.
- Transcribe supported audio and video containing speech.
- Analyze images and sampled video frames even when the video is silent.
- Read visible text with local OCR.
- Describe scenes, objects and general visual labels.
- Report face counts without identifying people.
- Surface possible names or brands from visible text as unverified hints.
- Start a user-requested online search using detected objects or names.
- Choose a destination language and translate supported extracted text with an installed on-device language pack.
- Select faithful or paragraph-aware natural-context output while keeping the captured source on the device.
- Use a light playful style for supported English and Italian output, or clearly labelled beta Napoletano and Barese profiles for Italian.
- Edit and approve an exact translation correction for private reuse on that device.

The beta dialect profiles apply conservative local wording changes after the Italian translation and must be reviewed. They do not claim the broader intent, cultural adaptation or full dialect coverage described by [OYYO Language](https://oyyo.one/language). Read the [offline translation and accessibility guide](OFFLINE_TRANSLATION_AND_ACCESSIBILITY.md).

## Meeting and call intelligence

- Preserve speaker labels found in a transcript and display turns as **Person 1**, **Person 2** or reviewed names.
- Edit one speaker label or apply a corrected name to matching turns without changing timestamps.
- Generate structured, reviewable meeting notes with an overview, topics, key points, concepts and explanations, problems, decisions, risks, open questions and action items.
- Keep every conclusion tied to the local transcript so the user can verify, edit, copy, translate, listen to, export or share it.
- Never invent a participant identity when the source does not provide one.

## Creative Blueprint for images and videos

- Analyze a user-selected image or sampled video locally; social-link downloading is not supported.
- Separate observed evidence from creative suggestions and unsupported claims.
- Produce an editable recreation plan, master generation prompt, negative prompt, personalization notes and format or hook variants.
- Let the user add brand, product, audience, tone, platform and requested changes before regenerating the blueprint.
- Treat explanations of attention or virality as hypotheses unless the user supplies real reach, retention, watch-time, save or share metrics.
- Keep rights, consent, likeness, watermark, privacy and claim-review checks visible in the result.

## Accessibility and Android device support

- Read a populated result section aloud with an installed offline Android voice.
- Stop speech immediately from the same file workspace.
- Use screen readers with spoken labels on primary controls and capture states.
- Keep Android display and font-size preferences throughout the interface.
- Use responsive touch layouts on phones, tablets and foldables.

Google TV is not supported. NotzUP requests touch capability so the mobile interface is not offered as a TV app.

Visual labels and possible brand hints are observations, not proof. The user should verify them against the original image or video.

## Mobile Barcode and QR Inventory

This is a **mobile-exclusive** feature, currently available on Android for **Pro and Organization** plans.

- Single-code mode with an explicit **Scan code** button on the camera.
- Inventory mode with manual scanning or a deliberate Start/Stop automatic scan session.
- Camera controls that remain visible above the result panel on phones.
- A two-column camera-and-results layout on tablets and foldables.
- Torch control and profiles for retail, QR, warehouse or all supported codes.
- Duplicate counting and a chronological scan history.
- Online lookup for one scanned code.
- CSV, XLS and XLSX catalog import.
- Comparison of expected, scanned and difference quantities.
- Clear handling of matched, short, over and unlisted items.
- CSV, Excel and branded PDF exports.
- Encrypted cloud backup and restore of inventory sessions.

Read the [complete barcode inventory guide](MOBILE_BARCODE_INVENTORY.md).

## Encrypted backup and shared storage pools

- Encrypt supported backups on the device before upload.
- Require account two-factor authentication before recovery-key setup.
- Download, import, rotate or remove recovery-key access on an authorized device.
- Restore a dated backup made by another authorized phone or computer.
- Keep personal and Organization storage quotas separate.
- Share the selected workspace's storage pool across its authorized devices.
- View usage, manage stored files and delete files from mobile or web account controls.

NotzUP never receives the content-encryption recovery key. If every key copy is lost, existing encrypted backups cannot be recovered. Read [Encrypted Backup and Cloud Storage](ENCRYPTED_BACKUP_AND_STORAGE.md).

## Search, edit, export and share

- Search local titles, transcript passages and supported extracted text.
- Edit transcripts, visual notes, visible text, summaries and action items.
- Copy a selected passage or a complete section.
- Share only the chosen result rather than the complete source.
- Export individual sections as Markdown, Excel, TXT or PDF.
- Export a full branded printable PDF or a complete ZIP package.
- Keep shared access scoped, reviewable and revocable where account sharing is used.

## Account, devices and security

- External-browser sign-in for native apps.
- Server-authoritative plan and device enrollment.
- Device list and session management.
- Two-factor authentication for sensitive security and encryption operations.
- Personal and Organization workspaces with separate permissions and quotas.
- In-app notifications with read-all and delete-all controls where supported.
- Native notifications for configured delivery channels.

## Calendar, bookings and connectors

- Give every user a personal public booking page and shareable meeting link.
- Let guests choose an available time in their own time zone without creating an account.
- Configure availability, duration, buffers and minimum notice.
- Prevent a confirmed time from being booked twice and manage confirmation, rescheduling or cancellation.
- Include an `.ics` file and a private booking-management link where supported.
- Connect supported providers only through their consent screen.
- Review provider scopes and disconnect an account when no longer needed.
- Treat exported AI output as a draft until the user approves it.

Read [Personal Booking Pages and Meeting Links](PUBLIC_BOOKING_PAGES.md).

## What stays local

Recordings, imported media and local analysis remain on the device unless the user explicitly selects an online action. NotzUP does not use a hidden cloud AI fallback for customer-content inference. Optional cloud storage, account sync, sharing, notifications and provider connectors are separate operations with their own permission and quota checks.

## Continue

- [Complete User Guide](USER_GUIDE.md)
- [Offline Translation, Read-Aloud and Accessibility](OFFLINE_TRANSLATION_AND_ACCESSIBILITY.md)
- [Mobile Barcode and QR Inventory](MOBILE_BARCODE_INVENTORY.md)
- [Encrypted Backup and Cloud Storage](ENCRYPTED_BACKUP_AND_STORAGE.md)
- [Personal Booking Pages and Meeting Links](PUBLIC_BOOKING_PAGES.md)
- [Local-First Privacy and Data Control](LOCAL_FIRST_PRIVACY.md)
- [FAQ](FAQ.md)
- [Downloads](DOWNLOADS.md)
