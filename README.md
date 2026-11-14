# Daemon downloads

Installers for [Daemon](https://daemon.bitwise0x.com), a 3D desktop companion for macOS, Windows and Linux.

Each release holds every installer for that version and a `SHA256SUMS` file with their checksums. The site's [Download page](https://daemon.bitwise0x.com/download) picks the right file for a computer.

| Platform | File | Install |
|---|---|---|
| macOS, Apple silicon and Intel | `Daemon-<version>-universal.dmg` | open the image and drag Daemon to Applications; the first time, right-click the app and choose Open |
| Windows x64 | `Daemon.Setup.<version>.exe` | run it; SmartScreen asks once |
| Linux x64 and arm64 | `Daemon-<version>-<arch>.AppImage` | `chmod +x`, then run it |
| Debian and Ubuntu | `Daemon-<version>-<amd64 or arm64>.deb` | `sudo apt install ./Daemon-<version>-<arch>.deb` |
| Chromebook | the `.deb` for its CPU | the same `apt install`, in the Linux environment's terminal |

The builds are unsigned.

To check a download, compare its SHA-256 with the line for it in `SHA256SUMS`:

```sh
shasum -a 256 Daemon-<version>-universal.dmg
```
