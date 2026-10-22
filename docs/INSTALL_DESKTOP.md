<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Install OYYO NotzUP on Windows

## Requirements

- Windows 10 or Windows 11, x64
- Microsoft Edge WebView2 Runtime (included with supported Windows installations or installed by the NotzUP bootstrapper when required)
- Sufficient local storage for the app, recordings, imported media and optional local models
- Internet access for first sign-in, verified model download, connectors and optional account services
- Microphone, screen, camera and notification permission only for the features you choose

## Official downloads

Download NotzUP only from:

1. The Microsoft Store listing published by **Vincenzo Picciuolo**, or
2. The official, versioned [OYYO NotzUP GitHub Releases page](https://github.com/vpicciuolo/oyyo-notzup/releases).

The GitHub installer URL is immutable for each release tag. A production release includes an Authenticode signature, SHA-256 checksums and release notes. Do not install a file that was copied to another host or whose signature/checksum does not match.

## Verify the Windows signature

1. Right-click the downloaded MSI or EXE and select **Properties**.
2. Open **Digital Signatures**.
3. Confirm the signature is valid and the signer/publisher matches **Vincenzo Picciuolo**.
4. If the tab is missing or Windows reports an invalid signature, delete the file and contact support.

Advanced PowerShell verification:

```powershell
Get-AuthenticodeSignature -FilePath '.\OYYO-NotzUP-Windows-x64.msi' | Format-List Status,StatusMessage,SignerCertificate,TimeStamperCertificate
Get-FileHash -Algorithm SHA256 -Path '.\OYYO-NotzUP-Windows-x64.msi'
```

Compare the SHA-256 result with the checksum published in the matching GitHub Release.

## Install

1. Open the signed MSI or EXE.
2. Review the publisher and destination.
3. Complete the installation and launch **OYYO NotzUP**.
4. Choose whether to allow privacy-safe analytics. You can change this later in Settings.
5. Approve only the device permissions needed for the source you select.
6. Let the local speech model download and pass integrity verification on first use.

## First capture

1. Select **Capture anything**.
2. Choose Audio, Screen recording, Screenshot, Scan, Import a file, or Text or link.
3. Review the source and output settings.
4. Start the capture and keep the visible recording indicator available.
5. Stop and save, then open **Library** to review the original and run supported local processing.

## Uninstall

Open **Settings → Apps → Installed apps → OYYO NotzUP → Uninstall**. Uninstalling the application and deleting local content are separate actions. Export anything you need and use the in-app deletion controls before uninstalling if you want local captures removed.

## Help

See the [FAQ](FAQ.md) or email [support@oyyo.one](mailto:support@oyyo.one).


