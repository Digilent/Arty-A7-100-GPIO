# Arty-A7-100-GPIO
Created for Vivado 2016.4

This project is an introductory level demonstration project for the Arty A7-100's LEDs, switches, buttons, and USB-UART bridge.

in order to open the project in Vivado, follow the [Using Digilent Github Demo Projects Tutorial](https://reference.digilentinc.com/learn/programmable-logic/tutorials/github-demos/start). This is an HDL design project, and as such does not support Vivado SDK. Select the tutorial options appropriate for a Vivado-only design.

In order to receive messages from the demo over the USB-UART bridge, use a terminal program such as Tera Term.The UART interface should be configured to 9600 baud, 8 data bits, no parity bit, and 1 stop bit.

Each of the 4 switches on the Arty A7-100 are tied to the corresponding LED. For instance, if Switch 0 is switched to the "down" (off) position, LED 0 will be off as well.

The Arty A7-100's four tri-color LEDs will cycle colors with no interruption from other I/O.

On startup, the demo will transmit "ARTY GPIO/UART DEMO" over the USB-UART bridge. Whenever any of the four push-buttons is pressed, the demo transmits "Button press detected!".