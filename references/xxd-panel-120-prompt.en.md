# Panel 120 delivery adapter

Read the complete `original-prompt/zh-CN.md` as the sole creative authority. Append only resolved delivery variables.

- `top-bottom`: two full-width regions, photograph above and design below, strict 50:50.
- `left-right`: override the source's 3:4 top/bottom delivery only. Map “upper/photo” to left and “lower/design” to right, each 50% of the full height canvas. Keep all architectural sketch instructions unchanged.
- `design-only`: use the full canvas for the designed transformation; source is an invisible reference.
- `wallpaper-pack`: full-design outputs for phone, iPad, desktop, and watch; resolve device dimensions and `linked` or `independent`.
- Sizes: `auto`, `source`, standard/custom ratios, or exact pixels. Selected size overrides the source's default 3:4.
- Text: `prompt`, `exact`, `none`; resolve locale. No fixed slogan or invented source facts.
- One original source per independent generation; no third band, inset, or second stylisation.
