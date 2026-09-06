---
name: xxd-panel-120
description: "Create XXD Panel 120 raster artwork from a source photograph as an architectural concept perspective sketch: relaxed freehand lines, sparse geometric guides, selective colour blocks, geometric shadows, and extensive whitespace. Use when the user invokes xxd-panel-120 or requests this architectural concept-sketch editorial transformation. Supports isolated image or directory inputs, strict 50:50 comparisons, design-only work, and wallpapers."
---

# XXD Panel 120

Create finished PNG artwork from the current photograph or image directory. Read `references/original-prompt/zh-CN.md` completely immediately before every generation. This verbatim Chinese brief is the sole creative and aesthetic authority. Reading translations, README copy, samples, and other Panels never replace or modify it.

## Delivery contract

- One original photograph produces isolated outputs. Never combine sources, copy another source's subject or wording, or use a sample as the input.
- Canonical presentation is a 3:4 portrait, photograph above and architectural concept sketch below, exactly 50:50.
- Resolve modes, sizes, text mode, locale, wallpaper relationship, device sizes, and output root from the current request and safe delivery preferences before generating.
- `top-bottom`: exactly two full-width equal-height regions; photograph above, design below.
- `left-right`: exactly two full-height equal-width regions; photograph left, design right. This explicit delivery selection overrides only the original brief's 3:4 top/bottom layout: map every “upper/photo” instruction to the left and every “lower/design” instruction to the right. Preserve all source aesthetics.
- `design-only`: use the entire canvas for the architectural sketch transformation; the photograph is an invisible reference.
- `wallpaper-pack`: full-design phone, iPad, desktop, and watch outputs, with explicitly resolved device sizes and `linked` or `independent` relationship.
- Never add a header, footer, third band, inset panel, or grid to comparison outputs.
- A directory means batch intent. Inventory supported raster files recursively in stable order, report the count, resolve shared settings once, and account for every source's successes and failures.

## Prompt assembly and generation

Concatenate the complete verbatim Chinese source brief, a short delivery preamble, exactly one selected mode contract, exactly one text contract, and only the user's explicit non-style requirements. Delivery additions change orientation, dimensions, visible source, and text settings only. Do not append an unrelated palette, aesthetic theory, slogan, or fixed title.

Resolve `prompt`, `exact`, or `none` for text. For `prompt`, write minimal source-grounded editorial words or annotations in the resolved locale. For `exact`, preserve the user's copy verbatim. For `none`, omit all letters, numbers, labels, logos, and pseudo-text.

Prefer the built-in image route. Generate each distinct output as one complete canvas from its original photograph. Do not stylise an intermediate result a second time. Never substitute deterministic vector or programmatic drawings for image generation. `scripts/compose_panel.py` is only for exact raster sizing, pixel-preserving composition, and read-only audits. If a compatible image route is unavailable, report the missing capability without exposing credentials.

For linked wallpapers, create an anchor from the original source, then independently recompose remaining devices with the original source and anchor; preserve the style without re-stylising the anchor. Independent wallpapers use only their original source.

## Acceptance and delivery

Inspect every result at full and thumbnail size. Verify source identity, natural photographic texture, correct dimensions and direction, and an exact 50:50 split in paired modes. The designed region must distil the identifiable subject and spatial relationships into relaxed architectural perspective lines, a few geometric guides, selective colour and shadow blocks, and extensive purposeful whitespace. It must not copy the full scene, densely fill the page, use heavy outlines, or resemble photorealistic rendering, cartoons, or 3D.

Verify selected text and locale; reject watermarks, UI, extra bands, and second-pass artefacts. Clean AI metadata with the available metadata-cleaning skill before final delivery and verify the cleaned files.

Write collision-safe PNGs flat in one fresh task directory under `~/Desktop/xxd/xxd-panel-120/` or the user's explicit root. Do not create source/mode/size subdirectories or an automatic contact sheet.

## References

Before delivery or publication, clean the final images using the available `xxd-strip-ai-meta` workflow and verify the supported provenance metadata is removed. Preserve pixels and colour profiles during cleanup. This is metadata hygiene, not a claim that the artwork was not AI-generated.

- `references/original-prompt/zh-CN.md`: canonical runtime source.
- `references/original-prompt/README.md`: faithful reading translations.
- `references/runtime-preferences.md`: safe delivery preference reuse; read when settings remain unresolved.
- `references/xxd-panel-120-prompt.zh-CN.md` and `.en.md`: delivery adapters.
