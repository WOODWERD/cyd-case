# WOODWERD CYD Case: a printed housing for the Cheap Yellow Display

_An open-hardware project from [WOODWERD LLC](https://woodwerd.com), a design group in Austin, Texas._

A split, screw-together 3D-printed case for the ESP32-2432S028R "Cheap Yellow Display" (CYD), USB-C variant. It's one case for every WOODWERD CYD build: the housing fits the board, not a particular firmware, so each project's firmware drops into the same enclosure.

![Case](docs/case_iso.png)

- Three printed parts, four M3 screws and four heat-set inserts. No supports, no glue.
- Only the USB-C port is exposed. The cable seats properly, sized to the USB Type-C spec.
- A clear light pipe carries the board's light sensor through the lid.
- STL for printing, STEP for editing.

**Build one:** [Build guide](docs/BUILD.md) covers buying, printing, inserts and assembly. The parts list is [BOM.csv](BOM.csv).

## Which firmware fits

| Project | Housing | Notes |
|---|---|---|
| [Flow Ctrl](https://github.com/WOODWERD/cyd-flow-ctrl): Wispr Flow push-to-talk button | v2 | Landscape, lies flat on the desk. |
| [Media Ctrl](https://github.com/WOODWERD/cyd-media-ctrl): iPad media remote | v2 | Portrait. Lean it against something for now; a dedicated portrait stand is planned. |
| Any other CYD firmware for the USB-C board | v2 | The case covers micro-USB, microSD, RST/BOOT and the JST headers. If your firmware needs those, wait for v3. |

## Housings

| Version | Status | What's different |
|---|---|---|
| [**v2**](housings/v2/README.md) | **Released**, printed and test-fitted | USB-C only, light pipe. 54.6 × 90.6 × 16.1 mm. |
| v3 | In development | Adds a microSD slot and printed RESET / BOOT flexure buttons. |
| v4 | In development | Longer body with a LiPo battery bay, USB-C charging and a slide switch. |
| Portrait stand | Planned | A standing housing for Media Ctrl. |

New versions are added as folders under `housings/`. Released ones are never changed in place.

## Shared hardware (every housing)

| Qty | Part | Spec |
|---|---|---|
| 1 | Cheap Yellow Display, **USB-C / 2-USB variant** | ESP32-2432S028R with a USB-C port |
| 1 | USB-C cable, data | USB-C → USB-A recommended (some boards lack CC resistors) |
| 4 | Flat-head screw | **M3 × 14 mm**, 90° countersunk, hex socket, DIN 7991 / ISO 10642. Not M3 × 16. |
| 4 | Heat-set insert | **M3 brass, 4 mm long, OD 4.0–4.2 mm** ("M3 × L4"). Not the 5.7 mm ones. |

Plus the printed parts for your housing version. The full fastener sheet, with a section drawing, is [housings/v2/Fastener_Spec.pdf](housings/v2/Fastener_Spec.pdf).

## License

MIT © 2026 WOODWERD LLC. See [LICENSE](LICENSE) and [THIRD_PARTY_NOTICES.md](THIRD_PARTY_NOTICES.md).
