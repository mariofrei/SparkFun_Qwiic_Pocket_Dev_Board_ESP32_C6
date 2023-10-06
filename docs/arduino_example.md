---
icon: simple/arduino
---

Now that we've installed the espressif boards package in Arduino, it's time to upload our first sketch to make sure everything is working properly.

## Example 1 - Blink 

This basic example makes sure the board package installed correctly and the board accepts programming properly to blink the blue STAT LED on the board every second. Open the example in Arduino by navigating to File > Examples > Basics > 01-Blink.

!!! note "USB CDC On Boot Settings"

    Take note of the option labeled "USB CDC on Boot" when selecting the Board from the Tools menu. This option sets the serial outputs and defines their label for use in code. The SparkFun variants default to Enable USB CDC on boot which sets both <code>Serial</code> and <code>Serial0</code> as available serial ports. In this configuration, <code>Serial</code> corresponds to the direct USB/Serial converter on the chip (and the USB-C interface) and <code>Serial0</code> corresponds to the UART0 bus (default pins are 16 and 17).

    With either setting, <code>Serial1</code> is available and refers to the UART1 bus (default pins are 4 and 5).

Select the board (SparkFun Qwiic Pocket Development Board - ESP32-C6) and Port and click "Upload". After uploading you should see the STAT LED on the board blinking every second.