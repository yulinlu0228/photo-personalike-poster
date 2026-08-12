---
name: photo-personalike-poster
description: Transform an uploaded human, pet, animal, object, mixed subject-and-place, or landscape photo into either an original high-energy rebellious pop-punk 2D subject poster or a colorful cinematic illustrated scene. Use for identity-preserving portrait and pet posters, stylized object-entry posters, photo-to-illustration landscapes, and photos where a subject and environment both matter. Require an uploaded source photo before generation.
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

- Human or group: always lock identity, count, age impression, facial structure, hairstyle, gaze, protected traits, body proportions, glasses, and identity-bearing objects. Preserve pose, relative positions, and clothing only when the user requests it or when they carry identity, occupation, cultural, accessibility, safety, or interaction meaning; otherwise they may be redesigned for energy and an original masked-action costume.
- Animal or pet: species/breed impression, facial proportions, ears, muzzle, eye direction, coat colors and markings, tail, pose, collar, and distinctive accessories.
- Object: silhouette, proportions, material cues, functional structure, and identity-bearing details.
- Landscape: landmark geometry, viewpoint, time/weather, spatial relationships, and three to six high-information scene facts.
- Mixed scene: the subject-place relationship as well as the applicable locks above.

## Mode rules

- **Subject — High-energy pop-punk 2D entry poster:** make the result theatrical, youthful, and immediately kinetic rather than merely decorative. If the source pose is static and the user did not require pose preservation, redesign it into a plausible action pose while preserving identity and body proportions. Daily clothing may become an original masked-action costume using abstract elements such as a fitted high collar, asymmetric tailored coat, cropped cape or long split tails, gloves, boots, harness seams, layered lapels, or an original eye mask; preserve required cultural, occupational, accessibility, and safety items. Never copy an existing character's costume or mask. Establish one dominant motion axis; use foreshortening, asymmetric weight, repeated silhouettes, fractured panels, halftone, and counter-directional shapes. Default to a scarlet/black/white anchor with two or three coordinated supporting hues. Preserve recognizable skin hue and value in hard-edged cel tones. Use three to seven coherent supporting motifs without obscuring identity anchors. Do not force human anatomy or costume onto an animal unless the user asks for anthropomorphism.
- **Landscape — Cinematic illustrated scene:** use a scene-appropriate harmonious multicolor palette, clear illustrated linework, simplified value shapes, layered foreground/midground/background, atmospheric light, and one strong visual focus. Do not impose the subject mode's limited palette on sky, water, foliage, light, or architecture.

Honor a user-specified ratio. Otherwise choose subject-poster ratio by composition: use horizontal `16:9` for sweeping action, full-body movement, prop direction, ensemble spacing, or a wide decorative stage; use vertical `4:5` for a dominant single figure, upward motion, or fashion-like entrance; preserve another source ratio when it serves the design better. For landscapes, preserve source orientation and approximate ratio, using `16:9` when a new horizontal cinematic crop is needed. Mixed scenes follow the selected mode.

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

`assets/examples/` contains authorized source images and approved original outputs. Use them only to understand visual boundaries: 2D stylization, color logic, hierarchy, shadows, widescreen action redesign, and original masked-action costume transformation. Treat every example as one possibility rather than a template; the written routing and high-tension rules take priority. Never copy a depicted identity, place, clothing, pose, costume, mask, prop, text, or exact composition.
