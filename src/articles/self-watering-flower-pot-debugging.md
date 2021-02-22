---
title: Self Watering Flower Pot Debugging
permalink: /blog/self-watering-flower-pot-debugging/
date: 2021-02-21
layout: base-layout.njk
breadcrumbs:
  - label: Home
    url: /
  - label: Blog
    url: /blog/
  - label: Self Watering Flower Pot Debugging
tags:
  - posts
---

# Debbugging the Self Watering Flower Pots

The self watering flower pot program runs extremely well when plugged directly into an external computer. However, when a 9V power supply is plugged into the arduino, all four pumps will turn on at once. This is because the wiring diagram provided by WayinTop has a single error: The positive power jumper that is connected to the relay board should be plugged into the 5V power pin, and not the VIN power pin. The wiring diagram for the relay board and the arduino should look like this:

![correct wiring diagram](/img/correct-wiring-diagram.jpg)

After making this small change, the entire system can run on external power without having a computer connected. I will run the system for a day connected to a computer to ensure that nothing strange happens such as strange sensor readings or motors turning on/off without the correct data value.
