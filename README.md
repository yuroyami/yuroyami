<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.svg">
  <img width="100%" src="assets/hero-light.svg" alt="yuroyami. Kotlin for everything.">
</picture>

I mostly write Kotlin Multiplatform (KMP) libraries. I keep their dependencies
to a minimum. I also aim for zero `expect`/`actual` declarations which makes
commonMain code run the same on every platform.

I use AI tools to automate most of my work. I review their output carefully, so
the quality matches what I would write by hand.

## Featured

<table align="left">
<tr><td align="center" width="380">
<br>
<img src="assets/logos/synkplay.png" width="72" height="72" alt="Synkplay logo"><br><br>
<b><a href="https://github.com/yuroyami/syncplay-mobile">Synkplay</a></b><br><br>
<img src="https://img.shields.io/badge/App-7F52FF?style=flat-square" alt="App"> <a href="https://github.com/yuroyami/syncplay-mobile/stargazers"><img src="https://img.shields.io/github/stars/yuroyami/syncplay-mobile?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56" alt="stars"></a><br><br>
Watch videos in sync with friends on Android and iOS. Anyone on a computer can join the same room with Syncplay.
<br><br>
</td></tr>
</table>

<table align="right">
<tr><td align="center" width="380">
<br>
<img src="assets/logos/kitepdf.svg" width="225" alt="KitePDF logo"><br><br>
<b><a href="https://github.com/yuroyami/KitePDF">KitePDF</a></b><br><br>
<img src="https://img.shields.io/badge/Library-7F52FF?style=flat-square" alt="Library"> <a href="https://github.com/yuroyami/KitePDF/stargazers"><img src="https://img.shields.io/github/stars/yuroyami/KitePDF?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56" alt="stars"></a><br><br>
Read, create, edit, and display PDFs, and open EPUB books. It is pure Kotlin, so the same code runs on Android, iOS, desktop, and the web.
<br><br>
</td></tr>
</table>

<br clear="both">

<table align="left">
<tr><td align="center" width="380">
<br>
<img src="assets/logos/kiteplayer.svg" width="72" alt="KitePlayer logo">&nbsp;&nbsp;&nbsp;&nbsp;<img src="assets/logos/kiteffmpeg.svg" width="72" height="72" alt="KiteFFmpeg logo"><br><br>
<b><a href="https://github.com/yuroyami/KitePlayer">KitePlayer</a></b> + <b><a href="https://github.com/yuroyami/KiteFFmpeg">KiteFFmpeg</a></b><br><br>
<img src="https://img.shields.io/badge/Library-7F52FF?style=flat-square" alt="Library"> <a href="https://github.com/yuroyami/KitePlayer/stargazers"><img src="https://img.shields.io/github/stars/yuroyami/KitePlayer?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56" alt="KitePlayer stars"></a> <a href="https://github.com/yuroyami/KiteFFmpeg/stargazers"><img src="https://img.shields.io/github/stars/yuroyami/KiteFFmpeg?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56" alt="KiteFFmpeg stars"></a><br><br>
KiteFFmpeg adds FFmpeg to your project as one Gradle dependency, with no NDK and nothing to install. Use it to convert, trim, and transcode video and audio. KitePlayer is a media player built on KiteFFmpeg. Its core is 100% Kotlin, so it plays the same on every platform. It supports subtitles, live streams, and hardware decoding.
<br><br>
</td></tr>
</table>

<table align="right">
<tr><td align="center" width="380">
<br>
<img src="assets/logos/kiteconfig.png" width="72" alt="KiteConfig logo"><br><br>
<b><a href="https://github.com/yuroyami/KiteConfig">KiteConfig</a></b><br><br>
<img src="https://img.shields.io/badge/Gradle%20plugin-7F52FF?style=flat-square" alt="Gradle plugin"> <a href="https://github.com/yuroyami/KiteConfig/stargazers"><img src="https://img.shields.io/github/stars/yuroyami/KiteConfig?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56" alt="stars"></a><br><br>
Set your app name, icon, version, and IDs once, in one Gradle block. Android, iOS, and desktop all read from it, so they never drift apart.
<br><br>
</td></tr>
</table>

<br clear="both">

## Other useful libraries

### Kodecs

The Kodec libraries read and write file formats in pure Kotlin, with the same
code on every platform.

| Library | Purpose |
| :--- | :--- |
| **[ImageKodec](https://github.com/yuroyami/ImageKodec)** | Decode and encode images (PNG, JPEG, GIF, WebP, AVIF, JPEG XL, and more), with a Coil adapter for Compose. |

### More

| Library | Purpose |
| :--- | :--- |
| **[KiteJS](https://github.com/yuroyami/KiteJS)** | Run JavaScript from shared code, with Rhino or QuickJS behind one API. |
| **[KiteCore](https://github.com/yuroyami/KiteCore)** | The small helpers every project rewrites, like `String.format()` and `Dispatchers.IO` in commonMain. |
| **[Kite3D](https://github.com/yuroyami/Kite3D)** | 3D math: vectors, matrices, quaternions, and bounding volumes, with the same API as three.js. |
| **[libmpvKt](https://github.com/yuroyami/libmpvKt)** | The mpv player engine for Android, prebuilt, with a typed Kotlin API. |

## Upcoming Kite libraries

These libraries all exist and build, but I have not tested them enough to trust
them yet. Each one stays private until it proves that it works, and then it
goes public.

| Library | Purpose |
| :--- | :--- |
| **KiteQR** | Scan and create QR codes and barcodes. |
| **ArchiveKodec** | Zip and unzip anywhere, plus TAR, gzip, LZ4, and Snappy. |
| **AudioKodec** | Decode, encode, and tag audio files. |
| **KiteSynth** | A synthesizer: it reads a SoundFont, takes MIDI notes, and turns them into sound. |
| **KiteRT** | Real-time audio output. Your code makes the samples, and KiteRT sends them to the speakers. |
| **KiteMIDI** | Read and write MIDI files, and talk to real instruments over USB and Bluetooth. |
| **KiteTorrent** | Download and seed torrents from shared code: magnet links, encryption, peer discovery. |

## Upcoming apps

These are the apps I am working on now. Each one runs on every platform from a single Kotlin codebase.

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
