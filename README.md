# CAN-Reactive-LEDS
Custom ESP32 based lighting for my  car, with CAN bus connectivity

This repository specifically is for the OBD2 dongle firmware. 
The overall system is composed of a master device connected to the CAN bus, and slave devices attached to addressable LED lighting elements. The master device generates the LED animations desired, using data from the CAN bus to trigger or modify the lighting patterns. The master transmits the animation frames to the slave devices using ESP-NOW at regular intervals. The slave deivces rceive the animation frames, then display them onto the LED lighting elements.
