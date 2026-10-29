# Export Guide

## What the studio can export

- **PNG frame:** a single frame of the current canvas. When transparent background is enabled, the canvas is exported with alpha transparency.
- **WebM recording:** a browser-recorded canvas clip, when `MediaRecorder` and `canvas.captureStream()` are supported.

The recording control captures the live preview for the selected loop duration. Browser timing, capture support, and codec availability vary. The resulting WebM is a useful working asset, not a guarantee of a perfectly seamless or production-mastered file.

## Recommended workflow

1. Open `index.html` in a current version of Chrome, Edge, or Firefox where available.
2. Pick the final aspect ratio before recording.
3. Start with a low particle count on older computers, then increase it if playback stays smooth.
4. Enable transparency if you intend to composite the particles over other footage.
5. Record the selected loop duration or export a still PNG.
6. Import the result into your video editor.
7. If your editor supports it, render a fixed frame rate (commonly 30 fps) and inspect the join between the final and first frames.
8. If there is a visible seam, trim to a matching frame boundary, crossfade a very short section, or use the editor's loop/optical-flow tools carefully.
9. Export a final master at the dimensions and frame rate required by your destination platform.

## Suggested output targets

| Destination | Canvas | Common timeline target |
|---|---|---|
| YouTube standard video | 1920 × 1080 (16:9) | 30 or 60 fps |
| YouTube Shorts / Reels | 1080 × 1920 (9:16) | 30 or 60 fps |
| Square social post | 1080 × 1080 (1:1) | 30 fps |
| Portrait social post | 1080 × 1350 (4:5) | 30 fps |
| Cinematic widescreen | 2560 × 1080 or project-native (21:9) | Match the project |

These are practical project targets, not platform guarantees; check the latest requirements for your destination.

## Transparent video caveat

WebM transparency support depends on browser, codec, and editor. Do not assume the recorded WebM retains alpha merely because the canvas background is transparent. Verify it in your editor. If alpha is missing, use PNG sequences or a video editor workflow that explicitly supports alpha export.

## Older Windows PCs

On a Windows 7 32-bit computer with limited RAM:
- Start with Preview / 960px and density 40–80.
- Close other browser tabs and apps during recording.
- Prefer short test recordings before trying a full-length export.
- If recording is unsupported or unstable, use the preview as a guide and create the final render in a compatible editor.
- Higher resolution and high particle counts may be slow or unavailable due to browser and memory limits.

## Troubleshooting

**The record button says unsupported:** browser APIs or codecs are missing. Try a browser version supported by your operating system, or use a video editor to capture/render the preview.

**Exported clip is black or empty:** check that the browser allows canvas capture and that the page is running normally. Retry with a lower render size.

**The clip does not loop cleanly:** browser capture timestamps can vary, and a periodic animation does not guarantee identical encoded first/last frames. Inspect and trim in the editor.

**The overlay has a solid background:** confirm transparent mode is enabled, then verify that the recording codec preserves alpha. PNG frame export is the safer transparency test.

**The PC slows down:** reduce density, render size, and glow; turn off particle connections and close unused tabs.
