# Arduino-optical-mouse https://www.thingiverse.com/thing:7266629
Arduino optical mouse learning project, CH32V00x MCU, 284x76 pixel 1.9" TFT. Optical Arduino Mouse Project

This project repurposes the sensor from a (wireless) mouse inside a custom 3D-printed enclosure. While the demonstration uses a CH32V003 Arduino-compatible microcontroller, the code can be adapted with minimal effort to run on most other MCU platforms.

Assembly Instructions:

Prepare the Sensor Module: Disassemble the mouse. Carefully remove the components surrounding the PAW3205 optical sensor chip. Using a jigsaw, cut the PCB around the sensor, aiming for a final size of approximately 18 x 43mm. Preserve only the essential components: the two capacitors connected to pins 6, 7, and 8, as well as the LED and its current-limiting resistor. 

Reassemble the Optical Unit: Position the optical assembly (lens) and the trimmed sensor PCB back into the original mouse housing in their correct alignment. Secure them together with adhesive. Important: Ensure no glue obstructs the optical path between the lens , LED and the sensor. Surfaces act as mirror.

Electrical Connections: Solder wires (for example, from a recycled USB cable) to the PAW3205 sensor pins:

Pin 3: SDIO (Data)

Pin 4: SCLK (Clock)

Pin 6: GND

Pin 7: VCC (3.3V or 5V, depending on your module)
Connect these wires to the corresponding pins on your Arduino board.

Software Demo:

The provided demonstration code displays a moving cursor on a TFT screen. By moving the physical mouse, you control the cursor position. A pushbutton (integrated or added) allows you to select on-screen functions, creating a simple graphical interface for your projects.

https://www.thingiverse.com/thing:7266629

https://github.com/boda-akos/CH32V003-ST7789-Virtual-Keyboard-with-PAW3205-Optical-Mouse
