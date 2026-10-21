# Folio

Folio is a focused document editor for Typst, with a live preview and a simple mode that works like a word processor. This repository holds its downloads.

## Download Folio 0.3.0

| System | Download |
| --- | --- |
| macOS (Apple Silicon) | [Disk image (.dmg)](https://github.com/Turtlezztz/folio-releases/releases/download/v0.3.0/Folio-0.3.0-macos-arm64.dmg) · [Zip](https://github.com/Turtlezztz/folio-releases/releases/download/v0.3.0/Folio-0.3.0-macos-arm64.zip) |
| Windows (x64) | [Installer (.exe)](https://github.com/Turtlezztz/folio-releases/releases/download/v0.3.0/Folio-0.3.0-windows-x64-setup.exe) · [Portable zip](https://github.com/Turtlezztz/folio-releases/releases/download/v0.3.0/Folio-0.3.0-windows-x64.zip) |
| Ubuntu / Debian | [folio_0.3.0-1_amd64.deb](https://github.com/Turtlezztz/folio-releases/releases/download/v0.3.0/folio_0.3.0-1_amd64.deb) |
| Fedora | [folio-0.3.0-1.x86_64.rpm](https://github.com/Turtlezztz/folio-releases/releases/download/v0.3.0/folio-0.3.0-1.x86_64.rpm) |
| Arch Linux | [folio-0.3.0-1-x86_64.pkg.tar.zst](https://github.com/Turtlezztz/folio-releases/releases/download/v0.3.0/folio-0.3.0-1-x86_64.pkg.tar.zst) |
| Other Linux | [Folio-0.3.0-linux-x64.tar.gz](https://github.com/Turtlezztz/folio-releases/releases/download/v0.3.0/Folio-0.3.0-linux-x64.tar.gz) |

Checksums: [SHA256SUMS.txt](https://github.com/Turtlezztz/folio-releases/releases/download/v0.3.0/SHA256SUMS.txt) · Older versions: [Releases](https://github.com/Turtlezztz/folio-releases/releases)

## Install

On first launch Folio offers to download its PDF renderer (PDFium), language service (Tinymist) and the Typst documentation (about 55 MB). You can also do that later in Settings › Components.

**macOS (Apple Silicon):** open `Folio-0.3.0-macos-arm64.dmg` and drag Folio to Applications. Folio is not notarized yet, so macOS blocks it the first time. Go to System Settings › Privacy & Security and click **Open Anyway**.

**Windows (x64):** run `Folio-0.3.0-windows-x64-setup.exe`. The installer is not signed yet, so SmartScreen may show "Windows protected your PC". Click **More info › Run anyway**. `Folio-0.3.0-windows-x64.zip` is a portable copy: unzip it and run `folio.exe`.

**Ubuntu / Debian:** `sudo apt install ./folio_0.3.0-1_amd64.deb`

**Fedora:** `sudo dnf install ./folio-0.3.0-1.x86_64.rpm`

**Arch Linux:** `sudo pacman -U folio-0.3.0-1-x86_64.pkg.tar.zst`

**NixOS / Nix:** `nix run github:Turtlezztz/typst-editor/v0.3.0`, or add the flake's `packages.<system>.folio` (or `overlays.default`) to your configuration. It builds from source and uses Tinymist and PDFium from nixpkgs.

**Other Linux:** unpack `Folio-0.3.0-linux-x64.tar.gz` and run `folio-0.3.0/folio`. The `share/` folder holds a desktop entry and icons for `~/.local/share`.

The Linux packages need glibc 2.39 or newer (Ubuntu 24.04, Fedora 40, Debian 13 or later) and a Vulkan driver (`mesa-vulkan-drivers` on Ubuntu and Fedora, `vulkan-radeon`/`vulkan-intel`/`nvidia-utils` on Arch).

`SHA256SUMS.txt` lists the checksum of every file.
