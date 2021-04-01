---
title: Open Source Drone
permalink: /blog/open-source-drone/
date: 2021-03-25
layout: base-layout.njk
breadcrumbs:
  - label: Home
    url: /
  - label: Blog
    url: /blog/
  - label: Open Source Drone
tags:
  - posts
---

# Open Source Drone

![Drone](/img/open-source-drone.jpeg)
<!-- Excerpt Start -->
I tried to build a drone, and ended up making an angry bee. When I spun up the motors for the first time it said, "5 more minutes" and threw its front right propeller at me. I was perplexed as to how the drone got my sleeping habits. Like project like builder perhaps?
<!-- Excerpt End -->
I built an open source drone following instruction from Doctor Peter Dalmaris' Udemy course, Make an Open Source Drone. The course is very detailed, and I was able to build the drone in a very short amount of time. I followed the build instructions for the version based on a PixHawk 2.4.8 flight computer, and flying it has been highly enjoyable for me. Of all of the drones that I have flown, this one is the largest by a huge margin. It really allowed me to realize the extent of the inherent stability of larger aircraft, as I barely had to move the sticks to get a controllable response. I also realized that capacitors are a really useful thing to have, as the drone would not be able to fly if the voltage output from the battery dropped too low.

An interesting effect I found from the battery dropping 0.5V from full charge is the ground effect. The drone would not be able to sustain an altitude greater than 4 inches if the battery is too low, but it can sustain 4 inches for several minutes before the battery got so low that the craft wouldn't even spin around on the ground due to uneven thrust output. Building GEVs are now of interest to me, as I think it would be very fun to have a little hovercraft skimming around and doing circles around me.

I did not build the drone entirely for fun. I also built it to learn how to use hobby electronics such as brushless motors, electronic speed controllers, as well as power distribution boards and power modules. This will allow me to built other remotely controlled vehicles such as cars, boats, and planes. I am hoping that I will be able to integrate a more powerful computer into a remotely controlled vehicle built around the PixHawk to allow me to create a fully automated vehicle.

I will probably upgrade the drone in the future to have more flight stability and carry an on board camera. I won't be increasing the maximum controllable range of the drone, as FAA regulations do not allow me to be more than 100 feet from the drone without a permit. If I can acquire a permit, I will consider upgrading the telemetry unit that I currently have.

Course link: [Make an Open Source Drone](https://www.udemy.com/course/make_a_drone/)