<div align="center">

# NextStream

**Your library. Your screens. Press play.**

[![Latest release](https://img.shields.io/github/v/release/nextstream-admin/nextstream-release?label=latest&style=flat-square&color=111111)](https://github.com/nextstream-admin/nextstream-release/releases/latest)
[![Website](https://img.shields.io/badge/website-nextstream.pages.dev-111111?style=flat-square)](https://nextstream.pages.dev)
[![Platforms](https://img.shields.io/badge/platforms-macOS%20%C2%B7%20Windows%20%C2%B7%20Tizen%20%C2%B7%20webOS%20%C2%B7%20Android-111111?style=flat-square)](#download)

Official desktop, TV and Android installers for **NextStream** — a debrid-only
streaming client built for the big screen.

[**Download the latest release →**](https://github.com/nextstream-admin/nextstream-release/releases/latest)

</div>

---

## Download

| Platform | Package | Version | Size |  |
| :--- | :--- | :---: | ---: | :--- |
| **macOS** · Apple Silicon | `NextStream-macOS-arm64-v0.3.16.dmg` | `0.3.16` | 31.4 MB | [**Download**](https://github.com/nextstream-admin/nextstream-release/releases/download/installers-2026-11-06/NextStream-macOS-arm64-v0.3.16.dmg) |
| **Windows** · x64 | `NextStream-Windows-x64-v0.3.16.exe` | `0.3.16` | 41.9 MB | [**Download**](https://github.com/nextstream-admin/nextstream-release/releases/download/installers-2026-11-06/NextStream-Windows-x64-v0.3.16.exe) |
| **Samsung TV** · Tizen | `NextStream-Samsung-Tizen-v0.0.8.wgt` | `0.0.8` | 46.8 KB | [**Download**](https://github.com/nextstream-admin/nextstream-release/releases/download/installers-2026-11-06/NextStream-Samsung-Tizen-v0.0.8.wgt) |
| **LG TV** · webOS | `NextStream-LG-webOS-v0.0.10.ipk` | `0.0.10` | 44.4 KB | [**Download**](https://github.com/nextstream-admin/nextstream-release/releases/download/installers-2026-11-06/NextStream-LG-webOS-v0.0.10.ipk) |
| **Android TV** | `NextStream-Android-v0.3.20.apk` | `0.3.20` | 32.8 MB | [**Download**](https://github.com/nextstream-admin/nextstream-release/releases/download/installers-2026-11-06/NextStream-Android-v0.3.20.apk) |

> [!NOTE]
> The TV packages are **shell loaders**, not copies of the web app. Their versions move
> separately from the desktop and Android builds. The app itself updates from the
> service when the TV launches.

---

## Before you install

> [!WARNING]
> These builds are **unsigned, unnotarized or debug-signed**. macOS is unnotarized,
> Windows is unsigned, and the Android APK is debug-signed. Your OS may warn you.
> Only run packages downloaded from this repository.

| Platform | Install notes |
| :--- | :--- |
| **macOS** | Apple Silicon (arm64) only. Open the DMG and drag **NextStream** into Applications. If macOS blocks it: **System Settings → Privacy & Security → Open Anyway**. No Intel or universal build is published here. |
| **Windows** | Windows x64. Run the installer and launch **NextStream** from the Start menu. SmartScreen may warn because the installer is unsigned; choose **More info → Run anyway** only if you trust the source. |
| **Samsung Tizen** | `.wgt` package for a Tizen TV. Install through Tizen developer mode with the Samsung/Tizen tooling. The package version is the **shell** version; the app version is shown inside NextStream. |
| **LG webOS** | `.ipk` package for a webOS TV. Install through LG Developer Mode with the webOS CLI. The package version is the **shell** version; the app version is shown inside NextStream. |
| **Android TV** | Sideload the `.apk` on Android TV, Google TV or Fire TV. Enable **Install unknown apps** for your file manager / ADB first. This is a debug-signed build, not a Play Store release. |
| **Browser** | No installer. Open **[nextstream.pages.dev](https://nextstream.pages.dev)** and choose **Watch in your browser**. WatchSync sign-in is required; there is no anonymous route. |

---

## Verify your download

Every release ships a `SHA256SUMS.txt` next to the installers.

```sh
# macOS
shasum -a 256 -c SHA256SUMS.txt

# Windows / Linux
sha256sum -c SHA256SUMS.txt
```

[**Download checksums**](https://github.com/nextstream-admin/nextstream-release/releases/download/installers-2026-11-06/SHA256SUMS.txt) ·
[**All releases**](https://github.com/nextstream-admin/nextstream-release/releases)

---

## What you are downloading

NextStream keeps the catalogue, search, profiles, subtitles and playback UI in the
app, and uses the platform's native video pipeline where one exists:

| Surface | Player |
| :--- | :--- |
| macOS / Windows | native **libmpv** surface below the app window |
| Samsung Tizen | **AVPlay** |
| LG webOS | native **video pipeline** |
| Android TV | **ExoPlayer / Media3** |
| Browser | the same web app at [nextstream.pages.dev](https://nextstream.pages.dev) |

Using NextStream requires a **WatchSync** account and a supported debrid service. NextStream does not host or provide media.

---

## Links

| | |
| :--- | :--- |
| Website | [nextstream.pages.dev](https://nextstream.pages.dev) |
| Latest release | [github.com/nextstream-admin/nextstream-release/releases/latest](https://github.com/nextstream-admin/nextstream-release/releases/latest) |
| Issues / feedback | [Open an issue](https://github.com/nextstream-admin/nextstream-release/issues) |
| Previous builds | [All releases](https://github.com/nextstream-admin/nextstream-release/releases) |

<div align="center">
<sub>NextStream · Press play.</sub>
</div>
