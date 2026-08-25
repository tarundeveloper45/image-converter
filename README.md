# Media Converter

A fast, private, in-browser image and video converter. Everything runs client-side — no files are ever uploaded anywhere.

## Image

Convert between **JPG**, **PNG**, and **WebP** using the Canvas API, with a live before/after comparison, quality control, and instant download.

- Drag & drop or click to upload an image
- Before/after split-view comparison with a draggable divider
- Convert to JPEG, PNG, or WebP
- Quality slider for lossy formats
- Live file size and percentage savings
- Zoom controls
- One-click download

## Video

Compress video using [ffmpeg.wasm](https://github.com/ffmpegwasm/ffmpeg.wasm) (FFmpeg compiled to WebAssembly), running entirely in the browser.

- Drag & drop or click to upload a video
- Output as MP4 (H.264) or WebM (VP8)
- Resolution presets (1080p / 720p / 480p / 360p) or original
- Compression slider
- Original vs. compressed preview toggle
- Live file size and percentage savings

The compression engine (~25 MB) downloads on first use and is cached by the browser afterward. Best with clips under a couple of minutes since encoding is single-threaded.

## Run locally

No build step required — it's a single static HTML file.

```bash
npx serve . -l 5540
```

Then open `http://localhost:5540`.
