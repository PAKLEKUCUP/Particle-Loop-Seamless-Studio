# Particle Overlay Asset Library

This guide defines reusable visual families and starting settings for the Particle Loop Seamless Studio. Recipes are starting points, not locked presets: adjust them to fit the song, typography, and footage.

## Particle families

| Family | Visual character | Suggested color pairing | Good use |
|---|---|---|---|
| Aurora drift | Smooth, flowing, airy points | Electric blue + mint | Ambient, chill, cinematic intros |
| Stardust field | Fine scattered specks | Silver-white + ice blue | Lyric videos, subtle backgrounds |
| Warm embers | Warm glowing flecks | Amber + orange-red | Rock, acoustic, emotional songs |
| Arctic particles | Cool crisp glints | Ice blue + white | Clean electronic, winter, science visuals |
| Orbital flow | Circular, planet-like movement | Cyan + violet | Futuristic music visuals |
| Minimal dust | Sparse, understated particles | Soft white + muted blue | Text-heavy videos and transitions |

## Production recipes

### 1. Clean lyric-video background
- Aspect ratio: 16:9
- Recipe: Minimal dust
- Density: 40–80
- Speed: 0.25–0.50×
- Particle size: 0.5–1.5
- Glow: 0.10–0.30
- Transparent background: on
- Connections: off

Keep particles away from the central text-safe area where possible. Low contrast behind lyrics improves readability.

### 2. Ambient / relaxation visual
- Aspect ratio: 16:9 or 9:16
- Recipe: Aurora drift
- Density: 70–140
- Speed: 0.20–0.55×
- Particle size: 1–2.5
- Glow: 0.35–0.65
- Trails: on
- Connections: off

Avoid rapid movement and bright flashes. Use long fades in the editor for a calm opening and ending.

### 3. Energetic music overlay
- Aspect ratio: 16:9
- Recipe: Stardust field or Orbital flow
- Density: 130–220
- Speed: 0.65–1.15×
- Particle size: 1.5–3
- Glow: 0.35–0.70
- Connections: optional

The studio motion is periodic for loop-friendly animation, but the rendered recording still needs inspection for frame-rate jitter and the first/last-frame match.

### 4. Warm acoustic / vintage tone
- Aspect ratio: 16:9
- Recipe: Warm embers
- Density: 45–110
- Speed: 0.25–0.65×
- Particle size: 1–2.5
- Glow: 0.20–0.50
- Colors: amber/orange-red

Use sparingly; too many bright particles can compete with faces and lyrics.

### 5. Short-form vertical
- Aspect ratio: 9:16
- Density: 45–100
- Speed: 0.35–0.70×
- Keep important titles and faces near the central safe zone.
- Check the composition on a phone-sized preview before publishing.

## Overlay layering ideas

1. **Base atmosphere:** one low-density, low-glow layer.
2. **Accent particles:** a second layer with fewer, brighter points.
3. **Typography:** keep lyrics or titles above particles.
4. **Optional spectrum:** add a separate audio visualizer in your editor; this project does not claim to analyze audio or generate a true audio-reactive spectrum.
5. **Finish:** use a subtle vignette or color grade in the editor if needed.

## Quality checklist

- [ ] Particle motion looks intentional rather than random noise.
- [ ] Bright particles do not obscure lyrics or faces.
- [ ] No distracting clipping, flicker, or compression banding.
- [ ] The final frame matches the first closely enough for the intended loop.
- [ ] Export resolution and aspect ratio match the video timeline.
- [ ] Audio, fonts, footage, and third-party elements are properly licensed.
