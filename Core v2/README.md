## OpenShock Core

v2.0

![image](https://github.com/nullstalgia/OpenShock-Hardware/assets/20761757/5d1454d3-cc5c-4eb4-9a53-95ad6c591f27)

![image](https://github.com/nullstalgia/OpenShock-Hardware/assets/20761757/1c5dca45-9f8a-4416-82b6-406104802f19)

#### Specs:
- ESP32-S3-WROOM-1
- USB-C
- In-built E-Stop button and AUX E-Stop port (3.5mm TRS jack)
- No USB-UART, uses built-in USB on ESP32-S3
- 3.3v regulator
- More compact than v1
- Footprint 40mm x 56mm

#### Important ordering information:
- PCB Thickness: 1.0mm
- 4 Layers
- WS2812B-Minis may incur an extra component baking fee
- Impedence Controlled for JLCPCB's `JLC04101H-7628` stackup
- Edge Rails in source files are not attached, and are not included in JLC gerbers

#### Redlines (v2.0):
- R1 (high side pullup for RF TX level-shifting) was causing unwanted RF signals when IO1 was Hi-Z/Input Enabled.
- EN pin missing debounce capacitor.