---
title: Pulse Sensor Amped
subtitle:
date: 2018-02-19
author: Lin Zhang
layout: post
comments: true
category: tangibleInteraction
---

## Description

The pulse sensor amped is an easy-to-use heart-rate sensor for Arduino. It makes incorporating live heart-rate data into projects straightforward. Use velcro finger strap for measuring heart rate or attach ear clip for measuring earlobe heart rate, and then plug the sensor into Arduino without soldering. It works with either a 3V or 5V Arduino.
![finger reading](https://github.com/WorldFamousElectronics/PulseSensor_Amped_Arduino/raw/master/pics/finger.jpg)

![earlobe reading](https://github.com/WorldFamousElectronics/PulseSensor_Amped_Arduino/raw/master/pics/earclip.jpg)

This sensor combines an optical heart rate sensor with amplification and noise cancellation circuitry. The improvements make the heart rate reading faster and more reliable.

Also, the Pulse Sensor creators made an accompany [Processing visualization software](https://github.com/WorldFamousElectronics/PulseSensor_Amped_Processing_Visualizer) for this hardware. Using the visualization software, one can instantly see output of the sensor and also use it for troubleshooting.

![sensor](https://cdn-shop.adafruit.com/970x728/1093-06.jpg)
![sensor](https://cdn-shop.adafruit.com/970x728/1093-04.jpg)
![sensor](https://cdn-shop.adafruit.com/970x728/1093-07.jpg)
![sensor](https://cdn-shop.adafruit.com/970x728/1093-05.jpg)

## Data Sheet

The full data sheet can be found on the [pulse sensor official website](https://pulsesensor.com/pages/open-hardware). Here are some of stats about this sensor:

  - Diameter = 0.625" (~16mm)

  - Overall thickness = 0.125" (~3mm)

  - Cable length = 24" (~609mm)

  - Voltage = 3V to 5V

  - Current consumption = ~4mA at 5V

This sensor uses Ambient light Sensor ([APDS-9008](http://www.avagotech.com/docs/AV02-1169EN)) from Avago. Also green bright reverse mount LED from Kingbright ([AM2520ZGC09](http://www.kingbrightusa.com/images/catalog/SPEC/am2520zgc09.pdf)), added diode protection in case when it is plugged in backwards. Active filter and amplifier to change the pulse waveform.

***Reading Before added filter and amplifier:***
![before reading](https://cdn.shopify.com/s/files/1/0100/6632/files/pulseWaveformOldVersion_large.jpg?619)
***After:***
![after reading](https://cdn.shopify.com/s/files/1/0100/6632/files/pulseWaveformAmpdVersion_large.jpg?619)
## Description of Example Uses

There are different types of projects that can incorporate live heart rate into, such as exercise, meditation, and light installation.

[Fall In Line](https://www.sparkfun.com/videos#all/ZgtvEsSGMJ8/124)


## Strengths and Weaknesses

## Example Circuit Schematic

## Example Microcontroller Code

## Citations

Links and images found on [Adafruit Pulse Sensor Amped](https://www.adafruit.com/product/1093)
Data Sheet found [here](https://media.digikey.com/pdf/Data%20Sheets/Pulse%20PDFs/PulseSensorAmpedGettingStartedGuide.pdf)
