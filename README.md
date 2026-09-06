# 🎬 OTT & Broadcast Streaming Tools

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

A curated list of open-source and free tools for Broadcast, OTT Video Streaming, and Ad Insertion. This repository aims to be a comprehensive resource for developers, broadcast engineers, and streaming professionals looking for high-quality tools across the entire video delivery pipeline.

## 📋 Table of Contents

- [Why This List?](#why-this-list)
- [Stage Breakdown](#stage-breakdown)
- [1. Content Ingestion & Production](#1-content-ingestion--production)
- [2. Transcoding & Processing](#2-transcoding--processing)
- [3. Packaging & Origin](#3-packaging--origin)
- [4. Delivery & Distribution](#4-delivery--distribution)
- [5. Ad Insertion](#5-ad-insertion)
- [6. Player & Client-Side SDKs](#6-player--client-side-sdks)
- [7. Supplementary & Testing Tools](#7-supplementary--testing-tools)
- [Existing Comprehensive Resources](#existing-comprehensive-resources)
- [How to Contribute](#how-to-contribute)
- [License](#license)

## 🎯 Why This List?

The video streaming ecosystem is complex, with tools spanning multiple stages from content creation to final delivery. This list helps you:

- **Find the right tool** for each stage of your pipeline
- **Discover alternatives** to commercial solutions
- **Save time** by leveraging community-maintained resources
- **Contribute back** by adding tools you've found useful

## 🗺️ Stage Breakdown

The streaming workflow is divided into logical stages, making it easier to identify tools for specific needs:

1. **Content Ingestion & Production** - Capture, create, and switch live video sources
2. **Transcoding & Processing** - Convert and optimize video formats and bitrates
3. **Packaging & Origin** - Prepare and store content for streaming delivery
4. **Delivery & Distribution** - Scale and deliver streams globally
5. **Ad Insertion** - Insert targeted advertisements into streams
6. **Player & Client-Side SDKs** - Play and display content on various devices
7. **Supplementary & Testing Tools** - Support, test, and monitor your pipeline

## 🎥 1. Content Ingestion & Production

Tools for video capture, live production switching, graphics, and broadcast playout.

| Tool                                                                  | Description                                                       | License         | Key Features                                             |
| --------------------------------------------------------------------- | ----------------------------------------------------------------- | --------------- | -------------------------------------------------------- |
| [OBS Studio](https://obsproject.com/)                                 | Industry-standard software for video recording and live streaming | GPLv2           | Real-time scene composition, encoding, broadcasting      |
| [CasparCG](https://www.casparcg.com/)                                 | Professional graphics and video playout software                  | GPLv3           | 24/7 broadcast operation, graphics, audio, video playout |
| [Voctomix](https://github.com/ebu/voctomix)                           | Full-HD software live-video mixer                                 | MIT             | Python/GStreamer based, multi-source mixing              |
| [Flowblade](https://jliljebl.github.io/flowblade/)                    | Multitrack non-linear video editor                                | GPLv3           | Professional-grade editing                               |
| [Snowmix](https://sourceforge.net/projects/snowmix/)                  | Live video mixer                                                  | GPLv3           | Flexible mixing capabilities                             |
| [vMix](https://www.vmix.com/)                                         | Software vision mixer (Free version available)                    | Commercial/Free | Professional production features                         |
| [NDI Tools](https://www.ndi.tv/tools/)                                | Network Device Interface management suite                         | Free            | Discovery and management of NDI sources                  |
| [Icecast2](https://icecast.org/) / [Ices2](https://icecast.org/ices/) | Streaming media server and source                                 | GPLv2           | Audio streaming, Ogg Vorbis support                      |

## ⚙️ 2. Transcoding & Processing

Tools for converting, scaling, and optimizing video for different delivery formats.

| Tool                                                                     | Description                                    | License     | Key Features                                                      |
| ------------------------------------------------------------------------ | ---------------------------------------------- | ----------- | ----------------------------------------------------------------- |
| [FFmpeg](https://ffmpeg.org/)                                            | Foundational multimedia framework              | LGPL/GPL    | Convert, record, stream; the Swiss Army knife of video processing |
| [GStreamer](https://gstreamer.freedesktop.org/)                          | Library for constructing media-handling graphs | LGPL        | Framework for streaming media pipelines                           |
| [Membrane Framework](https://github.com/membraneframework/membrane-core) | Multimedia processing framework                | Apache 2.0  | Elixir-based, RTP, HLS, MP4, various codecs                       |
| [Boombox](https://github.com/membraneframework/boombox)                  | Streaming tool built on Membrane Framework     | Apache 2.0  | Easy transformations between media formats and protocols          |
| [AvTranscoder](https://github.com/avTranscoder/avTranscoder)             | High-level API for FFmpeg/LibAV                | LGPL        | Re-wrapping and transcoding                                       |
| [LibAV](http://libav.org/)                                               | Audio and video processing tools               | LGPL        | Alternative to FFmpeg                                             |
| [Restreamer](https://restreamer.io/)                                     | Self-hosted live video broadcast platform      | Open Source | Web UI, configurable codecs, stream routing                       |
| [Monibuca](https://github.com/langhuihui/monibuca)                       | Modular streaming server framework             | MIT         | Go-based, extensible                                              |

## 📦 3. Packaging & Origin

Tools for packaging content into streaming formats (HLS, DASH) and storing on origin servers.

| Tool                                                        | Description                            | License      | Key Features                   |
| ----------------------------------------------------------- | -------------------------------------- | ------------ | ------------------------------ |
| [Bento4](https://www.bento4.com/)                           | MP4 format and MPEG-DASH C++ library   | Apache 2.0   | Full-featured MP4 tools        |
| [GPAC](https://gpac.wp.imt.fr/)                             | Multimedia player and packager         | LGPL         | MP4 and DASH packaging         |
| [MP4Box.js](https://github.com/gpac/mp4box.js)              | JavaScript MP4 processing library      | BSD-3-Clause | Browser and Node.js compatible |
| [Codem-isoboxer](https://github.com/mozilla/codem-isoboxer) | Browser-based ISOBMFF parser           | BSD-2-Clause | Small, efficient MP4 parsing   |
| [L-SMASH](https://github.com/l-smash/l-smash)               | Rigidly spec-compliant ISOBMFF library | ISC          | Full DASH muxing support       |
| [mpegts.js](https://github.com/xqq/mpegts.js)               | HTML5 MPEG2-TS/FLV stream player       | MIT          | Browser-based playback         |

## 🌐 4. Delivery & Distribution

Infrastructure for scaling and delivering streams to global audiences.

| Tool                                                                      | Description                           | License    | Key Features                               |
| ------------------------------------------------------------------------- | ------------------------------------- | ---------- | ------------------------------------------ |
| [MistServer](https://mistserver.org/)                                     | Full-featured streaming media toolkit | GPLv3      | OTT delivery, developer-friendly           |
| [Aliran](https://github.com/aliran-org/aliran)                            | Peer-to-peer OTT streaming solution   | MIT        | Self-hostable, viewers re-seed channels    |
| [Owncast](https://owncast.online/)                                        | Self-hosted live streaming server     | MIT        | Full control, HLS delivery, built-in chat  |
| [Wowza Streaming Engine](https://www.wowza.com/products/streaming-engine) | Commercial streaming server           | Commercial | Ingest, process, deliver at scale          |
| [ZLMediaKit](https://github.com/ZLMediaKit/ZLMediaKit)                    | High-concurrency streaming engine     | MIT        | Media server, protocol gateway             |
| [PeerTube](https://joinpeertube.org/)                                     | Decentralized video hosting platform  | AGPLv3     | ActivityPub federation, content management |

## 📡 5. Ad Insertion

Tools for replacing or overlaying advertisements into video streams.

| Tool                                                             | Description                      | License    | Key Features                                        |
| ---------------------------------------------------------------- | -------------------------------- | ---------- | --------------------------------------------------- |
| [Ritcher](https://github.com/Eyevinn/ritcher)                    | HLS & DASH stitcher              | MIT        | Rust-based, SSAI and SGAI support, VAST integration |
| [sgai-ad-proxy](https://github.com/Eyevinn/sgai-ad-proxy)        | Server-Guided Ad Insertion proxy | MIT        | Experimental HTTP proxy for dynamic ad insertion    |
| [AWS Elemental MediaTailor](https://aws.amazon.com/mediatailor/) | Managed ad-insertion service     | Commercial | Server-side ad insertion, personalization           |

## 📺 6. Player & Client-Side SDKs

Applications and SDKs for content playback across various devices.

| Tool                                                         | Description                       | License      | Key Features                                   |
| ------------------------------------------------------------ | --------------------------------- | ------------ | ---------------------------------------------- |
| [VLC Media Player](https://www.videolan.org/vlc/)            | Popular open-source media player  | GPLv2        | Cross-platform, handles streaming playback     |
| [Dash.js](https://github.com/Dash-Industry-Forum/dash.js)    | MPEG-DASH reference client        | BSD-3-Clause | JavaScript implementation for browser playback |
| [MoonTV](https://github.com/moontv-app/moontv)               | Web-based movie and TV aggregator | MIT          | Next.js, HLS.js, VidStack integration          |
| [Kodi](https://kodi.tv/)                                     | Media center application          | GPLv2        | Inputstream addons for adaptive, RTMP playback |
| [HbbPlayer](https://github.com/Orange-OpenSource/hbb-player) | Open-source HbbTV application     | Apache 2.0   | URL-based media playback on connected TVs      |
| [VideoContext](https://github.com/bbc/videocontext)          | HTML5/WebGL video library         | Apache 2.0   | Interactive and responsive web videos          |
| [hls.js](https://github.com/video-dev/hls.js)                | HLS playback in JavaScript        | Apache 2.0   | Browser-based HLS client                       |

## 🧪 7. Supplementary & Testing Tools

Tools for automation, quality assessment, and network testing.

| Category                 | Tool                                                                       | Description                           | License    |
| ------------------------ | -------------------------------------------------------------------------- | ------------------------------------- | ---------- |
| **Broadcast Automation** | [Sofie TV Studio Automation System](https://github.com/nrkno/sofie-core)   | Live TV news production automation    | MIT        |
| **Quality Assessment**   | [VMAF](https://github.com/Netflix/vmaf)                                    | Perceptual video quality assessment   | BSD+Patent |
| **Quality Assessment**   | [Wisual](https://github.com/SamyKaci/wisual)                               | Visual Quality Assessment web service | MIT        |
| **Network Testing**      | [SMPTE 2110-20 Analyzer](https://github.com/Eyevinn/smpte2110-20-analyzer) | Inspect SMPTE ST 2110 network packets | MIT        |
| **Network Testing**      | [iPerf3](https://iperf.fr/)                                                | Network bandwidth measurement         | BSD        |

## 📚 Existing Comprehensive Resources

These curated lists are fantastic resources that complement this repository:

- **[`ebu/awesome-broadcasting`](https://github.com/ebu/awesome-broadcasting)** - The most comprehensive list of open-source broadcast technologies curated by the EBU.
- **[`awesome-streaming-tools`](https://github.com/steveseguin/awesome-streaming-tools)** - Curated list of streaming video tools, frameworks, and libraries.
- **[`awesome-ffmpeg`](https://github.com/transitive-bullshit/awesome-ffmpeg)** - Curated list of amazing FFmpeg resources.
- **[`streaming-papers`](https://github.com/steveseguin/streaming-papers)** - A collection of research papers on streaming media.

# 