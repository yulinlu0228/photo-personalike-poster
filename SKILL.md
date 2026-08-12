---
name: photo-personalike-poster
description: "Transform an uploaded photo through one of two independent routes: a bright, clean, high-contrast original masked-action pop poster for an identity-bearing person, group, pet, animal, or object; or a colorful cinematic illustrated landscape that preserves recognizable place facts. Use for portrait-to-action-poster, original theatrical costume and pose redesign, subject-plus-place posters, pet or object entry posters, and photo-to-animated-landscape requests. Require an uploaded source photo before generation."
---

# Photo Personalike Poster

## Core workflow

Require one uploaded photo, then internally follow `OBSERVE → ROUTE → LOCK → DISTILL → STYLIZE → COMPOSE → CHECK`. Do not expose the analysis. Generate one finished image and make at most one targeted correction when a hard requirement fails.

Choose exactly one primary route:

- **Masked-action poster:** an identity-bearing person, group, pet, animal, or object is the focus. A human subject may receive an original dynamic pose, theatrical costume, mask, prop, and graphic stage when permitted by the preservation rules.
- **Cinematic landscape:** the place, weather, light, and spatial experience are the focus; people or animals are incidental scene elements.

For a mixed subject-and-place photo, follow the user's priority. Without one, use the poster route when identity is the intended focus and the landscape route when place recognition is the intended focus. Do not blend the two visual systems into a third mode.

## Preserve

- In poster mode, lock subject count, recognizable identity, age impression, face and hair, protected traits, original body build and proportions, and identity-bearing equipment. Redesign ordinary pose and clothing only when the user allows it or has not required preservation.
- In landscape mode, lock viewpoint, landmark geometry, perspective, time and weather, spatial relationships, and three to six defining scene facts.
- Preserve culturally, medically, religiously, occupationally, and safely significant clothing or equipment in either route.

## Route requirements

- For the **poster route**, read only the matching [Chinese poster reference](references/masked-action-poster.zh-CN.md) or [English poster reference](references/masked-action-poster.en.md). Enforce its bright-value, clean-surface, anatomy, costume, action, motif-density, and torn-frame gates before delivery. Treat torn paper as large structural framing and panel interruption, never as a global dirty texture.
- For the **landscape route**, read only the matching [Chinese landscape reference](references/cinematic-landscape.zh-CN.md) or [English landscape reference](references/cinematic-landscape.en.md). Do not import the poster palette or collage density into scenery.

Honor a user-specified ratio. Otherwise choose the poster ratio from the action: use `16:9` for lateral movement, full-body action, ensembles, or a wide graphic stage; use `4:5` for a dominant single figure or upward motion. Preserve a landscape's orientation and approximate ratio unless a cinematic `16:9` crop clearly improves it.

## Main prohibitions

Do not imitate a named game, character, artist, poster, UI, or screenshot. Do not copy a reference image's costume, pose, mask, prop, framing, text, or composition. Do not retain logos, brands, advertisements, watermarks, copyrighted character designs, or readable pseudo-text. Do not change identity or protected traits, distort adult body proportions, replace a pet with a generic animal, or add realistic people absent from the source. When text is allowed, reproduce the user's exact title once or use short original English copy in Arial.

## Output

Save the final image to the current project's `images/photo-personalike-poster/` directory with a short descriptive English filename. Keep only the latest approved formal result.

## Examples

Use `assets/examples/` only as authorized source/output pairs for visual boundaries. Landscape pairs demonstrate cinematic depth, light, and multicolor; subject pairs demonstrate normal adult proportions, layered motif richness, and torn-paper framing built from large clean ruptures rather than dirty texture. Never treat an example as a template or copy its identity, place, clothing, scene, pose, motif, or composition.
