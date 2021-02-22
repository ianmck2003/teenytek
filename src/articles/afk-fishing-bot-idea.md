---
title: AFK Fishing Bot Idea
permalink: /blog/afk-fishing-bot-idea/
date: 2021-02-21
layout: base-layout.njk
breadcrumbs:
  - label: Home
    url: /
  - label: Blog
    url: /blog/
  - label: AFK Fishing Bot Idea
tags:
  - posts
---

# AFK Fishing Bot Idea
<!-- Excerpt Start -->
In Minecraft 1.16, the single block AFK fish farm design no longer produced treasure pulls, making it largely useless. Personally, I do not enjoy fishing in Minecraft because while it yields very useful treasure such as books of mending and high level protection, the time it takes for a rod to catch something is just too slow and boring for me. Even with the highest level of Lure I cannot Fish in Minecraft for more than 5 minutes before I get bored and decide to go do something else.
<!-- Excerpt End -->

Recently my father provided me a link to a very interesting Minecraft bot creater built around Node.js (the same framework used by the static site generator [Eleventy](/blog/making-teenytek/). I believe that I can build a bot that will not only fish for me while I'm away from my computer, but even while I'm working on other things while I'm at my computer. I could become the richest man on my dad's Minecraft server if I built this bot correctly, but it would have to have two settings with two different processes:

## AFK Fish Farm Clicker

This version of the bot will simply continously right click until the fishing rod it is using is too low on durability, or until I tell it to stop. It should also switch to a new fishing rod if its current rod gets too low on durability.

## Pond Fisher

This version of the bot is much more complicated as it must do all of the following

1. Pull in the line every time the bobber dips
2. When its inventory becomes full, it must go to an empty chest in a nearby storage building and deposit everything in its inventory that is not a fishing rod, and should also deposit any fishing rods below 1/4 durability.

I will probably start by making AFK Farm Clicker, then learn how to make the Pond Fisher afterwards, as it will take much more time and research to do.
