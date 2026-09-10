---
name: xxd-panel-120
description: "Create XXD Panel 120 raster artwork from a source photograph as an architectural concept perspective sketch: relaxed freehand lines, sparse geometric guides, selective colour blocks, geometric shadows, and extensive whitespace. Use when the user invokes xxd-panel-120 or requests this architectural concept-sketch editorial transformation. Supports isolated image or directory inputs, strict 50:50 comparisons, design-only work, and wallpapers."
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
