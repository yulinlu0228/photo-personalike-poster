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

A user-specified aspect ratio takes priority. Otherwise choose a human subject-poster ratio from the composition: prefer `16:9` for lateral sweeps, full-body action, prop direction, group relationships, or a wide decorative stage; prefer vertical `4:5` for a dominant single close-up, upward motion, or fashion-like entrance; retain another source ratio when it serves the image better. For a landscape, preserve the source orientation and approximate aspect ratio; use `16:9` when a new horizontal cinematic crop is needed. A mixed scene follows its selected mode. Never mechanically fix every subject poster to `4:5`.

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

- **One person or a group — absolute lock:** preserve count, basic face shape, age impression, hairline, hairstyle, eye direction, primary expressive character, ethnic traits, body proportions, glasses/visual aids, medical or accessibility equipment, and other identity-bearing objects. Do not beautify, de-age, gender-swap, change ethnic traits, add muscle, or rewrite body proportions.
- **One person or a group — conditional lock:** preserve pose, relative placement, clothing, masks, and hand relationships exactly only when the user asks or when they carry occupational, cultural, religious, medical, safety, accessibility, interaction, or identity meaning. Ordinary photo poses and non-identifying basics may be redesigned to improve action and theatrical impact.
- **Pet or animal:** preserve species and breed impression, head and face proportions, ear shape, muzzle, eye direction, coat colors and marking placement, tail, pose, collar, and distinctive accessories. Do not replace it with a generic animal or add a human body, hands, clothing, or human expression by default. Anthropomorphize only when the user explicitly requests it.
- **Object:** preserve outer silhouette, proportions, functional structure, principal material cues, and identifying details. Do not alter its purpose or construction merely to make it look cooler.

### 4.2 Visual grammar

- Use complete black contours with clear line-weight variation, grouped block shapes for hair or fur, simplified but identity-preserving facial features, hard-edged cel shadows, and two to three value blocks per surface.
- Do not force human skin into black, gray, and white. Build two to three hard-edged animated skin tones from the person's actual skin tendency, preserving value range, warm/cool undertone, and identity-bearing ethnic traits while allowing stronger saturation or temperature contrast. Light skin may use ivory, peach, pale apricot, and warm-gray shadow; medium skin may use honey, ochre-apricot, copper-brown, and warm-brown shadow; dark skin may use deep copper, red-brown, cocoa, and violet-brown shadow. Never lighten dark skin into light skin, drain any skin into lifeless gray, or fill a face with solid red. Separate highlight, local color, and shadow as clear shapes rather than realistic soft gradients.
- Default to a scarlet, black, and white graphic anchor, but do not enforce a strict limited palette. Choose two or three coordinated supporting hues from ultramarine, cobalt, cyan, magenta, pink, violet, cream, limited gold, or green according to clothing, personality, and scene. Use one dominant color, two or three supporting colors, and neutrals; every support color must clarify depth, identity, or mood rather than forming an evenly distributed rainbow.
- Give the subject roughly `55%–75%` of the visual weight. Boldly crop hair, clothing edges, or peripheral limbs when useful, but keep identity anchors intact. Avoid a centered standing or ID-photo layout; prefer off-center placement, a tilted horizon, foreshortening, local perspective enlargement, and foreground overlap. If the source action is expressive or conditionally locked, preserve its joints while amplifying direction. If it is calm, stiff, or merely photographic and the user did not require preservation, redesign it into a body-appropriate run, leap, abrupt turn, forward lunge, rotational sweep, one-knee landing, boundary-breaking reach, or diagonal prop action. The new pose must be anatomically plausible, balanced, and clear in the hands while preserving face, hair, age impression, and body proportions.
- Establish one dominant motion axis. Align body direction, hair or clothing flow, a weapon or bouquet, sliced panels, and speed forms with it, then use a weaker counter-directional family to create tension. At first glance, show at least three strong signals together: bold off-center crop, obvious perspective or foreground overlap, an oversized graphic or prop, repeated/misregistered silhouette, torn paneling, a dense decorative field, or a collision of strong negative space.
- Organize the background into three levels: (1) a large black or saturated base shape for silhouette contrast; (2) medium fractured panels, rays, checker patterns, comic bursts, flower clusters, silhouettes, or scene symbols for rhythm; and (3) small halftone, registration offsets, paper texture, icons, and UI marks for detail. Vary scale and density, keep a clear reading zone around the face, and never give every element the same size or contrast.
- Use three to seven related original supporting motifs rather than restricting decoration too severely. Options include an abstract mask, fictional weapon or tool, bouquet, symbolic animal, character silhouette, card-like geometry, musical notes, stars, roses, chains, sparks, signal graphics, or fictional UI. Choose one primary motif and vary the others around it; do not pile up unrelated assets. Never cover the face, eyes, identifying animal markings, key gesture, or identity-bearing object, and never imply an existing character. For an animal subject, prefer non-contact graphics, foliage, lunar shapes, paw marks, speed forms, or environmental silhouettes.
- Original English copy of one to three words or graphic UI may be included. Use Arial and keep text secondary. Reproduce a user-supplied title exactly once. Prohibit game names, trademarks, logos, real menus, signatures, watermarks, brand copy, and pseudo-text.

### 4.3 Original masked-action costume redesign

When the user allows clothing changes, or ordinary daily clothing cannot support the intended entrance energy, redesign it into an original masked-action / theatrical thief costume. This is a broad costume language, not permission to reproduce any existing game character:

- Choose three to five elements from a fitted high collar, asymmetric tailored long coat, short cape or split long tails, layered lapels, harness-like seam lines, bracers, long gloves, narrow trousers, tall boots, metal fasteners, and a small area of bright lining. Organize them around one clean silhouette.
- An original eye mask may be added, but it must keep eye direction and face shape readable, cover only the eye area or half-face, and never copy an existing character's mask, horns, pattern, palette, or silhouette. If the source has glasses, respiratory protection, religious wear, or medical equipment, preserve it and integrate it safely rather than replacing it.
- Separate costume and background hierarchy: use black or a deep value for the main silhouette; place the dominant saturated hue in lining, gloves, cape edges, straps, or footwear; use support hues only for depth and identifying accents. Do not make every garment component equally bright.
- Make clothing serve the pose: tails, cape, scarf, cuffs, and straps should stream along the motion axis rather than cling rigidly, without covering the face or gesture or changing body proportions.
- Do not add an existing character's uniform, insignia, badge, signature weapon, companion, or story symbol. Any fictional weapon or tool must be original, functionally ambiguous, and unbranded; omit it when it does not suit the person.

### 4.4 Tension threshold and composition choice

Choose one primary composition from the source pose instead of applying the same template every time:

- **Burst into frame:** for an arm, leg, bouquet, or prop extending toward the camera; use foreshortening and foreground boundary breaks.
- **Rotational sweep:** for a side pose, turn, long hair, or loose clothing; form a vortex with hair, fabric, panels, and background arcs.
- **Diagonal intrusion:** for a seated, leaning, or restrained upper-body pose; when pose redesign is allowed, convert it into an abrupt turn, forward lunge, or diagonal prop action, then increase energy through tilted crop, local enlargement, repeated silhouette, and counter-wedges.
- **Stage spotlight:** for composed or restrained poses; surround the subject with oversized flowers, masks, symbols, or silhouettes, using a strong black base, luminous skin, and saturated edge colors for theatrical contrast.
- **Widescreen pursuit:** for `16:9`; make the figure run, leap, rotate, or stop across the frame, with prop, cape, and decorations extending laterally. Leave directional room ahead of the movement rather than dropping a vertical figure into a wide rectangle.

The result must go beyond “half-body figure on a red-and-black background.” If the action remains stiff, the subject is too small, the background feels empty, or decoration is evenly scattered, use the single targeted correction to strengthen subject scale, motion axis, foreground overlap, and background hierarchy together rather than adding random stickers.

### 4.5 Avoid and correction

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
- Does each person remain recognizable, with correct count, body proportions, anatomically plausible hands, glasses, and mask structure? If pose or clothing was redesigned, is it within user authorization, physically balanced, and inside the original masked-action costume boundary?
- Are the animal's ears, muzzle, markings, tail, pose, and accessories correct, without accidental anthropomorphism?
- Are the object's silhouette, proportions, and functional structure correct?
- Does the landscape preserve place facts, depth, light, and focus while removing brands and copyrighted characters?
- Does the subject poster have a clear motion axis, a sufficiently large subject, at least three strong tension signals, and layered decoration? Does the palette have hierarchy, and does skin preserve the source person's value and undertone without being grayed, lightened, or filled red? Is the landscape naturally rich and harmonious?
- Is the result clearly two-dimensional and free of logos, trademarks, watermarks, pseudo-text, protected characters, and unauthorized added real people?

If the result has obvious realism, a structural error, or a mode-specific color failure, make only one targeted correction. Do not redraw repeatedly without a precise failure target.

## 8. Example boundary

Pair examples as `<subject>-source.*` with `<subject>-subject-punk.png` or `<subject>-landscape-cinematic.png`. Examples demonstrate only the degree of 2D stylization, color logic, subject hierarchy, shadows, widescreen action redesign, and original masked-action costume transformation. Never copy their person, animal, place, clothing, mask, pose, prop, text, or exact composition. Every example is one possibility rather than a fixed template; prioritize this file's routing and high-tension rules.
