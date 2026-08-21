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
| **[KitePDF](https://github.com/yuroyami/KitePDF)** | Read, write, edit, and render PDF files. Read EPUB 2 and 3 books. Includes an optional Compose Multiplatform viewer. | [![kitepdf](https://img.shields.io/maven-central/v/io.github.yuroyami/kitepdf?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kitepdf) | [![stars](https://img.shields.io/github/stars/yuroyami/KitePDF?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KitePDF/stargazers) |
| **[KiteCodec](https://github.com/yuroyami/KiteCodec)** | Wraps FFmpeg through cinterop: demux, decode, filter, encode, transcode, remux. A Gradle plugin fetches the binaries. | ![source only](https://img.shields.io/badge/source%20only-8a8f98?style=flat-square) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteCodec?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteCodec/stargazers) |
| **[KitePlayer](https://github.com/yuroyami/KitePlayer)** | Media player on top of FFmpeg. Hardware decode, HDR, subtitles, live streams. No ExoPlayer, AVPlayer, or libmpv underneath. | ![source only](https://img.shields.io/badge/source%20only-8a8f98?style=flat-square) | ![stars](https://img.shields.io/badge/%E2%98%85%200-444c56?style=flat-square) |
| **[KiteCore](https://github.com/yuroyami/KiteCore)** | Cross-platform utilities for text, collections, coroutines, math, and time. | [![kitecore](https://img.shields.io/maven-central/v/io.github.yuroyami/kitecore?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kitecore) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteCore?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteCore/stargazers) |
| **[KiteQR](https://github.com/yuroyami/KiteQR)** | Read and create QR, Aztec, Data Matrix, PDF417, and common 1D barcodes. Optional Compose Multiplatform UI module. | [![kiteqr](https://img.shields.io/maven-central/v/io.github.yuroyami/kiteqr?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kiteqr) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteQR?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteQR/stargazers) |
| **[KiteImage](https://github.com/yuroyami/KiteImage)** | Read and write PNG, JPEG, GIF, and BMP. Read TIFF, JPEG 2000, and lossless WebP. Optional Compose and Coil modules. | [![kiteimage](https://img.shields.io/maven-central/v/io.github.yuroyami/kiteimage?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kiteimage) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteImage?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteImage/stargazers) |
| **[KiteArchive](https://github.com/yuroyami/KiteArchive)** | Read and write ZIP files. Read TAR, ar, and cpio. Compress with DEFLATE, gzip, zlib, LZ4, or Snappy. | [![kitearchive](https://img.shields.io/maven-central/v/io.github.yuroyami/kitearchive?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kitearchive) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteArchive?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteArchive/stargazers) |
| **[Kite3D](https://github.com/yuroyami/Kite3D)** | Vectors, matrices, quaternions, colors, and bounding volumes for 3D math. No renderer. | [![kite3d](https://img.shields.io/maven-central/v/io.github.yuroyami/kite3d?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kite3d) | [![stars](https://img.shields.io/github/stars/yuroyami/Kite3D?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/Kite3D/stargazers) |

### Upcoming

Still being built. The source is public, but there is nothing to depend on yet.

| Library | Purpose |
| :--- | :--- |
| **[KiteAudio](https://github.com/yuroyami/KiteAudio)** | Decode and encode audio, read common containers, and edit metadata. |
| **[KiteTorrent](https://github.com/yuroyami/KiteTorrent)** | Download and seed torrents with DHT, µTP, magnet links, encryption, and BitTorrent v2. |

## 🔌 Gradle plugin

| Plugin | Purpose | Release | Stars |
| :--- | :--- | :--- | :--- |
| **[KiteSSOT](https://github.com/yuroyami/KiteSSOT)** | App name, version, and bundle IDs live in one Kotlin config. Android and iOS both read from it, so they stay in sync. | [![kitessot](https://img.shields.io/gradle-plugin-portal/v/io.github.yuroyami.kitessot?style=flat-square&label=&color=02303A)](https://plugins.gradle.org/plugin/io.github.yuroyami.kitessot) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteSSOT?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteSSOT/stargazers) |

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
