# Environment measurement pack

SVG sources for environment / IoT measurement icons (CO₂, TVOC/FAVOC, VWC, humidity, PM1, PM2.5, PM10, air, water, and related).

## Layout

```
environment/
  svg/          # source of truth — hand-authored SVGs
    20/
    24/         # default optical size
    28/
    32/
  generated/    # codegen output (do not hand-edit)
    react/
    rust/
    c/
```

## Sizes

| Size | Folder     | Notes                          |
|------|------------|--------------------------------|
| 20   | `svg/20/`  | Compact UI                     |
| 24   | `svg/24/`  | **Default** viewBox / optical  |
| 28   | `svg/28/`  | Mid                            |
| 32   | `svg/32/`  | Larger / display               |

Smaller sizes may be added later. Design for sharp, pixel-aligned paths (`1` screen px ≈ `1` design point).

## Naming

- One file per icon, **kebab-case**, matching the measurement or concept.
- Same basename across every size folder (e.g. `co2.svg` in `20/`, `24/`, `28/`, and `32/`).
- Prefer ASCII identifiers: `co2`, `tvoc`, `vwc`, `humidity`, `pm1`, `pm2-5`, `pm10`, `air`, `water`.
- No size or pack prefix in the filename — size is the folder; pack is the path.

## Where to put SVGs

Drop finished artwork into the matching size folder under `svg/`. Leave `generated/` empty until a codegen step writes React, Rust, or C artefacts there.
