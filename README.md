# Picons

Custom icons for IoT devices, true to the pixel.

SVG is the source of truth. Icons are sharp and pixel-aligned (`1` screen px ≈ `1` design point), then codegen’d into React, Rust, C, and similar for embedded graphics. Browse and pick icons later at [picons.dev](https://picons.dev).

## Packs

| Pack | Path | Status |
|------|------|--------|
| Environment measurement | [`packs/environment`](packs/environment) | Scaffold — SVG sources pending |

Each pack keeps hand-authored SVGs under `svg/{20,24,28,32}/` (default **24**) and leaves room for generated targets under `generated/{react,rust,c}/`. See the pack README for naming and drop-in rules.
