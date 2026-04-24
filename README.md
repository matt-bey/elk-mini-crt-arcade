# Mini CRT Arcade Box

**Status:** Active
**Hardware:** Raspberry Pi Zero W
**Started:** 2026

A desk-sitting retro arcade box styled to look like a miniature CRT television. Runs RetroPie on a Pi Zero W. Display and audio connect via HDMI. USB controller plugs into the side for gameplay.

## Quick Start (after fresh RetroPie flash)

```bash
# From repo root on your Mac
bash projects/mini-crt-arcade/scripts/setup.sh
```

Then reboot the Pi. See SOFTWARE.md for full details.

## Features

- Retro gaming via RetroPie — NES ROMs confirmed working; other cores available
- 3.5" HDMI display (Waveshare) at native 640×480 4:3 — no letterboxing for NES content
- Built-in stereo speakers through a PAM8403 amplifier with a front-panel volume knob
- USB controller input (NES-style)
- Swappable display path: HDMI (primary) or SPI TFT (Velleman VMP400 backup)
- Cardboard v1 enclosure; 3D-printed v2 in design (see ENCLOSURE.md)

## Docs

- [HARDWARE.md](HARDWARE.md) — bill of materials and power budget
- [SOFTWARE.md](SOFTWARE.md) — Pi setup, display/audio configuration, SSH access
- [ENCLOSURE.md](ENCLOSURE.md) — enclosure design notes and 3D-printed parts
