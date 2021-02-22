---
title: Autonomous Flower Pot Data Hub Concept
permalink: /blog/autonomous-flower-pot-data-hub-concept/
date: 2021-02-21
layout: base-layout.njk
breadcrumbs:
  - label: Home
    url: /
  - label: Blog
    url: /blog/
  - label: Autonomous Flower Pot Data Hub Concept
tags:
  - posts
---

# Autonomous Flower Pot Data Hub Concept
<!-- Excerpt Start -->
With the completion of the self watering system for the flower pot, I realized a serious flaw with my system. In order to get data from my Arduino Uno, I had to directly connect a laptop to the Arduino. However, even with the direct connection I couldn't see data over time, resulting in me only getting a real time idea of how the moisture levels are doing. After consulting the resources that I have, I decided that I should find a way to have the Arduino pass its information to a Raspberry Pi, which will then allow me to remotely connect via wifi to a web server to see the sensor data in real time, as well as sensor data in the past on a graph.
<!-- Excerpt End -->
## Goal

The goal of upgrade to the Self Watering Flower Pot is to:

1. Allow me to remotely access the sensor data
2. Allow me to see data over time

## Expected Changes

There are two major changes that I will have to make to my arduino code:

- Store sensor data in a single array instead of four individual variables
- Remove the print to serial monitor

## Expected Additions

The only major addition from a hardware perspective is a Raspberry Pi 3 connected to the arduino through the microusb port on the arudino. The Raspberry pi will have the following functions:

- pull the sensor data array and store the values in a data file
- host a web server to allow me to view and analyze data from the data file, as well as let me see what the current sensor values are in real time
- allow me to change moisture values based on what I think would be best for the plants (Optional until later)

The Raspberry pi will also allow me to pull data from future systems such as PH monitoring systems, plant monitoring systems, etc. I will hopefully be able to finish this upgrade in the next couple of weeks.