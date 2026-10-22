<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Linux installation

Status: Linux x86-64 direct packages passed Ubuntu, Debian and Fedora virtual-
machine validation. The strict Snap also passed local installation, confined
CLI and rendered-GUI checks. Signing, physical-device QA, store review and
publication are still pending. Do not install a copy hosted outside this
repository, an approved store listing or [notzup.com](https://notzup.com/).

The first x86-64 release is designed to provide:

- a portable AppImage graphical application;
- a DEB graphical application plus `oyyo-notzup-cli` for Ubuntu and Debian;
- an RPM graphical application plus `oyyo-notzup-cli` for Fedora-family
  systems;
- a confined Snap with GUI and `oyyo-notzup.cli` commands;
- a standalone CLI archive.

Every direct package must pass clean-install tests and be published with a
SHA-256 manifest and detached signature before links appear here. Wayland/X11,
microphone, PipeWire/PulseAudio, camera and desktop-portal behavior still need
physical Linux validation.

## Ubuntu App Center

The planned Ubuntu catalog route is the Snap Store. After Canonical accepts and
publishes the stable revision, Ubuntu users will be able to find it in App
Center or install it with:

```bash
sudo snap install oyyo-notzup
```

This command is not expected to work until the public Snap listing exists.
Ubuntu App Center normally shows Snap Store applications by default. A direct
DEB can also be installed manually, but it is not automatically listed in App
Center's repository search merely because it exists on GitHub.

Snap audio recording permission is separate from installation. If it has not
been granted through Ubuntu's app permissions, connect it explicitly:

```bash
sudo snap connect oyyo-notzup:audio-record
```

## Direct package verification

When the public Linux release is available, download the package and
`SHA256SUMS-linux.txt` from the same tagged GitHub Release, then run:

```bash
sha256sum --check SHA256SUMS-linux.txt
gpg --verify SHA256SUMS-linux.txt.asc SHA256SUMS-linux.txt
```

Only install after both checks succeed with the published OYYO release key.
The key fingerprint and exact supported-distribution matrix will be added when
the first release is approved.

See [Linux distribution channels](LINUX_DISTRIBUTION.md) for the publication
plan and current release gates.
