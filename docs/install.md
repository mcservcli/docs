# Installation

## Linux
Arch Linux: `yay -S mcserv` (Or bleeding build: `yay -S mcserv-git`) (Packages: [mcserv](https://aur.archlinux.org/packages/mcserv), [mcserv-git](https://aur.archlinux.org/packages/mcserv-git))

### Manual Install
```bash
curl -fsSL https://github.com/DRSchlaubi/mcserv/releases/download/v{{ version }}/mcserv-{{ version }}-linux.tar.gz -o mcserv-{{ version }}-linux.tar.gz
mkdir -p /opt/mcserv
tar -xzvf mcserv-{{ version }}-linux.tar.gz -o /opt/mcserv/
rm mcserv-{{ version }}-linux.tar.gz
chmod 755 /opt/mcserv/mcserv
ln -s /opt/mcserv/mcserv /usr/bin/mcserv
```

## Windows
winget: `winget install mcserv`

Chocolatey: `choco install mcserv` (Package: [mcserv](https://community.chocolatey.org/packages/mcserv))

Scoop: `scoop install mcserv` (Package: soon)

Manual: [https://github.com/DRSchlaubi/mcserv/releases/download/v{{ version }}/mcserv-{{ version }}.msi](https://github.com/DRSchlaubi/mcserv/releases/download/v{{ version }}/mcserv-{{ version }}.msi)

## macOS
Coming Soon

# Installing from Source
See [Installing from Source](developers/compile_from_source.md)