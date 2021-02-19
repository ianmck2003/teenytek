---
title: Self Watering Flower Pot Concept
permalink: /blog/self-watering-flower-pot-concept/
date: 2021-02-06
layout: base-layout.njk
breadcrumbs:
  - label: Home
    url: /
  - label: Blog
    url: /blog/
  - label: Self Watering Flower Pot Concept
tags:
  - posts
---

# Self Watering Flower Pot Concept

<!-- Excerpt Start -->
The idea is to create a self watering flower pot using an arduino, a moisture sensor, and a pump in a water bucket. The arduino will take the data input from the sensor and determine if the soil is too dry. If the soil is too dry, it will activate a pump and run until the soil is moist enough. It will then stop the pump while the arduino waits a set amount of time before priming the system again.
<!-- Excerpt End -->

I will be using an Arduino Uno combined with the [WayinTop Automatic Irrigation kit](https://github.com/WayinTop/Automatic-Plant-Watering-System-Tutorial/blob/master/4%20Channel%20Relay%20Plant%20Watering%20System%20and%20code/Plant%20Watering%20System%20Tutorial-English.pdf), which comes with small DC submersible pumps, capacitive moisture sensors, and a driver board that can control up to 4 pumps at once. The wiring is relatively simple, using 4 of the 6 analog ports, digital pins 3-6, and 3 power pins. There will be a breadboard used since it is more efficient to run the sensors in parallel on a single power circuit, but it does not have to be very big since only 2 rows of 5 pins will be used.


![wiring diagram](/img/self-watering-flower-pot-array-schematic.png)
