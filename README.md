# Particle Loop Seamless Studio

A lightweight, browser-based toolkit and asset library for creating seamless particle-loop overlays and music-visualizer elements for YouTube, lyric videos, music videos, presentations, and other video platforms.

## Project goals

- Produce clean, professional-looking particle overlays with a seamless loop.
- Keep the interface lightweight for older Windows PCs and browsers.
- Work locally in a browser without a subscription, account, or cloud rendering service.
- Provide reusable transparent overlays and practical export guidance.
- Make visual assets usable in common video editors and compatible with 16:9, 9:16, and 1:1 projects.

## Current contents

- `index.html` — local browser studio with animated particle preview, adjustable parameters, aspect-ratio presets, and loop/export controls.
- `ASSET_LIBRARY.md` — asset categories, recommended settings, and use cases.
- `EXPORT_GUIDE.md` — workflow notes for transparent overlays and seamless-loop video export.

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern browser.
3. Choose a preset, adjust the controls, and preview the loop.
4. Use the built-in export option where supported, or follow `EXPORT_GUIDE.md` for recording/rendering the preview in a video editor.

The studio is designed to be self-contained and does not require a build step.

## Compatibility notes

The interface aims to remain lightweight, but browser capture/export support differs by browser and operating system. Older browsers may not support every export feature. If a feature is unavailable, use the preview and the export guide with a video editor.

## Quality and licensing

This repository is a practical toolkit, not a claim that every output is automatically broadcast-ready. Inspect exported footage for visible loop seams, flicker, compression banding, and readability before publishing. Assets created with the tool can be incorporated into your own projects; third-party logos, music, footage, and fonts remain subject to their respective licenses.

## Roadmap

- Expand the preset library and curated parameter recipes.
- Add more particle families and audio-spectrum layouts.
- Improve cross-browser export fallbacks.
- Document production workflows for common video editors.
