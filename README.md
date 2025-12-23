# Tasmota-Geiger-Counter
Using a generic Tasmota with some Berry code as a Geiger Counter

Take an ESP32 and install a generic Tasmota (currently used version 15.2.0), Upload a piece of Tasmota-App and you have the counter and saver for Geiger data, to which you communicate solely via WiFi.   

You need the Geiger hardware separately, i.e. the tube, the High-Voltage generator, and the pulse-former, so that you can deliver a logic pulse (3.3 Volt) to a pin of the ESP32 (currently using pin GPIO22).

(Actually, you don't need Geiger hardware - anything which produces logic pulses of 3.3 V can be used with the same data storage and data transfer abilities).

The Tasmota main page does show CPM (Counts per Minute) and CPS (Counts per Second). These data will also be saved on the ESP's local Flash. The available Flash sizes on an ESP32 range from 4 MB up to 64 MB, and Espressif is even preparing 128 MB. This will allow even years of storage onboard the ESP32.

This Tasmota-Geiger-Counter App can be used as-is with any system, but its main purpose is to be used with the big Geiger Counter software *"GeigerLog"*. This also is Open-Source software.

This repository has the Tasmota-App code 'geiger.tapp'. For the full GeigerLog code see https://sourceforge.net/projects/geigerlog/ . The latest pre-release can be found here: https://sourceforge.net/p/geigerlog/discussion/devel2/
Latest version as of now is: GeigerLog Version 2.2pre01

Note: while Tasmota can even be used on a ESP8266, this old device CANNOT be used for the Tasmota-Geiger-Counter!
