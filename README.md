<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.svg">
  <img width="100%" src="assets/hero-light.svg" alt="yuroyami. Kotlin for everything. Kotlin Multiplatform libraries and apps.">
</picture>

## Why I love KMP

I write everything in Kotlin. With Kotlin Multiplatform (KMP), one codebase
runs on Android, iOS, desktop, and web: you share the logic, and every platform
still gets native performance. I expect it to become the default way to build
cross-platform apps.

## Why I write the Kite libraries

The Kite libraries are written in pure Kotlin, and nearly all of them depend on
nothing at all: no JNI, no bundled binaries, no third-party code underneath.
That keeps things predictable. The same code runs on every platform, so it
behaves the same on every platform. And when something breaks, the bug is in
the library itself, where I can fix it, not buried in a native dependency I
have no control over.

You do not even need a KMP project to use them. The libraries are small, and a
plain Swift or Objective-C iOS app can add one like any other framework.

## 🪁 Kite libraries in 100% pure Kotlin

| Library | Purpose | Release | Stars |
| :--- | :--- | :--- | :--- |
| **[KitePDF](https://github.com/yuroyami/KitePDF)** | **TL;DR:** Read, write, and display PDFs and EPUB books.<br>**What it does:** Open a PDF, grab its text, edit it, or build a new one from scratch. Reads EPUB 2 and 3 too. Want to show pages on screen? A ready-made Compose viewer comes with it. | [![kitepdf](https://img.shields.io/maven-central/v/io.github.yuroyami/kitepdf?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kitepdf) | [![stars](https://img.shields.io/github/stars/yuroyami/KitePDF?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KitePDF/stargazers) |
| **[KiteCodec](https://github.com/yuroyami/KiteCodec)** | **TL;DR:** Convert and edit video and audio files.<br>**What it does:** Change format, resize, trim, crop, swap the codec, or drop the audio track. It is FFmpeg, except you call it from Kotlin instead of writing command lines. | ![source only](https://img.shields.io/badge/source%20only-8a8f98?style=flat-square) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteCodec?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteCodec/stargazers) |
| **[KitePlayer](https://github.com/yuroyami/KitePlayer)** | **TL;DR:** Play video and audio in your app.<br>**What it does:** One player for every platform, behaving the same on all of them. Handles subtitles, live streams, and seeking. | ![source only](https://img.shields.io/badge/source%20only-8a8f98?style=flat-square) | ![stars](https://img.shields.io/badge/%E2%98%85%200-444c56?style=flat-square) |
| **[KiteCore](https://github.com/yuroyami/KiteCore)** | **TL;DR:** The little helpers you rewrite in every project.<br>**What it does:** Around 450 shortcuts for text, lists, dates, math, and coroutines. Plus the few things KMP is missing, like running work off the main thread the same way everywhere. | [![kitecore](https://img.shields.io/maven-central/v/io.github.yuroyami/kitecore?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kitecore) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteCore?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteCore/stargazers) |
| **[KiteQR](https://github.com/yuroyami/KiteQR)** | **TL;DR:** Scan and create QR codes and barcodes.<br>**What it does:** Reads QR, Aztec, Data Matrix, PDF417, and the usual 1D barcodes out of an image. Creates them as PNG or SVG. Optional Compose UI included. | [![kiteqr](https://img.shields.io/maven-central/v/io.github.yuroyami/kiteqr?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kiteqr) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteQR?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteQR/stargazers) |
| **[KiteImage](https://github.com/yuroyami/KiteImage)** | **TL;DR:** Load and save images without platform code.<br>**What it does:** Opens PNG, JPEG, GIF, BMP, TIFF, JPEG 2000, and WebP into pixels you can use in shared code. Animated GIF and WebP work too. Plugs into Compose and Coil. | [![kiteimage](https://img.shields.io/maven-central/v/io.github.yuroyami/kiteimage?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kiteimage) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteImage?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteImage/stargazers) |
| **[KiteArchive](https://github.com/yuroyami/KiteArchive)** | **TL;DR:** Zip and unzip, on any platform.<br>**What it does:** Read and write ZIP files, read TAR and older archive formats, and compress with gzip, LZ4, or Snappy. All from shared code. | [![kitearchive](https://img.shields.io/maven-central/v/io.github.yuroyami/kitearchive?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kitearchive) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteArchive?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteArchive/stargazers) |
| **[Kite3D](https://github.com/yuroyami/Kite3D)** | **TL;DR:** 3D math, with three.js's API.<br>**What it does:** Vectors, matrices, rotations, colors, and collision shapes. It draws nothing. It only does the math. | [![kite3d](https://img.shields.io/maven-central/v/io.github.yuroyami/kite3d?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kite3d) | [![stars](https://img.shields.io/github/stars/yuroyami/Kite3D?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/Kite3D/stargazers) |

### Upcoming

Still being built. The source is public, but there is nothing to depend on yet.

| Library | Purpose |
| :--- | :--- |
| **[KiteAudio](https://github.com/yuroyami/KiteAudio)** | **TL;DR:** Read, write, and tag audio files.<br>**What it does:** Opens FLAC, WAV, AIFF, MP3, and Vorbis. Edit titles, artists, and artwork without touching the audio itself.
| **[KiteTorrent](https://github.com/yuroyami/KiteTorrent)** | **TL;DR:** Download and seed torrents from shared code.<br>**What it does:** Magnet links, peer discovery, encryption, and proxies. Nothing native to ship with your app.

## 🔌 Gradle plugin

| Plugin | Purpose | Release | Stars |
| :--- | :--- | :--- | :--- |
| **[KiteSSOT](https://github.com/yuroyami/KiteSSOT)** | **TL;DR:** One place for your app name, version, and IDs.<br>**What it does:** Set them once in your root Gradle file. Android and iOS both read from there, so they never fall out of sync. | [![kitessot](https://img.shields.io/gradle-plugin-portal/v/io.github.yuroyami.kitessot?style=flat-square&label=&color=02303A)](https://plugins.gradle.org/plugin/io.github.yuroyami.kitessot) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteSSOT?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteSSOT/stargazers) |

## 📱 KMP apps

One codebase for Android and iOS, UI included, built with Compose Multiplatform.

| App | Purpose | Stars |
| :--- | :--- | :--- |
| **[Synkplay](https://github.com/yuroyami/syncplay-mobile)** | Watch videos in sync with friends. Talks to the same rooms as the Syncplay desktop client. | [![stars](https://img.shields.io/github/stars/yuroyami/syncplay-mobile?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/syncplay-mobile/stargazers) |
| **[Pingy](https://github.com/yuroyami/PINGY)** | Measure network latency with ping. | [![stars](https://img.shields.io/github/stars/yuroyami/PINGY?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/PINGY/stargazers) |
| **[DuelistLP](https://github.com/yuroyami/DuelistLP)** | Track life points for two-player Yu-Gi-Oh games. | [![stars](https://img.shields.io/github/stars/yuroyami/DuelistLP?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/DuelistLP/stargazers) |

<div align="center">

<br>

<a href="mailto:evongintoki@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>

</div>

<img width="100%" src="assets/footer.svg" alt="">
