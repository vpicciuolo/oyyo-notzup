<!-- Copyright (c) 2026 HRN INNOVATION TECHNOLOGIES LTD -->

# Linux installation

Status: Linux x86-64 direct packages are available as a 1.0.0 preview after
Ubuntu, Debian and Fedora virtual-machine validation. The strict Snap also
passed local installation, confined CLI and rendered-GUI checks. The direct
packages are unsigned; physical-device QA and Snap Store review remain. Do not
install a copy hosted outside this
repository, an approved store listing or [notzup.com](https://notzup.com/).

The first x86-64 release is designed to provide:

- a portable AppImage graphical application;
- a DEB graphical application plus `oyyo-notzup-cli` for Ubuntu and Debian;
- an RPM graphical application plus `oyyo-notzup-cli` for Fedora-family
  systems;
- a confined Snap with GUI and `oyyo-notzup.cli` commands;
- a standalone CLI archive.

Download the GUI or CLI from the
[Linux 1.0.0 release](https://github.com/vpicciuolo/oyyo-notzup/releases/tag/v1.0.0-linux):

- [AppImage GUI](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-linux/OYYO-NotzUP-1.0.0-Linux-x86_64.AppImage)
- [Ubuntu/Debian DEB](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-linux/OYYO-NotzUP-1.0.0-Linux-x86_64.deb)
- [Fedora-family RPM](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-linux/OYYO-NotzUP-1.0.0-Linux-x86_64.rpm)
- [Strict Snap](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-linux/OYYO-NotzUP-1.0.0-Linux-x86_64.snap)
- [Standalone CLI archive](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-linux/OYYO-NotzUP-CLI-1.0.0-Linux-x86_64.tar.gz)
- [SHA-256 manifest](https://github.com/vpicciuolo/oyyo-notzup/releases/download/v1.0.0-linux/SHA256SUMS-linux.txt)

Wayland/X11, microphone, PipeWire/PulseAudio, camera and desktop-portal
behavior still need physical Linux validation.

## Direct installation

AppImage:

```bash
chmod +x OYYO-NotzUP-1.0.0-Linux-x86_64.AppImage
./OYYO-NotzUP-1.0.0-Linux-x86_64.AppImage
```

Ubuntu or Debian:

```bash
sudo apt install ./OYYO-NotzUP-1.0.0-Linux-x86_64.deb
```

Fedora-family distributions:

```bash
sudo dnf install ./OYYO-NotzUP-1.0.0-Linux-x86_64.rpm
```

Standalone CLI:

```bash
tar -xzf OYYO-NotzUP-CLI-1.0.0-Linux-x86_64.tar.gz
./OYYO-NotzUP-CLI-1.0.0-Linux-x86_64/bin/oyyo-notzup-cli --help
```

Direct Snap preview:

```bash
sudo snap install --dangerous ./OYYO-NotzUP-1.0.0-Linux-x86_64.snap
```

`--dangerous` is required because the downloaded Snap is not signed by the
Snap Store. Prefer the Store command below after its listing is approved.

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

Download the package and `SHA256SUMS-linux.txt` from the same tagged GitHub
Release, then run:

```bash
sha256sum --check SHA256SUMS-linux.txt
```

Only install after the checksum succeeds. This preview does not include a
detached OpenPGP signature; each direct package is explicitly distributed as
unsigned.

See [Linux distribution channels](LINUX_DISTRIBUTION.md) for the publication
plan and current release gates.
