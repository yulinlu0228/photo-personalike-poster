# Multi-Image Input Routing and Clarification

## Contents

1. Goal and principles
2. Input inventory
3. When to generate directly
4. When clarification is required
5. One-pass clarification format
6. Generation manifest
7. Special cases and prohibitions
8. Delivery labels

## 1. Goal and principles

For a multi-image task, first resolve which inputs jointly serve each output. Ask only about unknowns that change output count, route, identity, subject count, or reference roles. Do not block generation for irrelevant information. Combine all necessary questions into one short structured clarification instead of interrogating the user image by image.

If the user already specifies output count, route per output, and reference roles, execute directly. Ask only about remaining ambiguity that would materially change the result.

## 2. Input inventory

Number inputs in upload order as `Image 1, Image 2 … Image N`, then internally record:

- Type: subject-led, place-led, or mixed with equal subject and place importance.
- Possible identity groups: people clearly known to be the same, clearly known to be different, or uncertain.
- Possible roles: identity, pose, clothing, object, environment, viewpoint, light, or color reference.
- Conflicts: inconsistent age impression, hair, clothing, equipment, place, or time across inputs.

Never decide that people in two photos are the same or different merely from resemblance or dissimilarity. When confidence is insufficient, state that their identity relationship is uncertain.

## 3. When to generate directly

- When all inputs are one clearly consistent type, generate one corresponding output per input by default: masked-action posters for subject-led inputs and Persona-5-CG-inspired landscapes for place-led inputs.
- When the user explicitly requests separate treatment, route every clear input automatically. Identity relationships across separate outputs usually do not affect the result and must not be mandatory.
- When the user provides a complete custom output manifest, follow it directly.

Even with separate treatment, if one input itself gives equal importance to subject and place, clarify only whether that input should use poster mode, landscape mode, or one of each.

## 4. When clarification is required

Ask once before generation when any of these conditions applies:

- The set mixes subject-led, place-led, or mixed-focus inputs and the user has not chosen separate treatment or shared references.
- Two or more subject images will feed one output and it is uncertain whether they show the same person.
- Final output count or route per output is unresolved.
- Subject/identity versus environment reference roles are unresolved.
- It is unclear whether the final output should contain one main person, multiple people, or people only as secondary landscape figures.
- Multiple same-type images may show one person or place from several views and the user indicates merging, shared reference, or one combined output.

## 5. One-pass clarification format

State the observable classification and only the material ambiguity, then offer a separate default and a shared/custom alternative. Do not expose hidden visual analysis.

Recommended template:

> I identified Image 1 as a landscape and Images 2 and 3 as portraits, but I cannot confirm whether Images 2 and 3 show the same person. Please choose an output arrangement:
>
> **1) Generate all three separately (default):** one Persona-5-CG-inspired landscape from Image 1 and one masked-action poster each from Images 2 and 3, for three outputs total. Their identity relationship is not required for this option.
>
> **2) Shared-reference or custom outputs:** please confirm once:
> - Do Images 2 and 3 show the same person from different views, or two different people?
> - How many final images should be generated?
> - Which route should each output use: masked-action poster or Persona-5-CG-inspired landscape?
> - Which input images are subject/identity references and which are environment references for each output?
> - How many main people should appear in each output?
>
> Example reply: `Generate two images. Output 1: masked-action poster; Images 2 and 3 are the same identity references, Image 1 is the environment reference, and one person appears. Output 2: landscape mode; Image 1 is the environment reference and Image 2 is only a secondary scene-person reference.`

Adapt the template to the actual input count and classification. Remove any question already answered; never make the user repeat information.

## 6. Generation manifest

After the answer, internally resolve every output into this manifest:

| Field | Required resolution |
| --- | --- |
| Output number | Output 1, Output 2 … |
| Route | Masked-action poster or Persona-5-CG-inspired landscape |
| Subject/identity references | Image numbers and identity grouping; none when absent |
| Environment references | Image numbers and primary/secondary status; none when absent |
| Other reference roles | Pose, clothing, object, light, or color only when specified or conflicting |
| Final subject | Main-person count, or environment-primary with secondary people |

Generate immediately once the manifest is complete. Do not ask for a second confirmation. If the answer still lacks one field that would change the result, ask only for that field.

## 7. Special cases and prohibitions

- Multiple photos of one person may strengthen identity, angle, and detail, but final person count comes from the manifest. Never duplicate a person according to photo count.
- Never fuse the faces, skin, hair, or body traits of different people. Lock each identity separately in a multi-person output.
- One portrait may serve identity while another serves only pose or clothing, but the manifest must say so. Never transfer pose or clothing from one person to another without permission.
- Treat a group photo as one input unit by default. Do not split it into individual outputs without permission.
- When multiple environment images are shared, name one primary place or obtain permission for a fantasy fusion. Never mechanically combine unrelated landmarks into one supposedly real location.
- In poster mode, environment references provide stage, contour, and symbols without overpowering the identity subject. In landscape mode, subject references are secondary scene figures by default. If strict identity preservation and subject prominence are required, use poster mode.
- A mixed image may serve both identity and environment roles, but record both roles separately.
- Multiple uploads do not automatically mean more outputs, and shared references do not automatically mean only one output.

## 8. Delivery labels

Describe every output in manifest order:

> Output 1: masked-action poster mode; Images 2 and 3 are subject references for one identity; Image 1 is the environment reference; one main person appears.  
> Output 2: Persona-5-CG-inspired landscape mode; Image 1 is the environment reference; Image 2 serves only as a secondary scene-person reference.

For separate treatment, still state the input-to-output mapping. Never report only that all images were generated.
