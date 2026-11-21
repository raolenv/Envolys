<div align="center">

  <img src="assets/envolys-icon.png" width="160" alt="Envolys icon" />

  # Envolys

  <sub>A sleek, red-themed YouTube Music client for Android — open source, based on Metrolist, and focused on a clean listening experience.</sub>

  <br/>
  <br/>

  <a href="https://github.com/raolenv/Envolys/releases">
    <img src="https://img.shields.io/github/downloads/raolenv/Envolys/total?style=for-the-badge&color=B00020&labelColor=140A0E&label=Downloads" alt="Downloads">
  </a>
  <a href="https://github.com/raolenv/Envolys/stargazers">
    <img src="https://img.shields.io/github/stars/raolenv/Envolys?style=for-the-badge&color=FF4D5E&labelColor=140A0E&label=Stars" alt="Stars">
  </a>
  <a href="https://github.com/raolenv/Envolys/releases/latest">
    <img src="https://img.shields.io/github/v/release/raolenv/Envolys?style=for-the-badge&color=B00020&labelColor=140A0E&label=Release" alt="Release">
  </a>
  <a href="LICENSE">
    <img src="https://img.shields.io/badge/License-GPL--3.0-B00020?style=for-the-badge&labelColor=140A0E" alt="License">
  </a>

</div>

> [!WARNING]
> Envolys is still in early development (`0.0.2`). Expect bugs, rough edges, and breaking changes. Bug reports are welcome.

---

## What is Envolys?

Envolys is a fork/rebrand based on **[Metrolist](https://github.com/MetrolistGroup/Metrolist)**, keeping the powerful Metrolist base while evolving its own identity, visual direction, and audio experience.

- **Red-themed identity** — Envolys branding, icon, and package identity.
- **Metrolist base** — built on top of the Metrolist/Kotlin Multiplatform foundation.
- **Android first** — current build focus is Android while the codebase remains multiplatform.
- **No account required** — search, play, lyrics, and downloads can work without signing in.
- **Your data stays yours** — Envolys does not run its own account system for collecting your logins.

---

## How to install

1. Open the [latest release](https://github.com/raolenv/Envolys/releases/latest).
2. Download the APK that matches your device (if unsure, pick **arm64**; **universal** works everywhere but is larger).
3. Open the downloaded file and allow install from your browser/file manager if Android asks.
4. Open Envolys and start listening.

Updating works the same way: install the new APK over the old one and your library should stay.

> [!TIP]
> Only download Envolys from this repository's Releases page. Avoid random reuploads or modified APKs.

---

## Features

- YouTube Music playback with a modern Material UI
- Background playback, queue, lyrics, downloads, and library management
- Listen Together / room features (uses the existing Metrolist server/base behavior)
- Audio controls and customization from the Metrolist base
- **Audio Lab (WIP)** — being reworked with a Mochy-Music-inspired direction for Envolys

---

## Build it yourself (Android)

### Requirements

- Android Studio (latest stable) / JDK 21
- Android SDK 36
- Android NDK (as required by the project)
- Enough disk space for Gradle/Kotlin dependencies

### Build

```bash
git clone https://github.com/raolenv/Envolys.git
cd Envolys
./gradlew :androidApp:assembleDebug
```

The debug APK will be in:

```text
androidApp/build/outputs/apk/debug/
```

> [!NOTE]
> GitHub Actions in this repo are configured for **manual Android builds only** (`workflow_dispatch`) to avoid accidental CI builds on every push.

---

## Disclaimer

Envolys is an independent, unofficial project made for personal and educational use. It is provided as-is, without warranty of any kind.

- Envolys is **not affiliated with, endorsed by, or sponsored by** YouTube, YouTube Music, Google, or any other service it can connect to.
- Envolys does **not** host, store, or distribute any music or media. Content is fetched from third-party services.
- You are responsible for how you use the app, including third-party Terms of Service and local copyright laws.
- Support artists and creators by using official platforms/subscriptions when possible.

---

## Credits & License

Envolys is based on **Metrolist** and keeps Metrolist's license.

- **Metrolist** — [MetrolistGroup/Metrolist](https://github.com/MetrolistGroup/Metrolist)
- **Mochy-Music** — [realidkroo/Mochy-Music](https://github.com/realidkroo/Mochy-Music) (README style inspiration and Audio Lab reference direction)
- **Innertube/YouTube Music ecosystem projects** used by the upstream base

This project is licensed under **[GPL-3.0](LICENSE)**, the same license as Metrolist. See `LICENSE` for full terms.
