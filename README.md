# glowbuck
Glowbuck is a voltage converter and control board that allows you to power addressable LED strips with USB-C PD.

Together with [Firefly Luciferin](https://github.com/sblantipodi/firefly_luciferin), you can create your own ambilight that connects via USB-C to your computer and draws power from a USB-C PD power supply. Glowbuck is in no way associated with the linked project.

<img width="1632" height="1178" alt="image" src="https://github.com/user-attachments/assets/959389fa-ffcf-42b5-b2e9-d20aae3e01f9" />
The left USB-C socket is used for data. The right socket shall be connected to a suitable USB-C PD supply. The spring-loaded connection terminal allows easy and safe connection to a 5 V addressable LED strip with, for example, SK6812 or WS2812B. The output current is measured with a 2 mOhm shunt. A shunt amplifier allows the integrated ESP32 S3 to measure the current flow and shut down the buck regulator when an unusually large current is detected.

## Quick Facts:
- Output: 5 V @ 10 A
- Input: 20 V @ 3 A. Via I2C, the microcontroller can reconfigure the PD controller and negotiate other voltage and current requirements for the input.
- Microcontroller: ESP32 S3
- Output current measurement with an integrated shunt

## Warning and Disclaimer

**Warning**: This project is in a alpha state and the hardware has not yet been tested.

This project is provided "as is" without warranty of any kind, either expressed or implied. The author makes no guarantees regarding the functionality, reliability, or suitability of this project for any particular purpose.
By using this project, you acknowledge and agree that:
- No liability is accepted for any damages, losses, or issues arising from the use or inability to use this project
- There is no guarantee that this project will work as intended or work at all
- The author shall not be held responsible for any direct, indirect, incidental, or consequential damages
