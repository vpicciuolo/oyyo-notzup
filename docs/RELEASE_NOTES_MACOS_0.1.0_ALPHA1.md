<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# OYYO NotzUP macOS 0.1.0-alpha.1 test release

This pre-release makes the first public macOS DMG available for functional
testing. It uses the same shared Tauri, React and Rust desktop application built
alongside the Windows artifact from the same source revision; it does not add a
separate macOS product experience.

## Download

- [Universal macOS test DMG](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v0.1.0-alpha.1-macos/OYYO-NotzUP-0.1.0-alpha.1-macOS-universal-test.dmg)
- [SHA-256 manifest](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v0.1.0-alpha.1-macos/SHA256SUMS-macos.txt)
- [Installation and first-run instructions](INSTALL_MACOS.md)

## Verification completed

The GitHub-hosted macOS build completed:

- the shared desktop frontend build;
- Rust formatting, linting and tests;
- universal `x86_64` + `arm64` application compilation;
- application bundle creation;
- ad-hoc code signing and strict signature verification;
- DMG creation, verification and read-only mounting;
- mounted application signature and executable checks;
- a launch smoke test;
- immutable artifact publication with SHA-256 verification.

## Important test-build limitations

- The DMG is ad-hoc signed, not signed with an Apple Developer ID.
- Apple notarization has not been performed.
- Gatekeeper can require a deliberate **Open Anyway** override.
- The build is not a Mac App Store package and has not passed App Review.
- Physical Intel and Apple silicon capture/permission testing is still needed.
- Protected or application-restricted audio and video sources may be
  unavailable.
- Back up important work and do not use this alpha as the only copy of a
  recording.

## Checksum

```text
1cfb137867c6c452df3f8461e3c6d5ce90c1dc6bd4d852095021d564b905d8eb  OYYO-NotzUP-0.1.0-alpha.1-macOS-universal-test.dmg
```

Report non-sensitive defects through the
[public issue tracker](https://github.com/vpicciuolo/oyyo-notzup/issues). Never
attach recordings, transcripts, account credentials or personal data to a
public issue.
