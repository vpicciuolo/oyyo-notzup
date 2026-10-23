<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Encrypted Backup and Cloud Storage

OYYO NotzUP keeps capture and analysis local by default. Cloud storage is optional and selected by the user. Supported result and inventory backups are encrypted on the device before upload, using a recovery key that NotzUP does not receive.

## Three things that are separate

1. **Local originals and results** live on the device unless the user selects an online action.
2. **Encrypted content backups** contain selected transcript, visual notes, visible text, summary, edits or inventory data. The original large media file stays local unless a future workflow explicitly says otherwise.
3. **Settings backup** stores a restricted set of compatible preferences. It does not contain recordings, transcripts, credentials, plan grants or recovery keys.

## Security model

- Encryption and decryption occur on the authorized device.
- Encryption setup requires two-factor authentication on the account.
- The recovery key is 256-bit key material stored locally through protected device facilities where supported.
- The cloud receives encrypted backup data, not the recovery key.
- A key fingerprint helps the user confirm that two devices use the same key without revealing the key.
- Losing every exported or installed copy of the matching key makes existing encrypted backups permanently unreadable.

This design gives the user control, but it also gives the user responsibility for key custody.

## Set up encrypted backup

1. Sign in to the web account.
2. Open **Security** and enable two-factor authentication.
3. Open the encrypted-backup or recovery-key controls.
4. Generate the recovery key.
5. Download the `.notzup-key` file to a secure location that is separate from the backed-up device.
6. Keep at least one additional protected copy under the account owner's control.
7. On the mobile app, open **Settings**, then **Encrypted backup and cloud storage**.
8. Choose **Import recovery key** and select the downloaded key file.
9. Compare the displayed fingerprint with the web account fingerprint.

Do not email an unprotected recovery key to yourself or store the only copy on the same phone.

## Back up a result

1. Open a file workspace in **Library**.
2. Review the transcript, visual analysis, visible text, summary and edits.
3. Choose **Save results to cloud**.
4. Select the personal or Organization storage space.
5. Wait for confirmation that the encrypted backup was stored.

The app encrypts the backup before upload. The original media remains on the phone for the current result-backup workflow.

## Back up an inventory

1. Open the mobile barcode inventory.
2. Review the session name, catalog and counts.
3. Choose **Back up to cloud**.
4. Select the correct personal or Organization space.
5. Wait for the encrypted upload confirmation.

## Restore on a new installation

1. Install NotzUP and sign in to the account that has access to the storage space.
2. Enroll the new installation if the plan's device limit allows it.
3. Import the same `.notzup-key` file.
4. Open **Manage cloud files and restore** or the Restore action in a file workspace.
5. Choose the personal or Organization space.
6. Select a dated backup created by any authorized device in that space.
7. Review its name, size, date and type.
8. Restore a result as a new local copy. For inventory, confirm before replacing the current local count.

Cloud authorization and the correct recovery key are both required. Having only one of them is not enough.

## Personal and Organization storage

- Personal storage belongs to the user's personal workspace.
- Organization storage is a pooled workspace allowance governed by Organization membership and role permissions.
- Every authorized installation using the same selected space draws from the same quota.
- Removing one device does not automatically delete the shared cloud files.
- Leaving or losing access to an Organization removes access to that Organization's storage even if the device still has a local copy.

## Manage stored files

From the app or web account storage manager, users with permission can:

- View the selected space and total usage.
- List stored NotzUP backup files.
- Check file name, type, date and size.
- Restore or download a supported backup.
- Delete an unwanted cloud file after confirming the exact target.
- Review devices and active account sessions separately.

Deleting a cloud backup does not delete the original local file. Deleting a local file does not automatically delete its cloud backup.

## Key changes and loss

### Download another protected copy

Use the authenticated web security controls. Keep copies in protected locations and identify them by fingerprint and creation date.

### Import a key on another device

Use **Import recovery key** and verify the fingerprint. Never import a key supplied by an untrusted person or website.

### Regenerate or rotate the key

Read the warning carefully. Existing backups encrypted with an older key may still require that older key unless the product explicitly re-encrypts them. Do not destroy the old key until every required backup has been restored or migrated.

### Remove the key from one phone

Removing the local key prevents that phone from decrypting existing backups until the matching key is imported again. It does not erase the encrypted cloud files.

### Every key copy is lost

NotzUP cannot decrypt, reset or bypass the backup encryption. The encrypted cloud files may be deleted by an authorized account user, but their contents cannot be recovered.

## Troubleshooting

### Recovery key required

Import the `.notzup-key` file whose fingerprint matches the backup. A newly generated key cannot decrypt backups created with another key.

### Backup belongs to another space

Switch to the correct personal or Organization workspace and confirm current membership.

### Storage is full

Review usage, remove unneeded cloud files, or change storage capacity through the web account when billing is available for the workspace. A full cloud quota does not remove local access to the source.

### A backup cannot be restored

Check account authorization, workspace selection, key fingerprint, network connectivity and app version. Keep the encrypted file until support confirms that it is corrupt or incompatible.

## Safety checklist

- Enable two-factor authentication.
- Keep at least two protected recovery-key copies.
- Verify fingerprints when adding a device.
- Use the correct workspace before uploading.
- Test one restore before relying on the backup process.
- Never publish a recovery key or attach it to a public support issue.
