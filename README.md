A LiPo battery charger based on the Adafruit MicroLipo, with added reverse polarity protection.

Features:
* Based on a proven and tested design by Adafruit.
* Includes an additional output port for batteries using a JST-PZ connector.
* Reverse polarity protection for the charging IC, useful if you're dealing with batteries with the wires switched around (such as a Dualshock 4 battery).

Note that you MUST NOT try to use both output ports at once, this board is only designed to charge one battery at a time.

The original Adafruit design can be found [here](https://learn.adafruit.com/adafruit-microlipo-and-minilipo-battery-chargers/downloads).

Included in this repository are the KiCAD files for this design. If you're only interested in having the board manufactured, gerbers are available under 'releases'.

Parts List:
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

For more information, take a look at [my blog post](https://qubitsandbytes.co.uk/post/lipo-charger-with-reverse-polarity-protection/).

## Images
KiCAD render:

![KiCAD render](render.webp?raw=true "KiCAD render of the board")

## KiCAD
The files in this project were created using KiCAD 6, which introduced a new file format not compatible with older versions. Ensure you are using KiCAD 6 if you wish to open the files.
