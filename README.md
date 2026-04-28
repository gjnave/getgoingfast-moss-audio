# Get Going Fast: MOSS-Audio (Windows)

This repo provides a Windows-first wrapper around the upstream `OpenMOSS/MOSS-Audio` project.

It downloads the upstream code, applies a small UI/UX patch (branding, YouTube input, safer chunking, batch captioning, live logs), installs dependencies, downloads model weights, and runs the app locally.

## Quick Start

1. Run `install-audio-moss-standalone.bat`
2. Run `run-audio-moss-standalone.bat`

The app opens in your browser.

## What Gets Created

- `MOSS-Audio\` is the upstream repo clone plus the patch applied.
- `MOSS-Audio\.venv\` is the Python virtual environment.
- `MOSS-Audio\downloads\` and `MOSS-Audio\ffmpeg\` hold portable runtime files.
- `MOSS-Audio\outputs\` holds optional exported chunk pairs.

## Batch Mode

Batch mode writes `filename.txt` captions next to each input file. If chunk export is enabled, it also writes numbered training-ready pairs like `001.wav` + `001.txt`.
