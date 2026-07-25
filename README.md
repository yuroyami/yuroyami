<!-- ══════════════════════  HEADER  ══════════════════════ -->

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="assets/hero-dark.svg">
  <img width="100%" src="assets/hero-light.svg" alt="yuroyami. Kotlin for everything.">
</picture>

<div align="center">

<img src="assets/taglines.svg" width="100%" alt="Kite: PDFs, barcodes, images, archives, torrents and 3D maths in pure Kotlin" />

</div>

<!-- ══════════════════════  INTRO  ══════════════════════ -->

I write Kotlin Multiplatform libraries the ecosystem does not have yet, and apps
that use them. Almost all of it is pure `commonMain` Kotlin: no JNI, no native
binary.

<!-- ══════════════════════  KITE  ══════════════════════ -->

## 🪁 &nbsp;Kite

| Library | What it does | Targets | Latest | Docs |
| :--- | :--- | :---: | :--- | :---: |
| **[KitePDF](https://github.com/yuroyami/KitePDF)** | Read, create, edit and render PDFs. Also reads EPUB 2 and 3. | 22 | [![kitepdf](https://img.shields.io/maven-central/v/io.github.yuroyami/kitepdf?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kitepdf) | [Guide](https://yuroyami.github.io/KitePDF/) |
| **[KiteQR](https://github.com/yuroyami/KiteQR)** | Scan and generate QR, Aztec, Data Matrix, PDF417 and the 1D barcode families. | 22 | [![kiteqr](https://img.shields.io/maven-central/v/io.github.yuroyami/kiteqr?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kiteqr) | [Guide](https://yuroyami.github.io/KiteQR/) |
| **[KiteImage](https://github.com/yuroyami/KiteImage)** | Decode and encode PNG, JPEG, GIF, BMP, TIFF, JPEG 2000 and lossless WebP. | 22 | [![kiteimage](https://img.shields.io/maven-central/v/io.github.yuroyami/kiteimage?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kiteimage) | [Guide](https://yuroyami.github.io/KiteImage/) |
| **[Kite3D](https://github.com/yuroyami/Kite3D)** | Vectors, matrices, quaternions, bounding volumes and colour. Maths only. | 22 | [![kite3d](https://img.shields.io/maven-central/v/io.github.yuroyami/kite3d?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kite3d) | [Guide](https://yuroyami.github.io/Kite3D/) |
| **[KiteCore](https://github.com/yuroyami/KiteCore)** | The small things `commonMain` leaves out: an IO dispatcher, weak references, platform identity. | 8 | [![kitecore](https://img.shields.io/maven-central/v/io.github.yuroyami/kitecore?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kitecore) | [Guide](https://yuroyami.github.io/KiteCore/) |
| **[KiteArchive](https://github.com/yuroyami/KiteArchive)** | DEFLATE, gzip, zlib and LZ4. Reads and writes ZIP and ZIP64, reads TAR, ar and cpio. | 6 | [![kitearchive](https://img.shields.io/maven-central/v/io.github.yuroyami/kitearchive?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kitearchive) | [Guide](https://yuroyami.github.io/KiteArchive/) |
| **[KiteSSOT](https://github.com/yuroyami/KiteSSOT)** | Gradle plugin. Declare app name, version and bundle ID once, then it writes the Android and iOS copies. | Gradle | [![kitessot](https://img.shields.io/gradle-plugin-portal/v/io.github.yuroyami.kitessot?style=flat-square&label=&color=02303A)](https://plugins.gradle.org/plugin/io.github.yuroyami.kitessot) | [Guide](https://yuroyami.github.io/KiteSSOT/) |
| **[KiteTorrent](https://github.com/yuroyami/KiteTorrent)** | Download and seed torrents. DHT, µTP, magnet links, encryption and BitTorrent v2. | 5 | ![source only](https://img.shields.io/badge/source%20only-8a8f98?style=flat-square) | [Guide](https://yuroyami.github.io/KiteTorrent/) |
| **[KiteCodec](https://github.com/yuroyami/KiteCodec)** | Demux, decode, filter, encode and mux video and audio through FFmpeg. | Native | ![source only](https://img.shields.io/badge/source%20only-8a8f98?style=flat-square) | [docs/](https://github.com/yuroyami/KiteCodec/tree/main/docs) |

<!-- ══════════════════════  APPS  ══════════════════════ -->

## 📲 &nbsp;Apps

One Kotlin codebase, Android and iOS, Compose Multiplatform throughout.

| App | What it is | |
| :--- | :--- | :--- |
| **[Syncplay Mobile](https://github.com/yuroyami/syncplay-mobile)** | Watch video in sync with friends. Works with Syncplay on desktop. | [![stars](https://img.shields.io/github/stars/yuroyami/syncplay-mobile?style=flat-square&label=&color=7F52FF)](https://github.com/yuroyami/syncplay-mobile) |
| **[Pingy](https://github.com/yuroyami/PINGY)** | Network ping and latency tester. | <img src="https://img.shields.io/badge/Android%20%C2%B7%20iOS-3DDC84?style=flat-square" alt="Android and iOS"> |
| **[DuelistLP](https://github.com/yuroyami/DuelistLP)** | Life point counter for two-player Yu-Gi-Oh. | <img src="https://img.shields.io/badge/Android%20%C2%B7%20iOS-3DDC84?style=flat-square" alt="Android and iOS"> |

Peerora (file transfer) and Luddy (torrent and HTTP downloader, built on
KiteTorrent) are not public yet.

<!-- ══════════════════════  CONTACT  ══════════════════════ -->

<div align="center">

<br>

<a href="mailto:evongintoki@gmail.com"><img src="https://img.shields.io/badge/Email-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Email"></a>

</div>

<img width="100%" src="assets/footer.svg" alt="">
