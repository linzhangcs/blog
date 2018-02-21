---
title: Pulse Sensor Amped
subtitle:
date: 2018-02-19
author: Lin Zhang
layout: post
comments: true
category: tangibleInteraction
---
## Pulse Sensor
#### How does it work?

We are all very familiar with measuring heart rate manually - just think of doctor visits where the doctor or nurse listen to our pulse and count heart beats per minute. This method works because the expansion and contraction of blood vessel when blood enters and leaves the heart.

How does a pulse sensor measure heart rate? It is uses a different method called photoplethysmography (or PPG). It is based on the fact oxygenated and de-oxygenated blood have different optical properties. By detecting a change in the absorbance or reflectance of light, we can measure pulse. The pulse sensor flashes one or two green LEDs onto the skin, and a light sensor measures the green light absorption. This is the basic idea of how optical pulse sensors work.

![pulse sensor image]({{ site.baseurl }}/img/tangible/PPG-diagram-optical-heart.jpg)

## Description of Pulse Sensor Amped

The pulse sensor amped measures heart-rate based on PPG. It is an easy-to-use version of pulse sensor for Arduino. It makes incorporating live heart-rate data into projects straightforward. The kit comes with finger strap and ear clip. That provides ways to place the sensor and measure heart rate. We could use finger strap or attach ear clip, and then plug the sensor into Arduino. It also works with either a 3V or 5V Arduino.
![finger reading](https://github.com/WorldFamousElectronics/PulseSensor_Amped_Arduino/raw/master/pics/finger.jpg)

![earlobe reading](https://github.com/WorldFamousElectronics/PulseSensor_Amped_Arduino/raw/master/pics/earclip.jpg)

This sensor combines an optical heart rate sensor with amplification and noise cancellation circuitry. The improvements make the heart rate reading faster and more reliable. See sensor schematic:

![sensor schematic]({{ site.baseurl }}/img/tangible/schematic_sensor.png)

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

There are different types of projects that can incorporate live heart rate as part of its interactivity, such as wearables fitness tracker, meditation trainer, and sound and light installation.

<!-- [apple Watch](https://support.apple.com/en-us/HT204666)
[Playground](https://github.com/WorldFamousElectronics/PulseSensorPlayground)
[Fall In Line](https://www.sparkfun.com/videos#all/ZgtvEsSGMJ8/124) -->


## Strengths and Weaknesses

## Example Circuit Schematic

## Example Microcontroller Code

## Citations

Links and images found on [Adafruit Pulse Sensor Amped](https://www.adafruit.com/product/1093)
Data Sheet found [here](https://media.digikey.com/pdf/Data%20Sheets/Pulse%20PDFs/PulseSensorAmpedGettingStartedGuide.pdf)
