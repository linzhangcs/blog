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

How does a pulse sensor measure heart rate? That utilizes a different method called photoplethysmography (or PPG). It is based on the fact oxygenated and de-oxygenated blood have different optical properties. By detecting a change in the absorbance or reflectance of light emitted onto the skin, we can measure pulse. Pulse sensors have up to two green LEDs flash onto the skin, and a light sensor measures the green light absorption and detect the peak. This is the basic idea of how optical pulse sensor work. If you have used any of the fitness tracker wearables on the market, such like [Apple Watch](https://support.apple.com/en-us/HT204666) and [Fitbit](https://www.fitbit.com/technology), you can this method in action.

![pulse sensor image]({{ site.baseurl }}/img/tangible/PPG-diagram-optical-heart.jpg)

![apple watch](https://support.apple.com/library/content/dam/edam/applecare/images/en_US/applewatch/watch-measure-sensors.png)
***Apple Watch Tech Spec***

## Description of Pulse Sensor Amped

The pulse sensor amped measures heart-rate based on PPG. It is an easy-to-use version of pulse sensor for Arduino. It makes incorporating live heart-rate data into projects straightforward. The kit comes with finger strap and ear clip. That provides ways to place the sensor and measure heart rate. We could use finger strap or attach ear clip, and then plug the sensor into Arduino. It also works with either a 3V or 5V Arduino.
![finger reading](https://github.com/WorldFamousElectronics/PulseSensor_Amped_Arduino/raw/master/pics/finger.jpg)

![earlobe reading](https://github.com/WorldFamousElectronics/PulseSensor_Amped_Arduino/raw/master/pics/earclip.jpg)

This sensor combines an optical heart rate sensor with amplification and noise cancellation circuitry. The improvements make the heart rate reading faster and more reliable. See sensor schematic:

![sensor schematic]({{ site.baseurl }}/img/tangible/schematic_sensor.png)

Also, the Pulse Sensor creators made a complementary [Processing visualization software](https://github.com/WorldFamousElectronics/PulseSensor_Amped_Processing_Visualizer) for this hardware. Using the visualization software, one can instantly see output of the sensor and also use it for troubleshooting.

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
## Sample Projects

There are different types of projects that can incorporate live heart rate as part of its interactivity, such as wearables fitness tracker, meditation trainer, and sound and light installation.


#### [Meditation Trainer](https://learn.adafruit.com/heart-rate-variability-sensor)
![mediation]({{ site.baseurl }}/img/tangible/biometric_in_use.jpg)

This project in particular points out a different way of using pulse data.
When we think of pulses, we normally think it is likely to be pretty constant values. However, our interval between beats (IBI) fluctuates a lot, and the variance between heart beat interval is known as heart rate variability (HRV). When we breath in a certain pattern, our cardiac rhythms can also fall in sync and HRV becomes a sine wave. Meditation Trainer is a project that uses live heart-rate and based on this interesting fact to train the user to breath better and reduce anxiety.
![HRV]({{ site.baseurl }}/img/tangible/biometric_hrv_stressed.jpg)
***HRV pattern of someone that is feeling stressed***
![HRV]({{ site.baseurl }}/img/tangible/biometric_hrv_calm.jpg)
***This is the goal of meditation trainer - calm breathing pattern***


#### List of creative projects using pulse sensor amped
- Interactive mediation game: [Heart Sync](https://ellennickles.com/itpblog/2017/12/3/weeks-14-and-15-heart-sync)
- Light installation: [Pulse Room](https://learn.adafruit.com/pulse-room)
- Physical installation: [Fall In Line](https://www.sparkfun.com/videos#all/ZgtvEsSGMJ8/124)

## Strengths and Weaknesses
Strengths:
- Easy setup for use
- Small frame that can fit in most projects, good for wearables.
- It has a complementary software and well maintained [library](https://github.com/WorldFamousElectronics/PulseSensor_Amped_Arduino).

Weaknesses:
- The retail price is around $25. It is expensive; especially knowing its components.
- The circuit board is exposed, and need to prepare the sensor from body naturally produced sweat and oil. Otherwise, the board can be shorted by touching the solder points. The current solution is to use a thin film of vinyl on the sensor side. The back side can be protected by using a velcro dot or hot glue. Detailed instruction can be found on the [starting guide](https://media.digikey.com/pdf/Data%20Sheets/Pulse%20PDFs/PulseSensorAmpedGettingStartedGuide.pdf)
- The functionality is limited.
- The code involved for getting good reading can be complicated.

## Example Schematic and Microcontroller Code

Here is the schematic and the code of using NeoPixels to display Pulse

![neopixels display](https://cdn-learn.adafruit.com/assets/assets/000/027/919/original/biometric_Pulse-Sensor_final.jpg?1443353162)

<script src="https://gist.github.com/linzhangcs/a9b7a6bb633c2f04ac1b962d09a5fa67.js"></script>

<script src="https://gist.github.com/linzhangcs/9b3cc5a3e5fdb02cf0402bd169d63b28.js"></script>

## Citations
- Information and links about how Pulse Sensor work found on [Quora](https://www.quora.com/How-do-optical-heart-rate-sensors-work)
- Pulse Sensor Amped project kinks and images found on [Adafruit Pulse Sensor Amped](https://www.adafruit.com/product/1093)
- Information on Pulse Sensor Amped found on the [official website](https://pulsesensor.com)
- Data Sheet found [here](https://media.digikey.com/pdf/Data%20Sheets/Pulse%20PDFs/PulseSensorAmpedGettingStartedGuide.pdf)
- Schematic and Code found [here](https://learn.adafruit.com/pulse-sensor-displayed-with-neopixels/overview)
