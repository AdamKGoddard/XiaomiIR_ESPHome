XiaomiIR_ESPHome
Custom ESPHome Firmware for the Xiaomi Mijia Universal IR Remote Controller `MJYKQ01CM`.  
**NOTE:** This is not compatible with Marvell model `NDZ-08-GA`.

Thank you to Paul Nicholls for his work on adapting the Arduino ESP32 Core to the Single Core Processor variant used by Xiaomi, and his resulting Linp Doorbell ESPHome integration.

https://github.com/pauln/arduino-esp32/wiki

https://github.com/pauln/esphome-linp-doorbell-g03

** 2023/09/06 - Upgraded to ESP-IDF to bypass compilation issues with the old framework and newer ESPHome configs, please update your pre-script files and YAML code accordingly

** 2025/03/01 - Pre Script and remote_transmitter_esp32.cpp are no longer required as this issue was fixed upstream in the IR remote libraries.

Flashing Instructions:
 - Load yaml file to ESPHome and adjust parameters to suit your setup.
 ##### No longer required!! - Upload remote_transmitter_esp32.cpp and pre_extra_script.py to your home assistant files in "/config/esphome/" #####
 - Validate yaml and ensure no errors.
 - Manually compile and download binary firmware file.
 - Open the unit and solder GND, RX0 and TX0 to your USB-TTL Serial adapter.
 - Press and hold Reset whilst plugging in MicroUSB power.
 - Flash the unit with the ESPHome Flasher software.

Tested compiling against ESPHome 2025.2.1 under Home Assistant 2025.2.5.
