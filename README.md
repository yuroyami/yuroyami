<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.svg">
  <img width="100%" src="assets/hero-light.svg" alt="yuroyami. Kotlin for everything.">
</picture>

I write everything in Kotlin. With Kotlin Multiplatform (KMP), one codebase
runs on Android, iOS, desktop, and web: you share the logic, and every platform
still gets native performance. I expect it to become the default way to build
cross-platform apps.

## Why I write the Kite libraries

Every Kite library is one of two things. Either a full Kotlin port of an
existing library, like KiteTorrent which ports libtorrent. Or a Kotlin/Native
cockpit over a native core, like KiteFFmpeg which drives FFmpeg in a
Kotlin-first, coroutine-first way. The goal is to depend on nothing if I can
help it. No bundled third-party library and no outside API. So when a bug shows
up it is the Kite library's own bug, and it gets fixed there.

It also means every Kite library behaves exactly the same on every platform,
because there is no expect/actual split underneath, or almost none. Most of
the code is Kotlin/Native, and sometimes all of it is.

I also want the Kite libraries to fit into the KMP world on the rendering side.
So wherever it makes sense there are Compose bindings and renderers. KitePDF,
KitePlayer and Kite3D all have them.

## Featured

<table align="left">
<tr><td align="center" width="380">
<br>
<img src="assets/logos/synkplay.png" width="72" height="72" alt="Synkplay logo"><br><br>
<b><a href="https://github.com/yuroyami/syncplay-mobile">Synkplay</a></b><br><br>
<img src="https://img.shields.io/badge/App-7F52FF?style=flat-square" alt="App"> <a href="https://github.com/yuroyami/syncplay-mobile/stargazers"><img src="https://img.shields.io/github/stars/yuroyami/syncplay-mobile?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56" alt="stars"></a><br><br>
Watch videos in sync with friends, in the same rooms as Syncplay for PC. Android and iOS.
<br><br>
</td></tr>
</table>

<table align="right">
<tr><td align="center" width="380">
<br>
<img src="assets/logos/kitepdf.svg" width="225" alt="KitePDF logo"><br><br>
<b><a href="https://github.com/yuroyami/KitePDF">KitePDF</a></b><br><br>
<img src="https://img.shields.io/badge/Library-7F52FF?style=flat-square" alt="Library"> <a href="https://github.com/yuroyami/KitePDF/stargazers"><img src="https://img.shields.io/github/stars/yuroyami/KitePDF?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56" alt="stars"></a><br><br>
Read, write, create, and display PDFs and EPUB books. Pure Kotlin, on Android, iOS, desktop, and web.
<br><br>
</td></tr>
</table>

<br clear="both">

<table align="left">
<tr><td align="center" width="380">
<br>
<img src="assets/logos/kiteplayer.svg" width="72" alt="KitePlayer logo">&nbsp;&nbsp;&nbsp;&nbsp;<img src="assets/logos/kiteffmpeg.png" width="72" alt="KiteFFmpeg logo"><br><br>
<b><a href="https://github.com/yuroyami/KitePlayer">KitePlayer</a></b> + <b><a href="https://github.com/yuroyami/KiteFFmpeg">KiteFFmpeg</a></b><br><br>
<img src="https://img.shields.io/badge/Library-7F52FF?style=flat-square" alt="Library"> <a href="https://github.com/yuroyami/KitePlayer/stargazers"><img src="https://img.shields.io/github/stars/yuroyami/KitePlayer?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56" alt="KitePlayer stars"></a> <a href="https://github.com/yuroyami/KiteFFmpeg/stargazers"><img src="https://img.shields.io/github/stars/yuroyami/KiteFFmpeg?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56" alt="KiteFFmpeg stars"></a><br><br>
Twins. KiteFFmpeg is FFmpeg as a plain Kotlin dependency: convert, trim, and transcode video and audio. One Gradle line, no NDK, no install. KitePlayer is the media player built on it, with a 100% Kotlin core: subtitles, live streams, hardware decode.
<br><br>
</td></tr>
</table>

<table align="right">
<tr><td align="center" width="380">
<br>
<img src="assets/logos/kiteconfig.png" width="72" alt="KiteConfig logo"><br><br>
<b><a href="https://github.com/yuroyami/KiteConfig">KiteConfig</a></b><br><br>
<img src="https://img.shields.io/badge/Gradle%20plugin-7F52FF?style=flat-square" alt="Gradle plugin"> <a href="https://github.com/yuroyami/KiteConfig/stargazers"><img src="https://img.shields.io/github/stars/yuroyami/KiteConfig?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56" alt="stars"></a><br><br>
Set your app name, logo, version, and IDs once, in one Gradle block. Android and iOS both read from it, so they never drift apart.
<br><br>
</td></tr>
</table>

<br clear="both">

## Upcoming Kite libraries

All of these exist and build. None is tested enough to trust yet, so their
repos stay private. Each one goes public once it proves it works.

| Library | Purpose |
| :--- | :--- |
| **KiteImage** | Load and save images (PNG, JPEG, GIF, WebP, and more) from shared code. |
| **KiteQR** | Scan and create QR codes and barcodes. |
| **KiteCore** | The small helpers every project rewrites: text, lists, dates, math, and coroutines. |
| **KiteArchive** | Zip and unzip anywhere, plus TAR, gzip, LZ4, and Snappy. |
| **KiteAudio** | Decode, encode, and tag audio files. |
| **Kite3D** | 3D math: vectors, matrices, quaternions, and collision shapes. |
| **KiteSynth** | A synthesizer: it reads a SoundFont, takes MIDI notes, and turns them into sound. |
| **KiteRT** | Real-time audio output. Your code makes the samples, KiteRT gets them to the speakers. |
| **KiteMIDI** | Read and write MIDI files, and talk to real instruments over USB and Bluetooth. |
| **KiteTorrent** | Download and seed torrents from shared code: magnet links, encryption, peer discovery. |

## Upcoming apps

Bigger things in the works, each one a single Kotlin codebase for every platform.

| App | Purpose |
| :--- | :--- |
| **PINGETTO** | Check your network latency with ping. |
| **Luddy** | One download manager for every screen: torrents and direct links, streamed while they download. |
| **ChatStrata** | Read the chat backups you download from Facebook, Instagram, Snapchat, and others. |
| **Peerora** | Send files between your devices. |

<div align="center">

<br>

<a href="mailto:evongintoki@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>

</div>

<img width="100%" src="assets/footer.svg" alt="">
