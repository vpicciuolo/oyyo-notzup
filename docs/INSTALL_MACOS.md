<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Install and run OYYO NotzUP on macOS

This guide covers the public `1.0.27.0` offline test DMG. It contains
one universal application for Intel and Apple silicon Macs. It is ad-hoc
signed and **not notarized by Apple**, so it is not the production direct-
download release and macOS can block its first launch.

## Requirements

- macOS 11 or later;
- an Intel or Apple silicon Mac;
- about 50 MB for the downloaded DMG and installed application, plus storage
  for captures, imports and optional local models;
- internet access for GitHub download, first sign-in, verified model download,
  connectors and optional online account features;
- microphone and screen/system-audio permissions only for capture modes you
  choose.

This is a test release. Back up important work and do not use it as the only
copy of a recording.

## 1. Download only from the official release

Open the official
[macOS `1.0.27.0` offline test prerelease](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.27.0-macos-offline-test)
and download:

- `OYYO-NotzUP-1.0.27.0-macOS-universal-offline.dmg`;
- `SHA256SUMS`;
- `README.txt`.

Do not install a copy received through email, chat, a mirror or another host.

## 2. Verify the download

Open **Terminal**, change to the download directory, and run:

```bash
cd ~/Downloads
shasum -a 256 OYYO-NotzUP-1.0.27.0-macOS-universal-offline.dmg
```

The exact expected SHA-256 value is:

```text
eff66f53e3aead572ef1ce31900425ce79536330514543050dec9d2b36162117
```

You can also verify it against the downloaded manifest:

```bash
shasum -a 256 -c SHA256SUMS
```

Continue only if the command reports `OK`. If verification fails, delete the
downloads and contact [support@oyyo.one](mailto:support@oyyo.one).

## 3. Install the application

1. Double-click the verified DMG in Downloads.
2. In the mounted window, drag **OYYO NotzUP** onto the **Applications**
   shortcut.
3. Wait for the copy to finish.
4. Eject **OYYO NotzUP** from the Finder sidebar.
5. Open **Applications** in Finder and locate **OYYO NotzUP**.

Apple documents the same disk-image installation flow in
[Install and uninstall apps from the internet or a disc on Mac](https://support.apple.com/guide/mac-help/mh35835/mac).

## 4. Approve this non-notarized test build

The build is not signed with an Apple Developer ID and has not passed Apple
notarization. Gatekeeper is therefore expected to block the first launch.
Apple warns that overriding this protection carries risk. Proceed only after
you have verified the official GitHub URL and exact SHA-256 value above.

1. Double-click **OYYO NotzUP** in Applications once.
2. If macOS blocks it, dismiss the alert without moving the application to
   Trash.
3. Open **Apple menu → System Settings → Privacy & Security**.
4. Scroll to **Security** and choose **Open Anyway** for OYYO NotzUP.
5. Authenticate if macOS asks, review the warning again, and choose **Open**.

Apple says the **Open Anyway** control is available for about one hour after
the blocked launch attempt. See
[Open an app by overriding security settings](https://support.apple.com/guide/mac-help/mh40617/mac).

Do **not** override an alert saying the application is damaged or contains
malware. Delete the download and report it instead.

## 5. First run

1. Open **OYYO NotzUP** from Applications.
2. Sign in when you need account, entitlement, connector, booking or optional
   sync features. Limited guest capture can be used for evaluation where
   offered.
3. Choose whether to allow privacy-safe analytics. Captured content is excluded
   from analytics.
4. Install the verified local speech or AI model pack while online and let its
   integrity verification finish before expecting that capability to work
   offline. The DMG installs the native application offline; model weights are
   intentionally separate.
5. Select **Capture anything**, choose an available source, name the session,
   and start.
6. Keep the visible capture indicator available, then stop and save.
7. Open **Library** to review the original and supported local outputs.

Only capture material you are permitted to record. Obtain participant consent
and follow applicable law, workplace policy and source-service rules.

## 6. Grant capture permissions

NotzUP requests a permission when the related feature first needs it. Grant
only the permissions required for the capture you chose.

### Microphone

Choose **Allow** when macOS asks. To review the setting later:

1. Quit OYYO NotzUP.
2. Open **System Settings → Privacy & Security → Microphone**.
3. Enable OYYO NotzUP.
4. Reopen the application and try the recording again.

Apple's current instructions are available in
[If you can’t record audio from an external source on Mac](https://support.apple.com/102071).

### Screen and system audio

Choose **Allow** or **Allow While Using the App** when macOS asks. To change the
setting later, open **System Settings → Privacy & Security → Screen & System
Audio Recording** and enable OYYO NotzUP. Quit and reopen the application if
macOS requests it.

See Apple's
[Control access to screen and system audio recording](https://support.apple.com/guide/mac-help/mchld6aa7d23/mac).

macOS and the source application can restrict protected video, system audio,
cellular calls, VoIP audio or copyrighted media. NotzUP does not bypass those
restrictions.

## 7. Run NotzUP after installation

For later sessions, open Finder, choose **Applications**, and double-click
**OYYO NotzUP**. You can also launch it from Spotlight by searching for
`OYYO NotzUP`.

If the app opens but a capture source is unavailable:

1. confirm the relevant permission in Privacy & Security;
2. quit and reopen NotzUP;
3. confirm that the microphone or display is available to other apps;
4. retry with an unprotected source;
5. include the macOS version and Mac architecture when reporting the issue,
   but never attach private recordings or credentials to a public issue.

## 8. Update to a later build

1. Export or back up anything you need.
2. Download the newer DMG from the official Releases page.
3. Verify its own checksum; do not reuse the checksum from this release.
4. Quit OYYO NotzUP.
5. Mount the new DMG and drag the new application to Applications.
6. Approve **Replace** when Finder asks.
7. Launch and complete a short test capture before deleting the older DMG.

## 9. Uninstall

1. Export anything you need and use the in-app deletion controls for captures
   you want removed.
2. Quit OYYO NotzUP.
3. Open Applications in Finder.
4. Drag **OYYO NotzUP** to Trash, then empty Trash when ready.

Removing the application and deleting its local library are separate actions.
Do not manually delete application-data folders unless support gives you a
version-specific path and you have backed up required work.

## Release status

- Version: `1.0.27` (DMG package revision `1.0.27.0`)
- Architecture: universal Intel `x86_64` + Apple silicon `arm64`
- Minimum configured macOS version: `11.0`
- Signature: ad-hoc test signature
- Apple notarization: not performed
- Mac App Store: separate `1.0.27` build `7` is in TestFlight Beta App Review
- Runtime checks: cold launch, local-library loading and microphone-device
  discovery passed on Apple silicon; physical recording, Intel execution and
  minimum-OS execution were not completed
- SHA-256: `eff66f53e3aead572ef1ce31900425ce79536330514543050dec9d2b36162117`

The production DMG will be published separately after Developer ID signing,
Apple notarization and supported-device QA. The Mac App Store build follows a
separate Apple review route.

## Help

- [Download options](DOWNLOADS.md)
- [Getting Started](GETTING_STARTED.md)
- [FAQ](FAQ.md)
- [Public issue tracker](https://github.com/vpicciuolo/oyyo-notzup/issues)
- [support@oyyo.one](mailto:support@oyyo.one)
