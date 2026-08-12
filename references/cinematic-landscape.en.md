# Cinematic 2D Landscape Specification

## Contents

1. Input and scene lock
2. Visual language
3. Special sources
4. Mixed scenes
5. Text and copyright boundary
6. Output and quality check

## 1. Input and scene lock

Require a user-uploaded photo. If none is attached, ask for one and stop. Generate one complete image by default. Preserve the source orientation and approximate ratio; use `16:9` when a new horizontal cinematic crop is needed.

Preserve landmark geometry, camera height, viewpoint, perspective relationships, time and weather, spatial hierarchy, and three to six high-information facts needed to recognize the place. Examples include a bridge span and cables, a river and skyline, the rhythm of a torii passage, temple eaves and foot traffic, layered streets, or nighttime lights.

Internally perform `OBSERVE → LOCK → DISTILL → ILLUSTRATE → LIGHT → CHECK`. Select high-information facts, remove low-information photographic clutter, and compress real materials into clear contours, flat color shapes, and restrained atmospheric perspective. Do not expose the analysis.

## 2. Visual language

Aim for a saturated, multicolor, original animated-film scene. Do not impose the subject-poster route's red-black-white graphic system.

- Use a harmonious multicolor palette suited to the scene's mood. Sky, water, foliage, light, architecture, and pavement may use different hues, but unify their temperature relationships and value hierarchy.
- Establish a clear foreground, middle ground, and background. Use eaves, bridges, roads, tree canopies, railings, riverbanks, or crowd silhouettes to lead the eye.
- Build one emotional focus from sunlight, sunset, lanterns, neon, reflections, a break in the clouds, fireworks, or another source-derived light. Organize saturated regions around the focus rather than distributing them evenly.
- Simplify real materials into concise linework, clear contours, and two to three color blocks. The foreground may be deeper and firmer, the middle ground carries the principal color, and distance and sky retain brightness and atmosphere.
- Allow soft glow at cloud edges, local reflections, restrained atmospheric perspective, and small areas of animated light bloom, but never turn the result into a photo filter, semi-realistic concept painting, or 3D render.
- Small amounts of grain, halftone, or horizontal light bands may support atmosphere but must not cover place structure. Prohibit global grime, excessive gray haze, and dense noise.
- Add at most one source-derived environmental action, such as water ripples, traffic light trails, wind-blown flags, distant abstract firework-like lights, or lanterns turning on. Do not invent major people, animals, vehicles, monsters, or narrative props.

The result must read immediately as a 2D animated-film scene: clear contours, summarized color shapes, and designed light while retaining the source place's recognizable structure.

## 3. Special sources

Ordinary public buildings, streets, bridges, temples, shrines, and natural landmarks may retain their real geometry and place relationships.

If the source contains a theme-park set, branded installation, commercial screen, copyrighted character, or prominent trademark, remove only the character, logo, advertising copy, and proprietary ornament that identifies a brand or work. Preserve the real viewpoint, ordinary structural geometry, natural light, and spatial relationships whenever possible. Do not genericize an entire place merely because signage is present.

## 4. Mixed scenes

When a photo contains a person, pet, or object but the user primarily cares about the travel location, building, or environment, keep the landscape route:

- Preserve subject count, basic pose, clothing silhouette, or animal markings, but treat the subject as a scene character rather than redesigning it into a masked-action poster figure.
- Preserve contact, scale, and orientation between subject and place, such as a person leaning on a railing, a pet sitting by a window, or a person standing before a bridge.
- Do not add real people, and do not turn incidental crowds into detailed portrait focal points.
- If the user changes priority to identity and an original action redesign, switch to the masked-action poster reference instead of blending both systems.

## 5. Text and copyright boundary

Generate no readable text by default. Abstract signs, advertisements, brands, logos, on-screen characters, and watermarks into blank graphic shapes or non-text color blocks; prohibit pseudo-text. Reproduce a user-supplied title exactly once in Arial.

Animated-film and game-cutscene screenshots may inform only saturated multicolor, cinematic light, layered space, and emotional focus. Never reproduce a screenshot, character, proprietary UI, text, camera crop, composition, or a particular work's identifiable visual signature.

## 6. Output and quality check

Before delivery, check:

- Are landmark geometry, viewpoint, time and weather, spatial relationships, and three to six place facts preserved?
- Are foreground, middle ground, and background clear, and do light and color establish one focus together?
- Is the color rich, natural, and harmonious rather than forced into red, black, gray, and white or broad meaningless gray-black?
- Are source brands, logos, screen characters, and advertisements abstracted without over-genericizing the place?
- Are there no invented major people, animals, vehicles, monsters, or narrative props?
- Does it clearly read as a 2D animated-film scene rather than a photo filter, semi-realistic game painting, or 3D render?
- Is it free of global grime, excessive grain, pseudo-text, and watermarks?

If place structure is wrong or the result is excessively realistic, abnormally color-limited, or globally distressed, make only one targeted correction. Do not redraw repeatedly without a precise failure target.

Save the final image to the current project's `images/photo-personalike-poster/` directory with a short, clear English filename. Keep only the latest formal version.
