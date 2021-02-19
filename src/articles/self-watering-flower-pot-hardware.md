---
title: Self Watering Flower Pot Hardware
permalink: /blog/self-watering-flower-pot-hardware/
date: 2021-02-16
layout: base-layout.njk
breadcrumbs:
  - label: Home
    url: /
  - label: Blog
    url: /blog/
  - label: Self Watering Flower Pot Hardware
tags:
  - posts
---

# Self Watering Flower Pot Hardware

<!-- Excerpt Start -->
Following the recommended wiring diagram was farily easy requiring only a few rows on a breadboard. I decided to use two small breadboards to keep things organized, and I will be looking for ways to make things more compact as I go. The Wayintop kit you can buy on amazon comes with all the parts you need, but I did have to do some refinement to make them more usable. This is only an issue with the pumps, as the leads on them are extremely small and I don't want to risk damaging the waterproof coating on the wires since I have to submerge the pumps in the reservoir. To solve this problem, I spliced some red and black wire to the positive and negative poles respectively, giving me an extra 1 1/2 inches of wire to work with.
<!-- Excerpt End -->

![soldered wires](/img/soldered-wires.jpeg)

I also put some shrink wrap around the wires to make the wires look better. This will also help to reinforce the splice and prevent me from pulling the wires apart while moving things around.

![shrink wrapped wires](/img/shrink-wrapped-wires.jpeg)

Once the pumps were prepped, wiring everything up is a very simple exercise. I started by wiring the motor relay board to the battery pack, and plugged in the wires for the pumps. This was very easy as the relay board is very simple, and the wiring diagram is very clear as to what wire goes where. Unfortunately, I had to stop for a night after I hooked up the wires and the battery pack, as I did not have any male-female jumper cables. The data pins on the motor relay board are male, while that the arduino and the breadboard pins are female, meaning I had to use jumpers that have a male header on one end and a female header on the other (male headers are plugged into female headers). 

![motor layout](/img/motor-wiring.jpeg)

Once I found some properly configured jumper cables, I was able to finish connecting the data wires and power wires for the sensors in about 10 minutes.

![wiring finished](/img/wiring-finished.jpg)

The cups that I have the pumps in are just placeholders for now, as I am planning on implementing a larger reservoir that I can put my electronics on top of, allowing for the pumps to be suspended down into the liquid. I believe that this will allow for the electronics to stay safely away from the water, as there will be little to no way for the water to reach up past the lid. I will put the arduino, motor driver, and breadboards into a project case to make absolutely sure as electronics and water do not mix.