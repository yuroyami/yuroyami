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
| **[KitePDF](https://github.com/yuroyami/KitePDF)** | **TL;DR:** Pure-Kotlin PDF and EPUB engine, read and write.<br>**What it does:** Ships its own PDF stack: parser, content-stream interpreter, font engine, filters, encryption, writer and editor. The same core reads reflowable EPUB 2 and 3. Drawing is opt-in: an optional Compose Multiplatform viewer, plus Skia and native-canvas renderers if you are not on Compose. | [![kitepdf](https://img.shields.io/maven-central/v/io.github.yuroyami/kitepdf?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kitepdf) | [![stars](https://img.shields.io/github/stars/yuroyami/KitePDF?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KitePDF/stargazers) |
| **[KiteCodec](https://github.com/yuroyami/KiteCodec)** | **TL;DR:** FFmpeg for Kotlin Multiplatform, with no `ffmpeg` process to launch.<br>**What it does:** Binds FFmpeg's libav* through cinterop on native targets, and through a bundled JNI adapter on JVM and Android. One call runs demux, decode, filter, encode and mux in a single pass, video and audio together, without memory growing with the length of the input. A Gradle plugin fetches the prebuilt binaries. Frames arrive as a `Flow`, progress as a typed callback. | ![source only](https://img.shields.io/badge/source%20only-8a8f98?style=flat-square) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteCodec?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteCodec/stargazers) |
| **[KitePlayer](https://github.com/yuroyami/KitePlayer)** | **TL;DR:** A media player written in Kotlin from scratch, not a wrapper.<br>**What it does:** The playback engine, demux pump, decoders and A/V sync all live in `commonMain`, so it behaves the same everywhere. It does not wrap ExoPlayer, AVPlayer or libmpv. FFmpeg through KiteCodec is the portable backend, while Android can drive MediaCodec straight into its renderer. Only the audio device, video surface and decoder are platform-specific. | ![source only](https://img.shields.io/badge/source%20only-8a8f98?style=flat-square) | ![stars](https://img.shields.io/badge/%E2%98%85%200-444c56?style=flat-square) |
| **[KiteCore](https://github.com/yuroyami/KiteCore)** | **TL;DR:** The `commonMain` utilities every KMP project ends up rewriting.<br>**What it does:** Fills the five gaps KMP leaves: an IO dispatcher that resolves on every target, weak references, host-platform identification, and a `Deferred` that reports progress while it runs. Adds around 450 helpers for text, collections, flows, coroutines, math, encoding, time and randomness. One artifact, and `kotlinx-coroutines-core` is its only dependency. | [![kitecore](https://img.shields.io/maven-central/v/io.github.yuroyami/kitecore?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kitecore) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteCore?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteCore/stargazers) |
| **[KiteQR](https://github.com/yuroyami/KiteQR)** | **TL;DR:** Barcodes on every target, using ZXing's API.<br>**What it does:** Reads and writes QR, Aztec, Data Matrix, PDF417 and the 1D families, then renders the result to SVG or PNG. No `expect`/`actual`, no `java.*` imports, and nothing on the classpath but `kotlin-stdlib`. Shift_JIS, GB18030 and Big5 character tables ship inside the library, so they work everywhere. Optional Compose Multiplatform module. | [![kiteqr](https://img.shields.io/maven-central/v/io.github.yuroyami/kiteqr?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kiteqr) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteQR?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteQR/stargazers) |
| **[KiteImage](https://github.com/yuroyami/KiteImage)** | **TL;DR:** Image decoding in common Kotlin, without the platform bitmap APIs.<br>**What it does:** Decodes PNG, JPEG, GIF, BMP, TIFF, JPEG 2000 and lossless WebP from a `ByteArray`, and normalizes every format to non-premultiplied ARGB_8888 in a plain `IntArray`. Resolves palettes, grayscale, BGR ordering and chroma subsampling for you. GIF, APNG and animated WebP arrive fully composited. Optional Compose and Coil modules. | [![kiteimage](https://img.shields.io/maven-central/v/io.github.yuroyami/kiteimage?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kiteimage) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteImage?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteImage/stargazers) |
| **[KiteArchive](https://github.com/yuroyami/KiteArchive)** | **TL;DR:** `java.util.zip`, but for every KMP target.<br>**What it does:** Implements the formats in `commonMain`, so there is no JNI, no cinterop and no native binary. ZIP read and write including ZIP64, readers for TAR, ar and cpio, DEFLATE, gzip, zlib, LZ4 and Snappy codecs, and CRC-32, CRC-32C, Adler-32, CRC-64/XZ and xxHash32 checksums. The API is whole-array: pass a `ByteArray`, get one back. | [![kitearchive](https://img.shields.io/maven-central/v/io.github.yuroyami/kitearchive?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kitearchive) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteArchive?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteArchive/stargazers) |
| **[Kite3D](https://github.com/yuroyami/Kite3D)** | **TL;DR:** three.js maths, minus the renderer.<br>**What it does:** 29 maths types in common Kotlin: vectors, matrices, quaternions, Euler angles, boxes, spheres, planes, rays, frustums, color and interpolants, with the same API as three.js. It draws nothing. No scene graph, no camera, no materials, no GPU backend. Use it for the maths, not as an engine. | [![kite3d](https://img.shields.io/maven-central/v/io.github.yuroyami/kite3d?style=flat-square&label=&color=7F52FF)](https://central.sonatype.com/artifact/io.github.yuroyami/kite3d) | [![stars](https://img.shields.io/github/stars/yuroyami/Kite3D?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/Kite3D/stargazers) |

### Upcoming

Still being built. The source is public, but there is nothing to depend on yet.

| Library | Purpose |
| :--- | :--- |
| **[KiteAudio](https://github.com/yuroyami/KiteAudio)** | **TL;DR:** Audio codecs, containers and tags in pure Kotlin.<br>**What it does:** Reads and writes FLAC, WAV, AIFF and AU. Decodes FLAC, Vorbis, every MPEG audio layer and the uncompressed family to Float32 PCM. Edits ID3, APE, Vorbis comments and the RIFF, AIFF and Ogg metadata chunks without re-encoding the audio.
| **[KiteTorrent](https://github.com/yuroyami/KiteTorrent)** | **TL;DR:** libtorrent 2.0.12, reimplemented in Kotlin.<br>**What it does:** Downloads and seeds from shared code, with magnet links, a DHT node, µTP, encryption and proxies. No JNI, no cinterop, no bundled binary. Two artifacts: one of pure computation (bencoding, parsing, wire codec, piece picker), and one live session that owns the sockets, disk and trackers.

## 🔌 Gradle plugin

| Plugin | Purpose | Release | Stars |
| :--- | :--- | :--- | :--- |
| **[KiteSSOT](https://github.com/yuroyami/KiteSSOT)** | **TL;DR:** One place to declare app identity for a whole KMP repo.<br>**What it does:** App name, version, bundle ID, locales, Android SDK levels and Java level normally live in four places: Android `defaultConfig`, Xcode build settings, `Info.plist`, and a Kotlin constant. They drift. KiteSSOT declares them once in the root build and propagates them. Gradle config is applied on every build; edits to files you own (`project.pbxproj`, `Info.plist`, `Podfile`, icons) only run from explicitly named tasks. | [![kitessot](https://img.shields.io/gradle-plugin-portal/v/io.github.yuroyami.kitessot?style=flat-square&label=&color=02303A)](https://plugins.gradle.org/plugin/io.github.yuroyami.kitessot) | [![stars](https://img.shields.io/github/stars/yuroyami/KiteSSOT?style=flat-square&label=%E2%98%85&labelColor=444c56&color=444c56)](https://github.com/yuroyami/KiteSSOT/stargazers) |

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
