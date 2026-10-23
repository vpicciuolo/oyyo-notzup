<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# OYYO NotzUP 1.0.0 for Linux

This preview release contains the x86-64 OYYO NotzUP desktop application and
local command-line interface. Supported local capture, transcription, search
and AI work remains on the device unless the user explicitly selects an online
or connected feature.

## Packages

- AppImage: portable graphical application.
- DEB: graphical application plus `oyyo-notzup-cli` for Ubuntu and Debian.
- RPM: graphical application plus `oyyo-notzup-cli` for Fedora-family systems.
- Snap: strict-confined graphical application plus `oyyo-notzup.cli`.
- CLI archive: standalone command-line binary and notices.

The packages passed Ubuntu 22.04, Debian 12 and Fedora 44 virtual-machine and
container tests. The AppImage, installed DEB and strict Snap GUIs were rendered
and visually inspected. The CLI was executed from every applicable package.

These direct files are not distribution-store or code signed. Verify downloads
with `SHA256SUMS-linux.txt`. Physical Linux testing for microphone, system
audio, camera, screen capture, Wayland/X11 and desktop portals remains pending.

Linux screen and system-audio availability depends on the desktop session,
PipeWire/PulseAudio routing, permissions and source application. NotzUP does
not bypass operating-system or participant-consent controls.

Copyright © 2026 HRN INNOVATION TECHNOLOGIES LTD.
