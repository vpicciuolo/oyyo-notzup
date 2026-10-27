<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Getting Started with NotzUp

OYYO NotzUP is available from the Microsoft Store, with additional Windows,
macOS test, Android pre-release and Linux preview packages on the official
[GitHub Releases page](https://github.com/vpicciuolo/oyyo-notzup/releases).
Every direct package has a disclosed signature status and checksum. This public
repository contains user guides and approved release downloads, not the full
proprietary source.

## Install

- **Windows:** use the signed
  [Microsoft Store package](https://apps.microsoft.com/detail/9NX0604FJ0XN), or
  follow the [Windows desktop installation guide](INSTALL_DESKTOP.md) for the
  disclosed unsigned direct installers.
- **macOS:** follow the
  [macOS installation and first-run guide](INSTALL_MACOS.md). The current
  `1.0.27.0` universal offline DMG is an ad-hoc-signed, non-notarized test
  build and requires checksum verification plus an informed Gatekeeper
  override. The app installs offline; speech and AI model weights are separate.
- **Android:** follow the [mobile installation guide](INSTALL_MOBILE.md) and
  verify the APK checksum and signing-certificate digest.
- **Linux:** follow the [Linux installation guide](INSTALL_LINUX.md) and verify
  the selected package against its SHA-256 manifest.

The canonical list of current packages and their release status is
[Download OYYO NotzUP](DOWNLOADS.md).

## First run

1. Open NotzUP from the operating system's Applications or app menu.
2. Sign in for account, entitlement, connector, booking and optional sync
   features, or use limited guest capture where offered.
3. Choose whether to allow privacy-safe analytics. Captured content is excluded
   from analytics.
4. Approve only the microphone, screen, camera or notification permissions
   required for the feature you select.
5. Keep the app open while the local core engine downloads automatically and
   passes integrity verification. If Android pauses the download, reconnect to
   the internet, disable battery restrictions for NotzUP temporarily, and use
   **Settings → Local intelligence → Download / verify model** to resume it.
6. Select **Capture anything**, choose a source, name the session and start.
7. Keep the visible recording indicator available, then stop and save.
8. Open **Library** to review the original, transcript and supported local
   outputs.

Capture audio, screen, video and typed notes only when authorized, import
documents or saved provider content you are permitted to use, and organize the
results in a private local library. Supported transcription, analysis, search
and generated outputs run on the user's device without a hidden cloud-model
fallback. Optional account services and sync are separate choices.

## Account, plans and the local engine

Account registration is required for licensed runtimes. Plan limits and prices
are enforced by the current account service and displayed on
[notzup.com/pricing](https://notzup.com/pricing) and the signed-in Billing page.
Transcription, summarization and supported AI processing run on the device,
with no hidden cloud-model fallback. Optional cloud storage never means
automatic upload.

The mobile Barcode and QR Inventory workspace is available only on **Pro and
Organization**, and is currently an Android-only capability. Free and Plus can
review its plan information but cannot start an inventory scan. Read the
[barcode inventory guide](MOBILE_BARCODE_INVENTORY.md) before the first count.

Encrypted result and inventory backup requires account two-factor
authentication plus a user-controlled recovery key. NotzUP cannot replace a
lost key. Complete the [encrypted backup setup](ENCRYPTED_BACKUP_AND_STORAGE.md)
and test one restore before relying on it.

## Learn every workflow

The [Complete User Guide](USER_GUIDE.md) contains numbered instructions for
audio, screen and meeting capture; photos, scans and screenshots; file import;
playback; transcription; image and silent-video understanding; editable file
tabs; summaries; translation; export and sharing; notifications; cloud storage;
devices; sessions; calendar; bookings; connectors and problem reports.

The [Complete Feature Guide](FEATURES.md) is a concise capability and privacy
reference.

## Need help?

Read the [FAQ](FAQ.md), report non-sensitive defects through
[GitHub Issues](https://github.com/vpicciuolo/oyyo-notzup/issues), or email
[support@oyyo.one](mailto:support@oyyo.one). Never place recordings,
transcripts, credentials or personal data in a public issue.
