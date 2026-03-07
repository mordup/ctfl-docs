# Installation

Pre-built packages are available on the [Releases](https://github.com/mordup/ctfl/releases/latest) page.

## AppImage (any distro)

Download `CTFL-x86_64.AppImage`, make it executable, and run:

```bash
chmod +x CTFL-x86_64.AppImage
./CTFL-x86_64.AppImage
```

!!! tip
    Move the AppImage to a permanent location like `~/Applications/` so the built-in updater can replace it in place.

## pip

```bash
pip install ctfl
```

Or install from the `.whl` file on the releases page:

```bash
pip install ctfl-*.whl
```

## Arch Linux

Download the `.pkg.tar.zst` from the [Releases](https://github.com/mordup/ctfl/releases/latest) page:

```bash
sudo pacman -U ctfl-*-any.pkg.tar.zst
```

Or build from source:

```bash
git clone https://github.com/mordup/ctfl.git
cd ctfl
makepkg -si
```

## Debian / Ubuntu

```bash
sudo dpkg -i ctfl_*_amd64.deb
```

## Fedora / RPM

```bash
sudo rpm -i ctfl-*.x86_64.rpm
```

## Dependencies

- Python >= 3.11
- PyQt6
- keyring (for secure API key storage)

These are bundled in the AppImage and system packages. For pip installs, they are pulled automatically.
