<h1 align="center">Streamyx</h1>

<div align="center">
  <a href="https://github.com/vitalygashkov/streamyx/releases">
    <img src="https://img.shields.io/github/release/vitalygashkov/streamyx.svg?style=flat-square" alt="GitHub release">
  </a>
</div>

Streamyx is a command-line tool that allows you to download videos from streaming services for offline-viewing.

## Installation

### Prerequisites

The following dependencies are required and should be downloaded and placed in this path: `/files/bin/`.

- **[FFmpeg](https://ffmpeg.org/download.html)**
- **[mp4decrypt](https://www.bento4.com/downloads/)**

> **Note**: FFmpeg and mp4decrypt does not affect the download, only affects the final file merge and decryption.

**Device private keys** are required for DRM-protected content and should be placed in this path: `/files/cdm/`

### Install

Download the binary file from [latest release](https://github.com/vitalygashkov/streamyx/releases/latest) and put `/files/` folder with dependencies next to it.

## Getting Started

Open terminal from the folder where the binary file is located and run the application.

Usage:

```
streamyx [OPTIONS] URL
```

Use `-h` option to see all available options.

### Download a video

```console
$ streamyx "https://hd.kinopoisk.ru/film/46c5df252dc1a790b82d1a00fcf44812?content_tab=series&episode=10&season=5&watch="
1/1/2022, 10:00:27 AM  INFO   Fetching metadata and generate download configs...
1/1/2022, 10:00:28 AM  INFO   Rick and Morty • S5:E10 • Rickmurai Jack • Full HD • 1017 MB
1/1/2022, 10:00:28 AM  INFO   █████▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒▒ 9%
```

## Providers

| Title       | URL                            | Status      | Details                                            |
| ----------- | ------------------------------ | ----------- | -------------------------------------------------- |
| Crunchyroll | <https://beta.crunchyroll.com> | Supported   | Classic version is not supported                   |
| Kinopoisk   | <https://hd.kinopoisk.ru>      | Supported   |                                                    |
| Okko        | <https://okko.tv>              | Supported   | 4K support & email auth in progress                |
| IVI         | <https://www.ivi.ru>           | In progress | Auth in progress                                   |
| NTV         | <https://www.ntv.ru>           | In progress | Only download link extracting                      |
| Wakanim     | <https://www.wakanim.tv>       | Deprecated  | No longer maintained due to merge with Crunchyroll |
