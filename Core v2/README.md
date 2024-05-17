## OpenShock Core V2.2L

#### Now only two layers!

![2024-05-16--23-05-26-kicad](https://github.com/OpenShock/Hardware/assets/20761757/16b40d7f-5c7c-46bd-8691-fa044252268a)

![wF1W8qGIAY](https://github.com/OpenShock/Hardware/assets/20761757/860ca29c-f311-4dcb-a9d3-c8d7d4cef2a4)

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
- **2** Layers
- Impedence Controlled for JLCPCB's 1.0mm stackup
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

#### Redlines (v2.2):
- To be discovered.