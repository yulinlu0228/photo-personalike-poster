# Photo Personalike Poster: Full Image-Generation Specification

## General execution

First classify the uploaded photo as a **portrait** or a **landscape**. Generate one vertical 4:5 finished image by default; honor a user-specified ratio. Internally perform `OBSERVE → PRESERVE → DISTILL → STYLIZE → COMPOSE → CHECK` without exposing the intermediate analysis.

Extract high-information content from the photo and remove photographic noise, low-information clutter, and recognizable brands. The result must read first as two-dimensional animation or cel-shaded illustration, never as a photo filter, semi-realistic game key art, or a 3D render.

## Style-inspiration boundary

Use an original rebellious pop-art 2D poster language for portraits, aiming for youthful motion, torn-collage energy, and high-contrast graphic relationships. Draw landscape inspiration from common game-cutscene qualities: saturated multicolor, cinematic light, layered space, and one emotional focal point. Both modes borrow only abstract methods. Never reproduce a game screenshot, character, interface, text, camera crop, composition, accessory, logo, or the identifiable visual signature of a particular work.

## Portrait mode: original pop-punk 2D poster

### Identity lock

Preserve recognizable identity and age impression: basic face shape, hairline and hairstyle, eye direction, expression, head tilt, body pose, arm-crossing relationship, clothing type, glasses/goggles/masks, and identity-bearing objects. Anime simplification is allowed, but do not beautify, de-age, gender-swap, change ethnic traits, add muscle, or rewrite body proportions.

### Visual grammar

- The image must be unambiguously 2D animation: complete black outer contours with clear line-weight variation, blocky anime hair, simplified but identity-preserving features, hard-edged cel shadows, and two to three value blocks per surface.
- Use scarlet as the dominant color. Use saturated ultramarine only as a small depth accent; use black, charcoal, neutral gray, and cool white for the rest. Scarlet carries impact and ultramarine carries spatial depth, never overtaking the image.
- Let the subject occupy the main visual area. Use tilted, fractured, asymmetric panel divisions; a large black base and high-impact scarlet wedges should create a character-entry direction.
- Strengthen the rebellious, youthful energy of a torn poster by directing body orientation, clothing folds, scarlet wedges, repeated contours, and misregistered overprints toward one shared movement direction. Use ripped-paper edges, thick black separators, halftone, local white negative space, and a small number of cut-paper planes. Make the subject feel as if they are breaking onto a stage; avoid a static centered ID-photo composition.
- When they do not obstruct the face, eyes, gesture, or key equipment, optionally add zero to three original supporting elements: abstract masks, fictional weapons, companion animals, flower arrangements, background character silhouettes, signal graphics, or original UI. They support the subject's mood; they must not replace the subject, use an existing character design, or imply a specific work.
- Short original English text or graphic UI may be included. Use Arial for text, normally one to three words, legible but secondary to the subject. If the user provides a title, reproduce it exactly once. Prohibit game names, trademarks, brands, real logos, recognizable menus, signatures, watermarks, and proprietary copy that imitates an existing UI.

### Avoid

Avoid pores, realistic skin texture, natural skin color, individual realistic hairs, photographic depth of field, lens flare, soft realistic gradients, oil-paint marks, plastic-figure texture, 3D rendering, and direct photo filters. If the first result still reads as realistic, make only one targeted correction focused on linework, simplified features, hard-edged shadows, and flat material treatment.

## Landscape mode: colorful 2D anime scene

### Scene lock

Preserve the landmark, camera height, main perspective relationships, time/weather, and the three to six most informative scene facts. Examples include a bridge span and its cables, a river and skyline, the rhythm of a torii passage, temple eaves and foot traffic, layered streets, or nighttime lights.

### Visual grammar

- Use a harmonious multicolor palette appropriate to the scene. Sky, water, foliage, light, and architecture may use different colors. Do not impose the portrait mode's scarlet/black/gray/white restriction on landscapes.
- Organize the image with an original animated-cinema feeling: clear foreground, middle ground, and background; use eaves, bridges, roads, tree canopies, railings, riverbanks, or crowd silhouettes to lead the eye; establish one focus with sunlight, lanterns, neon, reflections, a break in the clouds, or other light derived from the source.
- Compress real materials into clear contours, concise linework, two to three cel-shaded values, and soft but restrained atmospheric perspective. Layer cool and warm color: the foreground may be deeper, the middle ground carries the principal colors, and the distance and sky retain high-value light. Small amounts of grain, horizontal light bands, glowing cloud edges, or halftone are allowed but must not cover the place itself.
- Add at most one environment action derived from the original scene, such as water ripples, traffic light trails, wind-blown flags, distant abstract firework-like lights, or lanterns turning on. Do not invent major people, animals, vehicles, monsters, or narrative props.
- Do not generate readable text by default. Remove or abstract signage, brands, logos, advertisements, copyrighted characters, and watermarks in the source; never replace them with pseudo-text.

### Special source handling

If the photo contains a theme park, protected architecture, commercial signage, on-screen characters, or prominent trademarks, retain only non-identifying spatial relationships, natural light, ordinary architectural silhouettes, and camera mood. Remove details that identify a specific brand, work, or location design. Never use any reference CG, screenshot, or web image as output material or directly reproduce its composition.

## Pre-delivery check

- Is the mode correct: does a portrait read first as a character poster, and does a landscape read first as an animated scene with spatial depth?
- Does the person remain recognizable, with sound pose, hands, glasses, and mask structure?
- Does the landscape retain its scene facts, depth, and focal point while removing brands and identifiable IP?
- Is the portrait scarlet-led with only small ultramarine depth accents; does the landscape use natural, rich, harmonious multicolor?
- Are realistic texture, logos, trademarks, watermarks, pseudo-text, copyrighted character traits, and unauthorized added people absent?

## Example boundary

Example files are paired as `<subject>-source.*` with `<subject>-portrait-punk.png` or `<subject>-landscape-cinematic.png`. They demonstrate only the degree of 2D stylization, color logic, hierarchy, shadows, and composition strength. Never copy their person, location, clothing, pose, props, text, or exact composition.
