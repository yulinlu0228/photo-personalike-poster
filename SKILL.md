---
name: photo-personalike-poster
description: Transform an uploaded human, pet, animal, object, mixed subject-and-place, or landscape photo into either an original rebellious pop-punk 2D subject poster or a colorful cinematic illustrated scene. Use for identity-preserving portrait and pet posters, stylized object-entry posters, photo-to-illustration landscapes, and photos where a subject and environment both matter. Require an uploaded source photo before generation.
---

# Photo Personalike Poster

## Core goal

Turn one uploaded source photo into one original, clearly two-dimensional finished image. If no photo is attached, ask for one and stop.

Route the image before generation:

- **Subject poster:** a person, group, animal, pet, or object is the main identity-bearing subject.
- **Landscape scene:** the place, atmosphere, or environment is the main subject; people are incidental.
- **Mixed scene:** a subject and place are both important. Follow the user's priority; otherwise use subject-poster treatment and preserve three to five defining scene facts as supporting background.

## Workflow

Internally follow `OBSERVE → ROUTE → PRESERVE → DISTILL → STYLIZE → COMPOSE → CHECK`. Do not expose the analysis. Generate one finished image; make at most one targeted correction when a required constraint fails.

## Must preserve

- Human or group: identity, count, age impression, facial structure, hairstyle, gaze, pose, relative positions, clothing, glasses, masks, and meaningful objects.
- Animal or pet: species/breed impression, facial proportions, ears, muzzle, eye direction, coat colors and markings, tail, pose, collar, and distinctive accessories.
- Object: silhouette, proportions, material cues, functional structure, and identity-bearing details.
- Landscape: landmark geometry, viewpoint, time/weather, spatial relationships, and three to six high-information scene facts.
- Mixed scene: the subject-place relationship as well as the applicable locks above.

## Mode rules

- **Subject — Pop-punk 2D entry poster:** use scarlet as the dominant impact color, ultramarine as a limited depth accent, plus black, charcoal, gray, and cool white. Build youthful motion with fractured diagonal panels, torn edges, thick black dividers, halftone, offset repeats, and directional wedges. Optional original masks, fictional props, flowers, symbolic animals, silhouettes, short English copy, and fictional UI may support the subject without obscuring or replacing it. Do not force human anatomy, clothing, or expressions onto an animal unless the user asks for anthropomorphism.
- **Landscape — Cinematic illustrated scene:** use a scene-appropriate harmonious multicolor palette, clear illustrated linework, simplified value shapes, layered foreground/midground/background, atmospheric light, and one strong visual focus. Do not impose the subject mode's limited palette on sky, water, foliage, light, or architecture.

Honor a user-specified ratio. Otherwise use vertical `4:5` for a subject poster; for a landscape, preserve the source orientation and approximate aspect ratio, using `16:9` only when a new horizontal cinematic crop is needed. Mixed scenes follow the selected mode.

## Style boundary

Use rebellious pop-art posters and cinematic game-cutscene scenery only as high-level inspiration for graphic energy, saturated color, light, depth, and emotional focus. Create an original scene and composition every time. Never reproduce a game screenshot, character, proprietary interface, text, framing, or a particular work's identifiable visual signature.

## Main prohibitions

Do not imitate a named game, character, artist, poster, UI, or screenshot. Do not retain logos, brands, advertisements, watermarks, or copyrighted character designs. Do not change a person's identity or protected traits, replace a pet with a generic animal, alter subject count, or add realistic people absent from the source. Do not invent readable pseudo-text. When text is allowed, use original short English copy in Arial or reproduce the user's exact title once.

## Output

Save the final image in the current project's `images/photo-personalike-poster/` directory with a short descriptive English filename, such as `scarlet-cat.png`, `city-couple.png`, or `river-sunset.png`. Keep only the latest approved version of each formal result.

## References

- Read [Chinese production rules](references/photo-personalike-poster-prompt.zh-CN.md) for Chinese requests.
- Read [English production rules](references/photo-personalike-poster-prompt.en.md) for English requests.

## Examples

`assets/examples/` contains authorized source images and approved original outputs. Use them only to understand visual boundaries: 2D stylization, color logic, hierarchy, shadows, and composition strength. Never copy a depicted identity, place, clothing, pose, prop, text, or exact composition.
