---
name: photo-personalike-poster
description: "Transform one or many uploaded photos through two independent routes: a bright, clean, high-contrast original masked-action pop poster for an identity-bearing person, group, pet, animal, or object; or an original colorful Persona-5-CG-inspired cinematic landscape that preserves recognizable place facts without copying the game. Use for portrait-to-action-poster, original theatrical costume and pose redesign, subject-plus-place routing, pet or object entry posters, photo-to-animated-landscape requests, and multi-image batches or composites. Require uploaded source photos before generation."
---

# Photo Personalike Poster

## Core workflow

Require at least one uploaded photo, then internally follow `OBSERVE → COUNT → CLASSIFY → ROUTE → LOCK → DISTILL → STYLIZE → COMPOSE → CHECK`. Do not expose the visual analysis. Generate one finished image per resolved output and make at most one targeted correction per output when a hard requirement fails.

Choose exactly one primary route:

- **Masked-action poster:** an identity-bearing person, group, pet, animal, or object is the focus. Its highest visual goal is immediate impact, vitality, and a vivid sense of life. A human subject may receive an original dynamic pose, theatrical costume, mask, prop, and graphic stage when permitted by the preservation rules. A technically compliant but static, stiff, decorative, or template-like result fails this route.
- **Cinematic landscape:** the place, weather, light, and spatial experience are the focus; people or animals are incidental scene elements.

## Input-count routing

For **one uploaded photo**:

- If it is clearly a landscape or place photo with no identity-bearing subject, automatically use **Persona-5-CG-inspired cinematic landscape mode**.
- If it is clearly a portrait or subject-led photo whose person, group, pet, animal, or object dominates, automatically use **masked-action poster mode**.
- If both an identity-bearing subject and a recognizable place are important, pause before generation and ask exactly one short question: “请选择生成方式：1）怪盗海报模式；2）Persona 5 CG 气质的风景图片模式；3）两种模式各生成一张。” Generate one or two outputs according to the answer.

For **multiple uploaded photos**:

- If all images are clearly the same type, generate one result per input automatically: poster mode for all subject-led images or landscape mode for all place-led images.
- If the set mixes subject-led, place-led, or mixed-focus images, read the matching [Chinese multi-image routing reference](references/multi-image-routing.zh-CN.md) or [English multi-image routing reference](references/multi-image-routing.en.md). Ask one consolidated clarification covering only material unknowns: identity grouping, separate versus shared-reference outputs, output count, route per output, reference roles, and intended subject count.
- First offer the fully separate default with its resolved output list. If the user chooses it, identity relationships across different outputs are optional and must not block generation.
- For shared-reference or custom outputs, never guess whether uncertain people are the same identity. Resolve every output into a generation manifest before drawing. Do not ask again when the user's request already resolves all material fields.
- Do not silently treat multiple views of the same person as separate identities, fuse different identities, combine unrelated places, split a group photo, or merge inputs into one image without permission.

“Persona-5-CG-inspired” is user-facing shorthand only. In prompts, use original saturated multicolor, cinematic lighting, layered space, and animated-cutscene atmosphere; never request a direct copy of a game screenshot, protected character, UI, or exact composition.

## Preserve

- In poster mode, lock subject count, recognizable identity, age impression, face and hair, protected traits, original body build and proportions, and identity-bearing equipment. Redesign ordinary pose and clothing only when the user allows it or has not required preservation.
- In landscape mode, lock viewpoint, landmark geometry, perspective, time and weather, spatial relationships, and three to six defining scene facts.
- Preserve culturally, medically, religiously, occupationally, and safely significant clothing or equipment in either route.

## Route requirements

- For the **poster route**, read only the matching [Chinese poster reference](references/masked-action-poster.zh-CN.md) or [English poster reference](references/masked-action-poster.en.md). Enforce its impact-and-vitality, bright-value, clean-surface, anatomy, costume, action, motif-density, and torn-frame gates before delivery. Treat torn paper as large structural framing and panel interruption, never as a global dirty texture.
- For the **landscape route**, read only the matching [Chinese landscape reference](references/cinematic-landscape.zh-CN.md) or [English landscape reference](references/cinematic-landscape.en.md). Do not import the poster palette or collage density into scenery.

Honor a user-specified ratio. Otherwise choose the poster ratio from the action: use `16:9` for lateral movement, full-body action, ensembles, or a wide graphic stage; use `4:5` for a dominant single figure or upward motion. Preserve a landscape's orientation and approximate ratio unless a cinematic `16:9` crop clearly improves it.

## Main prohibitions

Do not imitate a named game, character, artist, poster, UI, or screenshot. Do not copy a reference image's costume, pose, mask, prop, framing, text, or composition. Do not retain logos, brands, advertisements, watermarks, copyrighted character designs, or readable pseudo-text. Do not change identity or protected traits, distort adult body proportions, replace a pet with a generic animal, or add realistic people absent from the source. When text is allowed, reproduce the user's exact title once or use short original English copy in Arial.

## Output

Save final images to the current project's `images/photo-personalike-poster/` directory with short descriptive English filenames. Keep only the latest approved formal result for each source or composite.

After delivery, enumerate every output in source or manifest order and state its route, for example: “第 1 张：怪盗海报模式；第 2 张：Persona 5 CG 气质的风景图片模式。” When one source produces both modes, label both results separately as `第 X 张-A` and `第 X 张-B`. For every shared-reference output, name its identity/subject references, environment references, and intended subject count.

## Examples

Use `assets/examples/` only as authorized source/output pairs for visual boundaries. Landscape pairs demonstrate cinematic depth, light, and multicolor; subject pairs demonstrate normal adult proportions, layered motif richness, and torn-paper framing built from large clean ruptures rather than dirty texture. Never treat an example as a template or copy its identity, place, clothing, scene, pose, motif, or composition.
