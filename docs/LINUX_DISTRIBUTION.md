<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Linux distribution channels

OYYO NotzUP uses different package formats for different Linux installation
experiences. A build artifact is not a store listing; each channel is announced
only after its own review and clean-machine installation checks pass.

| Channel | User experience | Current status |
| --- | --- | --- |
| [Snap Store](https://snapcraft.io/oyyo-notzup) | Search/install through Ubuntu App Center; automatic updates | Version 1.0.0 is public on `latest/edge`; strict Snap CLI and GUI validation passed; physical QA remains before stable promotion |
| GitHub Releases | AppImage, DEB, RPM, Snap and CLI direct downloads | [Unsigned 1.0.27.0 x86-64 release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.27.0-linux); build, tests, checksum, package metadata, CLI and virtual-display GUI smoke checks passed; physical permission QA remains |
| Ubuntu/Debian archive | Native package search through official repositories | Separate distribution-maintainer review required; not submitted |
| Fedora COPR / openSUSE OBS | Repository-managed RPM updates | Possible later channel; account, source-package and distro review required |
| Arch User Repository | Maintainer-owned `PKGBUILD` | Possible after an immutable public release exists |
| Flathub | Flatpak listing across many desktop software centers | Separate human packaging/review assessment required; not submitted |

The first release targets x86-64. ARM64 remains unavailable until native ARM64
build and physical-device tests pass.

The direct package candidate has passed clean virtual-machine installation and
runtime tests: the DEB on Ubuntu 22.04 and Debian 12, the RPM on Fedora 44, and
the AppImage GUI on Ubuntu 22.04. The strict Snap also passed local installation,
confined CLI execution and rendered-GUI validation in the Ubuntu VM. The
direct packages are now available as an unsigned GitHub preview. The Snap Store
listing is public on `latest/edge`, but that does not replace physical Linux
checks for audio, camera, screen capture, Wayland/X11 or desktop portals and
does not represent a stable-channel release.

## Why Snap is first for Ubuntu

Ubuntu's App Center shows snaps from the Snap Store by default. Publishing a
DEB on GitHub does not add it to Ubuntu's official repositories; it remains a
manual third-party installation. The Snap therefore provides the shortest
reviewed path to a searchable Ubuntu catalog listing while the DEB remains
available for users who prefer a direct system package.

## Other distributions

The AppImage is the broad portable option. RPM serves Fedora-family direct
installs, and DEB serves Ubuntu/Debian direct installs. Store and repository
channels such as Flathub, COPR, OBS and AUR have independent policies and
maintainer workflows, so support will be added one channel at a time rather
than treating one package build as universal compatibility.

Linux system audio depends on an explicitly selected PipeWire or PulseAudio
monitor source. OYYO NotzUP does not bypass desktop permissions, protected
audio or participant-consent requirements.

Official background:

- [Ubuntu App Center package behavior](https://ubuntu.com/desktop/docs/en/24.04/explanation/snap-and-deb-packages/)
- [Snapcraft publishing](https://documentation.ubuntu.com/snapcraft/latest/how-to/publishing/)
- [Tauri Linux distribution formats](https://v2.tauri.app/distribute/)
- [Flathub submission requirements](https://docs.flathub.org/docs/for-app-authors/requirements)
