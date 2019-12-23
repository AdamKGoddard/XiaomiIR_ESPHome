# XiaomiIR_ESPHome
Custom ESPHome Firmware for the Xiaomi Mijia Universal IR Remote Controller

Thank you to Paul Nicholls for his work on adapting the Arduino ESP32 Core to the Single Core Processor variant used by Xiaomi, and his resulting Linp Doorbell ESPHome integration.

https://github.com/pauln/arduino-esp32/wiki

https://github.com/pauln/esphome-linp-doorbell-g03

Flashing Instructions:
 - Load yaml file to ESPHome and adjust parameters to suit your setup.
 - Validate yaml and ensure no errors.
 - Manually compile and download binary firmware file.
 - Open the unit and solder GND, RX0 and TX0 to your USB-TTL Serial adapter.
 - Press and hold Reset whilst plugging in MicroUSB power.
 - Flash the unit with the ESPHome Flasher software.

