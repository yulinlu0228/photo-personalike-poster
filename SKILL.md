---
name: photo-personalike-poster
description: Transform an uploaded portrait or landscape photo into either an original pop-punk 2D character-entry poster or a colorful cinematic anime landscape. Use for photo-to-anime posters, portrait character posters, or animated scenic illustrations. Require an uploaded source photo before generation.
---

# Photo Personalike Poster

## Core goal

Turn one uploaded photo into one original, clearly two-dimensional anime image. First classify it as **portrait** (a person is the main subject) or **landscape** (a place is the main subject), then use the matching reference. Default canvas: vertical 4:5.

## Workflow

Internally follow `OBSERVE → PRESERVE → DISTILL → STYLIZE → COMPOSE → CHECK`. Do not expose the analysis. Generate one finished image; make at most one targeted correction when a required constraint fails.

## Must preserve

- Portrait: recognizable identity, age impression, facial structure, hairstyle, gaze, pose, clothing, glasses, masks, and meaningful objects.
- Landscape: the landmark, viewpoint, time/weather, main spatial relationships, and the most informative three to six scene facts.

## Mode rules

- **Portrait — Pop-punk 2D character poster:** use scarlet as the dominant color with ultramarine as a small depth accent, plus black, charcoal, gray, and white. Build an energetic entrance composition with broken diagonal panels, torn edges, thick black dividers, halftone, offset repeats, and black/red wedges. Optional original props, masks, companion animals, flowers, silhouettes, short English text, and fictional UI may support the subject without replacing them.
- **Landscape — Cinematic anime scene:** use a scene-appropriate, harmonious multicolor palette. Render clear animated linework, cel-shaded forms, layered foreground/midground/background, atmospheric light, and a strong visual focal point. Do not force the portrait palette onto sky, water, foliage, or architecture.

## Style-inspiration boundary

Use game-cutscene landscapes only as high-level inspiration for saturated color, cinematic light, depth, and a single emotional focal point. Use rebellious pop-art posters only as high-level inspiration for torn collage energy and graphic contrast. Create an original scene and composition every time; never reproduce a game screenshot, its UI, its characters, its text, its framing, or a specific work's visual signature.

## Main prohibitions

Do not imitate a named game, character, artist, poster, UI, or screenshot. Do not retain logos, brands, signage, watermarks, or copyrighted character designs. Do not make portraits photorealistic, change a person's identity, or add real people not in the source. Never add readable text unless the portrait workflow calls for original short English copy or the user supplies an exact title.

## References

- Read [Chinese production rules](references/photo-personalike-poster-prompt.zh-CN.md) for Chinese requests.
- Read [English production rules](references/photo-personalike-poster-prompt.en.md) for English requests.

## Examples

`assets/examples/` contains user-provided source photos and approved original outputs. Use them only to understand the two modes' visual boundaries; never copy a depicted person, place, pose, object arrangement, text, or composition.
