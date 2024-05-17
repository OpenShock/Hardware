## OpenShock Core V2.1


![2024-05-16--22-54-31-kicad](https://github.com/OpenShock/Hardware/assets/20761757/aa46de72-ddff-41f8-bfed-6b0960d3e07f)

![qLOPlbv9ng](https://github.com/OpenShock/Hardware/assets/20761757/e706d793-6bf8-43be-b28a-68b780d25b00)

#### Specs:
- ESP32-S3-WROOM-1
- USB-C
- In-built E-Stop button and AUX E-Stop port (3.5mm TRS jack)
- No USB-UART, uses built-in USB on ESP32-S3
- 3.3v regulator
- More compact than v1
- Footprint 40mm x 56mm

#### Important ordering information:
- PCB Thickness: **1.0mm**
- **4** Layers
- Impedence Controlled for JLCPCB's `JLC04101H-7628` stackup
- Edge Rails in source files are not attached, and are not included in JLC gerbers
- **Standard PCBA** only (As of writing, Economy PCBA is unsupported for the ESP32-S3 modules due to solder reflow curve requirements)

JLCPCB may contact you about a couple of things:

- WS2812B-Minis may incur an extra component baking fee (~$8-10)
- Rotations of WS2812B-Mini and Antenna. Ensure that they match these examples:

![2024-05-16--22-49-20-firefox](https://github.com/OpenShock/Hardware/assets/20761757/bad84f53-0470-4866-86c6-6435b8a50218)

![image](https://github.com/OpenShock/Hardware/assets/20761757/bbf42ef5-77e4-412e-a156-4f9997add13c)


#### Redlines (v2.0) (Solved in v2.1+):
- R1 (high side pullup for RF TX level-shifting) was causing unwanted RF signals when IO1 was Hi-Z/Input Enabled.
- EN pin missing debounce capacitor.

#### Redlines (v2.1):
- To be discovered.