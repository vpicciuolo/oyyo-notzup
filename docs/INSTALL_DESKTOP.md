<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Install OYYO NotzUP on Windows

For a Mac, use the separate [macOS installation and first-run guide](INSTALL_MACOS.md).

OYYO NotzUP is the private capture and knowledge app inside [OYYO ONE AI](https://oyyo.one/). Its **Local OYYO AI Core runs privately on your device** for supported transcription, music and audio analysis, visual descriptions, translation, search, summaries and grounded outputs.

## Requirements

- Windows 10 or Windows 11, x64
- Microsoft Edge WebView2 Runtime (included with supported Windows installations or installed by the NotzUP bootstrapper when required)
- Sufficient local storage for the app, recordings, imported media and optional local models
- Internet access for first sign-in, verified model download, connectors and optional account services
- Microphone, screen, camera and notification permission only for the features you choose

## Official downloads

Download NotzUP only from:

1. The [Microsoft Store listing](https://apps.microsoft.com/detail/9NX0604FJ0XN), or
2. The official, versioned [OYYO NotzUP GitHub Releases page](https://github.com/vpicciuolo/oyyo-notzup/releases).

The GitHub installer URL is immutable for each release tag. The version 1.0.0 direct Setup EXE and MSI are intentionally unsigned and can trigger SmartScreen; the Microsoft Store package is the signed recommended route. Direct releases include SHA-256 checksums, release notes and an explicit signature-status disclosure. Do not install a file copied to another host or whose checksum does not match.

## Verify the Windows download

1. Confirm that the address is `github.com/vpicciuolo/oyyo-notzup` and that the file name exactly matches the tagged release.
2. Compare its SHA-256 value with `SHA256SUMS-windows.txt` in that release.
3. Right-click the MSI or EXE, choose **Properties**, and inspect **Digital Signatures** if present.
4. For version 1.0.0, a missing Digital Signatures tab is expected because the direct files are disclosed as unsigned. If a later release is described as signed, require a valid matching signature.

Advanced PowerShell verification:

```powershell
Get-AuthenticodeSignature -FilePath '.\OYYO-NotzUP-Windows-x64.msi' | Format-List Status,StatusMessage,SignerCertificate,TimeStamperCertificate
Get-FileHash -Algorithm SHA256 -Path '.\OYYO-NotzUP-Windows-x64.msi'
```

Compare the SHA-256 result with the checksum published in the matching GitHub Release.

## Install

1. Open the verified MSI or EXE.
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


