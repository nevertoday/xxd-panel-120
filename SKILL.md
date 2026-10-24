---
name: xxd-panel-120
description: "XXD Panel 120｜Architectural Concept Sketch Chronicle: turns the core form and spatial relationships of a photo into an architectural concept perspective sketch — loose, restrained free-hand perspective lines with some construction, extension and geometric guide lines left in, colour laid lightly on only a few key parts, a few geometric shadow blocks for volume, most background removed, a smaller subject moved, cropped or rescaled to rescue a weak photo, very large whitespace, a clean sketch palette of two to four photo colours (off-white, greys, soft green, pale wood, blue-grey) with one brighter accent, and a few quiet notes in any language. Outputs PNG top-bottom or left-right comparisons, design-only images, or phone/tablet/desktop/watch wallpapers, from one photo or a folder. Use when the user invokes xxd-panel-120 or asks for architectural concept sketch or perspective line drawing from a photo."
---

# XXD Panel 120

Create finished PNG artwork from the current user-supplied photograph or image directory. Read `references/original-prompt/zh-CN.md` completely immediately before every generation. That Chinese source brief is the sole creative and aesthetic authority; never summarise, translate, blend, or replace it with this file, a README, a sample, or another Panel.

Read `references/soldier-runtime.md` completely immediately before building every generation request. It is the sole family runtime contract for parameters, preference reuse, directory batches, preflight, prompt assembly, bitmap execution, output isolation, and acceptance. This Skill must not write a second art direction or a second runtime.

## Panel-specific overlay

Verify selected text and locale; reject watermarks, UI, extra bands, and second-pass artefacts. Clean AI metadata with the available metadata-cleaning skill before final delivery and verify the cleaned files.

Write collision-safe PNGs flat in one fresh task directory under `~/Desktop/xxd/xxd-panel-120/` or the user's explicit root. Do not create source/mode/size subdirectories or an automatic contact sheet.

These overlay rules add to `references/soldier-runtime.md`. They never replace the source brief or the family runtime contract.

Write every selected final PNG directly inside one fresh task directory under `~/Desktop/xxd/xxd-panel-120/` (or the explicit `--out` root). Use collision-safe filenames; do not create source, mode, or size subdirectories and do not generate an automatic contact sheet.

## References

- `references/soldier-runtime.md` — family runtime contract used at generation time
- `references/original-prompt/zh-CN.md` — canonical source brief used at runtime
- `references/original-prompt/README.md` — translation index and authority note
- `references/runtime-preferences.md` — safe delivery-preference reuse
- `references/sample-workflow.md` — sample-artwork maintenance only; never a runtime prerequisite
- `references/xxd-panel-120-prompt.zh-CN.md` and `.en.md` — delivery adapter notes matching the family runtime blocks
