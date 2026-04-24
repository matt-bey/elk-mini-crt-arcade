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

## Current Status

- ✅ Pi Zero W running RetroPie with NES ROMs
- ✅ Waveshare 3.5inch HDMI LCD (E) — 640×480, HDMI audio, powered via pogo pins
- ✅ PAM8403 amplifier + 2x speakers wired and working
- ✅ Full audio chain: Pi → HDMI → display 3.5mm → PAM8403 → speakers
- ✅ v1 cardboard enclosure — prototype self-contained and working
- ✅ Velleman VMP400 TFT retained as backup display
- ✅ SD card backup taken

## Docs

- [HARDWARE.md](HARDWARE.md) — bill of materials and power budget
- [SOFTWARE.md](SOFTWARE.md) — Pi setup, display/audio configuration, SSH access
- [ENCLOSURE.md](ENCLOSURE.md) — enclosure design notes and 3D-printed parts
