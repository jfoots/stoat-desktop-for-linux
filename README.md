# 📦 Stoat Desktop — Community Linux Packages

![GitHub release](https://img.shields.io/github/v1.3.0/release/jfoots/stoat-desktop-for-linux?display_name=tag&logo=github)
![GitHub downloads](https://img.shields.io/github/downloads/jfoots/stoat-desktop-for-linux/total?logo=github)
![Fedora](https://img.shields.io/badge/Fedora-43%20%7C%2042-294172?logo=fedora&logoColor=white)
![RHEL / EPEL](https://img.shields.io/badge/EPEL-9-8A2BE2?logo=redhat&logoColor=white)
![Arch Linux](https://img.shields.io/badge/Arch-rolling-1793D1?logo=arch-linux&logoColor=white)
![Debian](https://img.shields.io/badge/Debian-bookworm-A81D33?logo=debian&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-noble-E95420?logo=ubuntu&logoColor=white)
![x86_64](https://img.shields.io/badge/Arch-x86__64-blue)
![ARM64](https://img.shields.io/badge/Arch-aarch64-green)

---

This repository hosts **community-built Linux packages** for **Stoat Chat Desktop** across multiple distributions.

Supported platforms:

- 🟥 Fedora  
- 🟥 RHEL / EPEL 9  
- 🟦 Arch Linux  
- 🟨 Debian  
- 🟧 Ubuntu  
- Multi-arch: `x86_64 / amd64` and `aarch64 / arm64`

Upstream project:  
https://stoat.chat

---

# 🚀 Installation Instructions

## 🟥 Fedora / RHEL / EPEL (RPM)

### Direct Install

```bash
sudo dnf install ./stoat-<version>.fc<release>.<arch>.rpm
```

Example:

```bash
sudo dnf install ./stoat-1.3.0-1.fc44.x86_64.rpm
```

---

## 🟦 Arch Linux

### Install Package

```bash
sudo pacman -U stoat-<version>-<arch>.pkg.tar.zst
```

### Or Build from PKGBUILD

```bash
makepkg -si
```

---

## 🟨 Debian / Ubuntu

```bash
sudo dpkg -i stoat_<version>_<arch>.deb
sudo apt-get -f install
```

---

# 🏗 Build Infrastructure

Packages are built in clean environments using:

- `mock` for RPM-based systems  
- `dpkg-buildpackage` for Debian-based systems  
- `makepkg` for Arch Linux  
- Multi-architecture containerized builds  

All builds are reproducible and automated.

---

# 📂 Repository Structure

```
dist/
  rpm/
    fedora-43/
    fedora-42/
    epel-9/
  deb/
    bookworm/
    noble/
  arch/
    x86_64/
```

---

# 🔄 Updating

- Fedora / RHEL:
  ```bash
  sudo dnf upgrade stoat
  ```

- Arch:
  ```bash
  sudo pacman -Syu stoat
  ```

- Debian / Ubuntu:
  ```bash
  sudo apt upgrade stoat
  ```

---

# 📜 License

Stoat is licensed under:

AGPL-3.0-only

This repository provides redistribution builds of the official upstream desktop bundle.

---

# ⚠ Disclaimer

This is a community packaging effort and is not an official distribution channel of the Stoat project.
