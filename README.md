# ESP-OpenTherm
OpenTherm compatible hardware for home automation. It includes all the hardware needed for OpenTherm communication.
Based on the ESP8266, uses the ESP-07S module with external WiFi antenna. Simply connect to OT terminals and power.

You are free to choose the software as there are a few possibilities here:
- Tasmota, more info here: https://tasmota.github.io/docs/OpenTherm/
- build your own local webserver on the ESP using this great library: https://github.com/ihormelnyk/opentherm_library/


For the library use GPIO 14 for IN pin and GPIO 12 as the OUT pin.
For Tasmota configure D6 GPIO 12 as OpenTherm TX (203) and D5 GPIO 14 as OpenTherm RX (202).


Version 1.2 of the PCB adds on the back a solder bridge jumper to select for IN (read/RX) pin GPIO 14 or GPIO 4 and for OUT (write/TX) GPIO 12 or GPIO 5 as requested by some ESPHome users.

For ESPHome we have tested with great success the component by khenderick available here: https://github.com/khenderick/esphome-opentherm
