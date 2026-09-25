---
name: landscape-architecture-watercolor
description: Transform an uploaded landscape, cityscape, architecture, storefront, or architectural-interior photograph into a vertical editorial diptych that preserves the original photo and reconstructs its visual memory as subject-specific watercolor. Use for scenery and built environments; do not use for portrait or animal close-ups.
---

# Landscape & Architecture Watercolor

Create one finished vertical editorial image from one uploaded photograph. Keep the original photograph faithful in the upper section; create a watercolor memory panel below it. The watercolor must respond to the photograph's camera distance, lighting, spatial structure, and strongest visual memory rather than applying a fixed filter.

## Non-negotiable invariants

- Use the uploaded photo as the sole content and palette source.
- Preserve the photo unchanged except for proportional scaling or a restrained crop. Do not redraw, retouch, relight, extend, or stylize it.
- The lower panel is a reconstruction, not a miniature copy, tracing, generic watercolor landscape, or filtered photograph.
- Every prominent mark must correspond to an observed shape, axis, rhythm, light, reflection, or color role in the photo.
- Use genuine watercolor logic: transparent washes, reserved paper white, pigment pooling, selective hard/soft edges, and purposeful brush direction. Texture alone does not create watercolor.
- Keep the composition quiet and selective. Use only a few justified splashes, drips, blooms, or stains; omit them when the source does not support energetic marks.
- Create one original English title of two to five words, grounded in visible facts. No other text, logo, signature, date, or watermark.

## Workflow

1. Classify the photograph by subject, camera distance, and dominant light using [scene-routing.md](references/scene-routing.md).
2. Identify three to six decisive facts: major masses, perspective or horizon axes, light-dark pattern, dominant color roles, repeated elements, reflections, negative space, and movement.
3. Select no more than five cue types for the lower panel. A repeated family such as windows, lamps, boats, spires, or people counts as one cue type. If the panel still reads as a complete scene or facade, remove cues rather than adding texture.
4. Choose one primary watercolor language and at most two supporting mark families. Do not combine every available effect.
5. Preserve the minimum recognition cues required for this specific place or structure; remove surface detail and background noise.
6. Build the lower panel from large relationships to small accents: pale wash/white reservation first, principal masses second, structural darks third, accents last.
7. Check that the result could not plausibly describe an unrelated photograph with the same broad subject.
8. Return only the completed diptych.

For reusable prompt scaffolds, read [prompt-recipes.md](references/prompt-recipes.md) after selecting the scene branch. Do not load recipes for unrelated branches.

## Editorial composition

- Join photo and panel directly without frame, shadow, tape, torn edge, collage mockup, or gap.
- Use warm ivory cold-press paper in the watercolor panel. Keep large areas untouched.
- Target roughly 65–80% clean or nearly clean panel space. Wide landscape bands may occupy more width but should stay low.
- Adapt the split to the photograph: horizontal views generally use 38–52% photo height; vertical architecture generally uses 55–68%; balanced images use 48–58%. Adjust when the subject requires it.
- Place the title below or beside the watercolor motif in a restrained editorial serif. Choose deep muted color from the source, not default black.

## Quality gate

Reject and retry when any of these are true:

- The lower panel looks like a softened or posterized copy of the photo.
- All regions receive equal detail or equal contrast.
- Watercolor appearance comes mainly from paper texture, noise, or edge roughness.
- Architecture contains many literal windows, bricks, signs, ornaments, or perspective details.
- Landscape depth is represented by outlines instead of value, temperature, overlap, or atmospheric wash.
- Splashes and stains are decorative rather than derived from light, weather, foliage, writing, reflection, or structural rhythm.
- The source's strongest memory cue is missing.
- The lower panel keeps a complete facade, room, landscape, boat, or other literal object when a directional mark would carry the same memory.
- The photo or panel has a vignette, black corner, glow, gradient, frame, or unintended shadow.

Retry at most twice for the same concept. Each retry must correct one named failure rather than add more style effects. If the result still fails, report the limitation and keep the best clearly labelled preview.

## Pixel-faithful delivery

Image generation may reconstruct the photographic section even when prompted not to. For a final that must preserve the original pixels, generate the watercolor panel separately and combine it with the source photo using deterministic image compositing. Treat a one-shot generated diptych as a visual preview unless direct comparison confirms pixel identity.

When a named living artist is supplied as a reference, do not imitate that artist exactly. Translate only broad, non-exclusive attributes such as transparency, edge control, limited palette, negative space, geometric simplification, or gestural energy.
