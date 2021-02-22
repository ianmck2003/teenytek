---
title: Self Watering Flower Pot Programming
permalink: /blog/self-watering-flower-pot-programming/
date: 2021-02-20
layout: base-layout.njk
breadcrumbs:
  - label: Home
    url: /
  - label: Blog
    url: /blog/
  - label: Self Watering Flower Pot Programming
tags:
  - posts
---

# Self Watering Flower Pot Programmming

<!-- Excerpt Start -->
Programming the arduino to run the pumps and the sensors was very simple as the arduino has to only do two things: read the sensor input and turn the pumps on and off accordingly. In order to understand what sensors were returning, I added a set of code in the loop section to return the sensor reading from each pot. This also allowed me to fine tune the timing for when the pumps turn on to fall into the following ranges:
<!-- Excerpt End -->

<ul style="list-style: none;">
  <li>450+ = Bone Dry</li>
  <li>450 - 400 = Water Soon</li>
  <li>400 - 300 = Ideal range</li>
  <li>300- = Swamp</li>
</ul>

For clarification, the lower the value that the sensor returns, the more moisture that is present.

The code used on the arduino is very simple and follows the following steps:


Setup:
  - Set digital pins 2-5 as output pins
  - Set analog pins 0-3 as input pins
  - Set output of all digital pins to HIGH<a href="#fn1" id="fnote1"><sup>*</sup></a>

Loop:
  1. Poll analog pins for sensor values
  2. Print analog pin values to serial monitor
  3. Repeat for all sensor values:
      - If sensor value is above 375, turn pump associated with sensor on (set output to LOW)
      - If sensor value is less than 375, turn pump associated with sensor on (set output to HIGH)
  4. Delay for 1000ms

As of now, my code is using 4 individual floats to store each value, but I am planning to modify the program to store sensor data in an array to make it easier to extract data to a separate program or computer (such as a raspberry pi).

I also swapped out the Arduino Uno produced by Arduino with an Elektor Uno R4, which is essentially an Arduino Uno built around the ATmega328PB-au chip. I made this decision because the box of spare Arduino related parts and projects has several Elektor Uno R4s, so I wanted to keep the microcontrollers used on this project uniform so modifying/upgrading the system will be easier.

Elektor Uno R4:

![Elektor Uno R4](/img/elektorlab-uno-r4.png)

Arduino Uno:

![Arduino Uno](/img/arduino-uno.jpg)

<hr style="width: 30rem; margin-top: 1rem; border: 1px solid var(--skyblue);">

<sup id="fn1">*</sup> The 4 channel relay board used for this project is low input activated.<a href="#fnote1">&larrhk;</a>
