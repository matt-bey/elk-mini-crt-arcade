# Hardware — Mini CRT Arcade Box

## Bill of Materials

| Component | Details |
|-----------|---------|
| Raspberry Pi Zero W | Main board |
| Waveshare 3.5inch HDMI LCD (E) | 640×480 capacitive touch IPS, 3.5mm audio; powered via pogo pins from Pi 5V (USB-C also supported) |
| PAM8403 amplifier board | 5V, 2×3W, volume pot |
| Gikfun 2" 4Ω 3W speakers | Full range (×2) |
| 3.5mm stereo to bare wire connector | Audio in to PAM8403 |
| 22 AWG stranded silicone wire | General wiring |
| Mini-HDMI to HDMI cable | Pi Zero W to display |
| USB NES-style controller | Player input |
| 5V/2.1A power supply | v1 only — replaced by battery in v2 |
| TP4056 + 5V/2A boost combo board | USB-C charge input, Output +/− pads, K point for power button (DWEII or equivalent) |
| Samsung 30Q 18650 cell | 3000mAh, 15A continuous. Source from a reputable vendor (e.g. 18650batterystore.com) — counterfeits are common on general marketplaces. |
| 18650 battery holder (single cell) | Wire leads to BAT+/BAT− on combo board. SparkFun PRT-12899 fits. |
| Momentary push button | Wires to K point — toggles boost output on/off |
| Power distribution block, 2-pole 6-position Dupont | Teansic 2×6 or equivalent. One row 5V, one row GND. Distributes to Pi GPIO, PAM8403, cap. |
| Electrolytic capacitor | 100µF on supply rail; 1000µF as a fallback if reboots occur under load |
| Velleman VMP400 TFT | Optional alternate display (SPI, 320×240) — kept as a reference; HDMI path is the default |
| USB audio DAC | Optional — useful during early bring-up before the HDMI display's 3.5mm jack is wired |

## Power Budget

| Component | Draw |
|-----------|------|
| Pi Zero W under load | ~400mA |
| HDMI display backlight | ~200mA |
| PAM8403 at moderate volume | ~200–300mA |
| USB controller | ~100mA |
| **Total** | **~900–1000mA** |

Supply: 5V/2.1A = 10.5W. Comfortable headroom at typical use.
