---
description: >-
  WorldGuard is a well-known plugin used for protecting your builds
  [https://worldguard.enginehub.org/en/latest/]
---

# WorldGuard

### _This tutorial was submitted by PandaChan. Find out how you can submit a tutorial_ [_here_](../contribute.md)_._

## OVERVIEW

**WorldGuard** is a powerful plugin with a large bag of tricks for server owners, server map makers, regular survival servers, and everyone in between! Create zones in your world that only permit mods or certain players from building within Set additional game rules on your server \(deny wither block damage, falling damage, etc.\).

## DEPENDENCIES

WorldGuard is quite easy to use, you only need two plugins for everything to work! These two plugins being **WorldGuard** of course and **WorldEdit** for creating regions.

## CREATING REGIONS

WorldGuard has many features but one of the more known ones is protecting builds with regions, regions are certain areas that are protected from users.

Our first step is getting a wand from WorldEdit, this can be done by simply doing //wand after executing this command you should receive a wooden axe. After this you create a kind of invisible box with your wand, you do this by going to one side of the build and right clicking a block on the bottom or simply typing //pos1 and then going to the other side and typing //pos2 high up in the air to create the box. Once you've done this all you have to do is type `/rg define (name)`

You can also go a bit deeper with this command and give the region owners on creation, this allows these users or groups to do whatever they want in the region. The more detailed commands will turn into `/rg define (name) (optional users) (g:(optional groups))`

## USING REGION FLAGS

Region flags are 'flags' that allow users to do a specific thing within the region, whether this means allowing users to click buttons or attack other users within the region.

To change the flags your region currently has all you have to do is `/rg flag (region) (flag) deny/allow` WorldGuard has many different kinds of flags, all flags are listed here \([https://worldguard.enginehub.org/en/latest/regions/flags/\#protection-related](https://worldguard.enginehub.org/en/latest/regions/flags/#protection-related)\)

## EXTRA

Though WorldGuard is most known for its protection purposes, there are also some other fun commands that can be useful, some of these being `/heal`, `/god`and `/stack` for example. I highly recommend using this plugin if you want some simple protection!

{% hint style="success" %}
Join our **[Discord](https://discord.gg/TYhH5bK)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}
