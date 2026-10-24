# chrissi's Image Tool

A lightweight, client-side tool for resizing, cropping, converting, and compressing images.

## What it does

Redraws your image on a canvas at the size and format you choose and exports it as a new file. Because the image is redrawn, metadata like EXIF and GPS is dropped automatically.

## Features

- Drag to move and zoom to crop, the frame shows exactly what gets exported
- Presets for Discord stickers, emojis, profile banners and server banners, YouTube thumbnails, and profile pictures, all editable in one config object at the top of the script
- Or no preset: any size up to 4096 px, starting from the image's own size
- Output as PNG, JPG, or WebP, with a quality slider for JPG and WebP
- Live file size next to the preset's limit, so you know before you download

## How it works

Everything runs in the browser. Images are never uploaded to a server or processed anywhere else.

## Preset sources

- [Discord sticker](https://support.discord.com/hc/en-us/articles/4402687377815-Tips-for-Sticker-Creators-FAQ): PNG, exactly 320 x 320, max 512 KB
- [Discord emoji](https://support.discord.com/hc/en-us/articles/360041139231-How-to-Add-Emojis-on-Discord): up to 128 x 128, under 256 KB
- [Discord profile banner](https://support.discord.com/hc/en-us/articles/4403147417623-Custom-Profiles): PNG or JPG, at least 680 x 240, under 10 MB
- [Discord server banner](https://support.discord.com/hc/en-us/articles/360028716472-Server-Banners): 16:9, at least 960 x 540
- [YouTube thumbnail](https://support.google.com/youtube/answer/72431): 16:9, at least 640 px wide, JPG or PNG, max 2 MB on mobile
- Profile picture: not an official limit, just a sensible default

## Design

Font: Crimson Pro (SIL Open Font License), weight 500, 18px text and 1.25em heading.

Design tokens, peach theme. Light and dark follow the system.

| Token | Light | Dark |
| --- | --- | --- |
| background | `#fff6f0` | `#171009` |
| accent | `#2b170d` | `#fdebdd` |
| body | `#5c3f2e` | `#cdb3a2` |
| sub | `#785a48` | `#ab9282` |
| highlight | `#fde5d5` | `#35231a` |
