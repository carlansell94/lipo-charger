LiPo battery chargers based on the Adafruit MicroLipo, with added reverse polarity protection.

Features:
* Based on a proven and tested design by Adafruit.
* Includes JST-PH and JST-ZH footprints to support a wider range of battery connectors.
* v1 supports 1x JST-PH port and 1x JST-ZH port, while v2 has 2 of each port - the second pair on the rear swapping the polarity of the connector.
* Includes an additional output port for batteries using a JST-PZ connector.
* Reverse polarity protection for the charging IC, useful if you're dealing with batteries with the wires switched around (such as a Dualshock 4 battery).
* v2 features a USB type C port for power input, and a surface-mount switch to choose between fast and slow charging modes (v1 required soldering a resistor).

Note that you MUST NOT try to use multiple ports at once, this board is only designed to charge one battery at a time.

The original Adafruit design can be found [here](https://learn.adafruit.com/adafruit-microlipo-and-minilipo-battery-chargers/downloads).

Included in this repository are the KiCAD files for both designs. If you're only interested in having them manufactured, gerbers are available under 'releases'.

## Parts Lists
v1 Parts List:
| Component                       |Qty| Symbol(s) |
| ------------------------------- | - | --------- |
| USB Micro B Port                | 1 | X1        |
| MCP73831/2 SOT23 Charging IC    | 1 | U1        |
| 0805 10uF Capacitor             | 2 | C1,C2     |
| 0805 470Ω Resistor              | 2 | R1,R2     |
| 0805 10kΩ Resistor              | 1 | R3        |
| 0805 2.49kΩ Resistor            | 1 | R4        |
| 0805 100kΩ Resistor             | 1 | R5        |
| 0805 1MΩ Resistor               | 1 | R6        |
| ZXMP3A13FTA P Channel MOSFET    | 1 | Q1        |
| MMBT3904,215 BJT NPN Transistor | 1 | Q2        |
| 0805 LED (Colours Optional)     | 2 | LED1,LED2 |
| JST-PH Connector                | 1 | CN1       |
| JST-PZ Connector                | 1 | CN2       | (Optional)
| 0805 0Ω Resistor                | 1 | SJ1       | (Optional)

v2 Parts List:
| Component                       |Qty| Symbol(s) |
| ------------------------------- | - | --------- |
| 16-pin USB Type C Port          | 1 | J1        |
| MCP73831/2 SOT23 Charging IC    | 1 | U1        |
| 0805 10uF Capacitor             | 2 | C1,C2     |
| 0805 470Ω Resistor              | 2 | R1,R2     |
| 0805 10kΩ Resistor              | 1 | R3        |
| 0805 2kΩ Resistor               | 1 | R4        |
| 0805 100kΩ Resistor             | 1 | R5        |
| 0805 1MΩ Resistor               | 1 | R6        |
| 0805 5.1kΩ Resistor             | 2 | R7,R8     | (Optional)
| ZXMP3A13FTA P Channel MOSFET    | 1 | Q1        |
| MMBT3904,215 BJT NPN Transistor | 1 | Q2        |
| 0805 LED (Colours Optional)     | 2 | LED1,LED2 |
| JST-PH Connector                | 2 | CN1,CN4   |
| JST-PZ Connector                | 1 | CN2,CN3   | (Optional)
| PCM12SMTR Slide Switch          | 1 | SW1       | (Optional)

For more information on the v1 (micro USB) board, take a look at [my blog post](https://qubitsandbytes.co.uk/lipo-charger-with-reverse-polarity-protection/).

For more information on the v2 (USB type C) board, take a look at [this post](https://qubitsandbytes.co.uk/building-a-better-lipo-battery-charger/).

## Images
v1 KiCAD render:

![v1 KiCAD render](render.webp?raw=true "KiCAD render of the board")

v2 KiCAD render:
![v2 KiCAD render](render.webp?raw=true "KiCAD render of the v2 board")

## KiCAD
The files in this project were created using KiCAD. To open these files, make sure you're using KiCAD v9 or above.
