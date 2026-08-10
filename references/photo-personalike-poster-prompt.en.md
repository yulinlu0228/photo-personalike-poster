# Photo Personalike Poster: Full Image-Generation Specification

## Contents

1. Input and routing
2. General workflow
3. Style-inspiration boundary
4. Subject-poster mode
5. Landscape-scene mode
6. Mixed scenes
7. Output and quality check
8. Example boundary

## 1. Input and routing

Require a user-uploaded source photo. If no photo is attached, ask the user to upload one and stop. Generate one complete image by default.

Choose a route first:

- **Subject poster:** a person, group, pet, other animal, or object carries the primary identity and visual focus.
- **Landscape scene:** the place, weather, light, or environment is the primary focus; people are incidental scale or ambient elements.
- **Mixed scene:** subject and place are equally important. Follow the user's stated priority; otherwise default to subject-poster treatment while preserving three to five defining scene facts.

A user-specified aspect ratio takes priority. Otherwise use vertical `4:5` for a subject poster. For a landscape, preserve the source orientation and approximate aspect ratio; use `16:9` only when a new horizontal cinematic crop is needed. A mixed scene follows its selected mode.

## 2. General workflow

Internally perform `OBSERVE → ROUTE → PRESERVE → DISTILL → STYLIZE → COMPOSE → CHECK` without exposing the analysis.

1. Identify subject type, count, pose, and identity anchors.
2. Lock the structures of the people, animals, objects, or place that must not change.
3. Select three to six high-information scene facts and remove photographic noise and low-information clutter.
4. Compress real materials into clear contours, flat color shapes, and two to three value levels.
5. Build either a subject-entry poster or a cinematic scene according to the route.
6. Check identity, structure, color, text, copyright boundaries, and the degree of 2D stylization.

The result must read first as two-dimensional animation or cel-shaded illustration, never as a photo filter, semi-realistic game key art, or a 3D render.

## 3. Style-inspiration boundary

Use an original rebellious pop-punk 2D poster language for subject mode, aiming for youthful motion, torn-collage energy, and high-contrast graphic relationships. For landscape mode, borrow only common qualities of animated films and game cutscenes: saturated multicolor, cinematic light, layered space, and one emotional focal point. Learn only abstract methods. Never reproduce a game screenshot, character, proprietary UI, text, camera crop, composition, accessory, logo, or a specific work's identifiable visual signature.

Reference images are for analyzing style boundaries only and must not become output material. Do not download third-party screenshots, character art, or unauthorized portraits into the Skill or a generated result.

## 4. Subject-poster mode

### 4.1 Subject lock

- **One person or a group:** preserve count, basic face shape, age impression, hairline, hairstyle, eye direction, expression, head tilt, body pose, relative placement, arm relationships, clothing type, glasses/goggles/masks, and identity-bearing objects. Do not beautify, de-age, gender-swap, change ethnic traits, add muscle, or rewrite body proportions.
- **Pet or animal:** preserve species and breed impression, head and face proportions, ear shape, muzzle, eye direction, coat colors and marking placement, tail, pose, collar, and distinctive accessories. Do not replace it with a generic animal or add a human body, hands, clothing, or human expression by default. Anthropomorphize only when the user explicitly requests it.
- **Object:** preserve outer silhouette, proportions, functional structure, principal material cues, and identifying details. Do not alter its purpose or construction merely to make it look cooler.

### 4.2 Visual grammar

- Use complete black contours with clear line-weight variation, grouped block shapes for hair or fur, simplified but identity-preserving facial features, hard-edged cel shadows, and two to three value blocks per surface.
- Let scarlet carry the primary impact. Use saturated ultramarine only as a small spatial-depth accent; use black, charcoal, neutral gray, and cool white for the rest. Map human skin to cool-white and neutral-gray animated value blocks rather than red. Remap an animal's natural markings into grayscale while preserving their placement.
- Let the subject occupy the primary visual area. Use tilted, fractured, asymmetric panels, a large black base, scarlet wedges, and a few ultramarine depth shapes to establish one movement direction.
- Use ripped-paper edges, thick black separators, halftone, repeated contours, misregistered overprints, local white negative space, and a few cut-paper planes. Align pose, clothing or fur flow, graphic wedges, and background rhythm toward one motion direction; avoid a static centered ID-photo composition.
- Optionally add zero to three original supporting elements: an abstract mask, fictional weapon or tool, flower arrangement, symbolic animal, character silhouette, signal graphic, or fictional UI. Do not cover a face, eyes, identifying animal markings, gesture, or key object. Supporting elements must not replace the subject or imply an existing character. For an animal subject, prefer non-contact graphics, foliage, lunar shapes, paw marks, speed forms, or environmental silhouettes.
- Original English copy of one to three words or graphic UI may be included. Use Arial and keep text secondary. Reproduce a user-supplied title exactly once. Prohibit game names, trademarks, logos, real menus, signatures, watermarks, brand copy, and pseudo-text.

### 4.3 Avoid and correction

Avoid pores, realistic skin, individual photorealistic hairs or fur, photographic depth of field, lens flare, soft realistic gradients, oil-paint marks, plastic-figure texture, 3D rendering, and direct photo filters. If the first result remains visibly realistic, make only one targeted correction focused on linework, simplified human or animal features, hard-edged shadows, and flat materials.

## 5. Landscape-scene mode

### 5.1 Scene lock

Preserve landmark geometry, camera height, viewpoint, perspective relationships, time/weather, and three to six high-information facts needed to recognize the place. Examples include a bridge span and its cables, a river and skyline, the rhythm of a torii passage, temple eaves and foot traffic, layered streets, or nighttime lights.

### 5.2 Visual grammar

- Use a harmonious multicolor palette suited to the scene's mood. Sky, water, foliage, light, and architecture may use different colors. Do not impose subject mode's limited palette.
- Establish clear foreground, middle ground, and background. Use eaves, bridges, roads, tree canopies, railings, riverbanks, or crowd silhouettes to lead the eye. Build one emotional focus from sunlight, lanterns, neon, reflections, a break in the clouds, or another source-derived light.
- Simplify real materials into clear contours, concise linework, two to three color blocks, and restrained atmospheric perspective. The foreground may be deeper, the middle ground carries principal colors, and distance and sky retain higher values. Small amounts of grain, horizontal light bands, glowing cloud edges, or halftone must not cover the place itself.
- Add at most one environmental action derived from the source, such as water ripples, traffic light trails, wind-blown flags, distant abstract firework-like lights, or lanterns turning on. Do not invent major people, animals, vehicles, monsters, or narrative props.
- Do not generate readable text by default. Abstract signs, advertisements, brands, logos, on-screen characters, and watermarks into blank graphic shapes or non-text color blocks; do not use pseudo-text.

### 5.3 Special sources

Ordinary public buildings, streets, bridges, temples, shrines, and natural landmarks may retain their real geometry and place relationships. If a source contains a theme-park set, branded installation, commercial screen, copyrighted character, or prominent trademark, remove only the character, logo, advertising copy, and proprietary ornament that identifies a brand or work. Preserve the real viewpoint, ordinary structural geometry, natural light, and spatial relationships whenever possible. Do not genericize an entire place merely because signage is present.

## 6. Mixed scenes

When a person, pet, or object and a place are equally important:

- By default, place the identity-bearing subject at the primary hierarchy and rebuild three to five place facts as secondary background contours, color shapes, or lighting cues.
- Preserve contact, scale, and orientation between subject and scene, such as a person leaning on a railing, a pet sitting by a window, or a person standing before a bridge.
- When the user explicitly emphasizes a travel location, building, or environment, switch to landscape mode. Preserve subject count, pose, clothing, or animal markings, but treat the subject as a scene character rather than a poster silhouette.
- Do not reduce a mixed photo with clear place information to a purely abstract background, and do not let background detail overpower the identity-bearing subject.

## 7. Output and quality check

Save the final image to the current project's `images/photo-personalike-poster/` directory with a short readable English filename, such as `scarlet-cat.png`, `city-couple.png`, or `river-sunset.png`. Keep only the latest formal version of each result.

Before delivery, check:

- Does the route match what the user actually cares about, and does a mixed scene preserve the subject-place relationship?
- Does each person remain recognizable, with correct count, pose, anatomically plausible hands, glasses, and mask structure?
- Are the animal's ears, muzzle, markings, tail, pose, and accessories correct, without accidental anthropomorphism?
- Are the object's silhouette, proportions, and functional structure correct?
- Does the landscape preserve place facts, depth, light, and focus while removing brands and copyrighted characters?
- Is the subject poster scarlet-led with restrained ultramarine, and is skin cool-white/gray rather than red? Is the landscape naturally rich and harmonious?
- Is the result clearly two-dimensional and free of logos, trademarks, watermarks, pseudo-text, protected characters, and unauthorized added real people?

If the result has obvious realism, a structural error, or a mode-specific color failure, make only one targeted correction. Do not redraw repeatedly without a precise failure target.

## 8. Example boundary

Pair examples as `<subject>-source.*` with `<subject>-subject-punk.png` or `<subject>-landscape-cinematic.png`. Examples demonstrate only the degree of 2D stylization, color logic, subject hierarchy, shadows, and composition strength. Never copy their person, animal, place, clothing, pose, prop, text, or exact composition.
