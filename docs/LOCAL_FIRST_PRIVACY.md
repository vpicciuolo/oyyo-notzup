<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Local-First Privacy and Data Control

NotzUp is local by default. Your recordings, imported files, photos, scans, local searches and supported AI results remain on the device where you created them unless you deliberately choose an online action.

Supported transcription, OCR, visual analysis, summarization, translation and search run on an authorized device. NotzUp does not send customer content to a cloud AI model and does not use a hidden remote-inference fallback.

## You decide what leaves the device

Data can leave a device only through an action you choose, such as:

- sharing an approved section or exported file;
- starting an online product or visual-result search;
- connecting an external calendar or content provider;
- saving a selected supported backup to online storage;
- submitting a problem report after reviewing its diagnostic contents.

The selected destination receives the data required for that action and then applies its own privacy terms. For example, an online product search sends the search terms you approve, while sharing a PDF sends the PDF to the app or person you select.

## Local processing and downloaded engines

Some local features require a verified engine or language pack to be downloaded first. The download obtains software or model assets; it does not upload your recording for processing. NotzUp verifies trusted assets before use where the release supports verification.

## Optional encrypted backup

Supported result and inventory backups are encrypted on the device before upload. Backup setup requires two-factor authentication and a user-controlled recovery key. The recovery key is not sent to NotzUp. If every copy of the matching key is lost, NotzUp, support and the storage provider cannot recover the encrypted backup.

Read [Encrypted Backup and Cloud Storage](ENCRYPTED_BACKUP_AND_STORAGE.md) before relying on backup recovery.

## Authorized devices and storage pools

Authorized devices can use the selected personal or Organization storage pool, subject to plan limits and workspace permissions. A newly installed device must be authorized, have access to the same storage space and import the matching recovery key before it can restore a compatible encrypted backup.

The app and web account can expose separate controls for stored files, enrolled devices and active sign-in sessions. Removing one does not automatically remove the others.

## Calendar, booking and connector data

Public booking pages use the scheduling information intentionally shown to guests. They do not expose local media, transcripts, scans or searches. External connectors work only after authorization through the provider's own consent flow and only when the integration is configured.

## Permissions and protected sources

NotzUp follows Android, iOS, Windows, macOS and Linux permission controls. It does not bypass protected audio, cellular-call restrictions, private audio from another app or digital-rights controls. Grant only the microphone, camera, screen, notification or file permissions needed for the feature you intend to use.

## Share the minimum necessary

Before sharing or exporting:

1. Open the exact file workspace.
2. Review and edit the result.
3. Choose one section when the recipient does not need the complete package.
4. Check the destination app and recipient.
5. Remove sensitive names, account details or recovery information.

Never send a recovery key, password, access token or private recording through a public GitHub issue.

## Related guides

- [Encrypted Backup and Cloud Storage](ENCRYPTED_BACKUP_AND_STORAGE.md)
- [Personal Booking Pages and Meeting Links](PUBLIC_BOOKING_PAGES.md)
- [Complete User Guide](USER_GUIDE.md)
- [FAQ](FAQ.md)

