# Android-x86 9.0-r2 (64-bit) ISO mirror

Unmodified mirror of `android-x86_64-9.0-r2.iso` from the [Android-x86 project](https://www.android-x86.org/), hosted as a GitHub Release asset for use with the in-browser Bochs x86-64 emulator (`android9-bochs.html`).

This is **not** an official distribution and is **not** affiliated with Google or the Android-x86 project. Android is a trademark of Google LLC.

## Download

Get `android-x86_64-9.0-r2.iso` from the [Releases](../../releases) page. The ISO is too large for a normal repo file, so it is only attached to the release.

## Verify

The file is byte-for-byte identical to the official release (965,738,496 bytes):

| Hash   | Value |
|--------|-------|
| SHA256 | `f7eb8fc56f29ad5432335dc054183acf086c539f3990f0b6e9ff58bd6df4604e` |
| SHA1   | `1cc85b5ed7c830ff71aecf8405c7281a9c995aa0` |
| MD5    | `e9ba997cede7bf3514d2ba3e624ff767` |

```bash
# Linux / macOS
sha256sum android-x86_64-9.0-r2.iso

# Windows (PowerShell)
Get-FileHash .\android-x86_64-9.0-r2.iso -Algorithm SHA256
```

If the hash doesn't match, don't use the file.

## What it is

- Android-x86 9.0-r2, based on Android 9.0.0 Pie (`android-9.0.0_r54`)
- Linux kernel 4.19.110 LTS
- 64-bit, bootable live/installer ISO (legacy BIOS and UEFI)
- Plain AOSP build: **no Google apps (GApps) or other proprietary Google software**

## Use with the Bochs page

1. Open `android9-bochs.html` in a desktop browser.
2. Click **Boot built-in demo** first. `test64 PASSED` means the 64-bit emulator works on your machine.
3. Under the ISO file input, select `android-x86_64-9.0-r2.iso` and boot it.

Bochs interprets x86-64 in WebAssembly, so it is roughly 1000x slower than native. Expect very long boot times.

## Licences

Android-x86 is a mix of open-source components under their own licences:

- Most of Android (AOSP) is under the [Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0)
- The Linux kernel and other components are under the [GNU GPL v2](https://www.gnu.org/licenses/old-licenses/gpl-2.0.html)
- Other components carry their own licences, shipped inside the image

This repository contains no changes to the ISO. All licence notices are preserved inside it.

## Source code

Corresponding source for the GPL components is available from the upstream project:

- Android-x86 source on GitHub: https://github.com/android-x86
- Project page and downloads: https://osdn.net/projects/android-x86/
- Release notes: https://www.android-x86.org/releases/releasenote-9-0-r2.html

## Original sources

- OSDN: https://osdn.net/projects/android-x86/downloads/71931/android-x86_64-9.0-r2.iso/
- SourceForge: https://sourceforge.net/projects/android-x86/files/Release%209.0/
- FossHub: https://www.fosshub.com/Android-x86.html

## Takedown

If you are a rights holder and want this removed, open an issue and it will be taken down.
