---
description: Learn how to make a speedrunner versus hunter gamemode on minehut.
---

# Dream's Manhunt

## OVERVIEW

This plugin is a remake of the popular YouTuber Dream's Manhunt gamemode. This tutorial will show you how to set it up.

## HOW TO USE

Run `/speedrunner (player)` to **add a player** to the speed runner team and use `/speedrunner (player) remove` to **remove the player** from the speed runner team.

Use the command `/assassin (player)` to **add a player** to the hunter group and use `/assassin (player) remove` to **remove the player** from the hunter group.

**You should now be able to start a manhunt!**

## CONFIG.YML SETUP

If you would like to play the manhunt with different options you can open the config.yml file and change one of these properties:

**"compass-tracking"** - `true/false`, changes if the assassins compass \(if they have one\) points to the closest speedrunner

**"compass-give"** - `true/false`, if true gives a compass to assassins on group assignment and on respawn

**"compass-particle"** - `true/false`, if true draws a yellow particle near assassin \(if he holds a compass in main hand\) in the direction of closest speedrunner

**"compass-particle-in-nether"** - `true/false`, the previous option also works in nether if this option is set to true

**"compass-random-different-worlds"** - `true/false`, if true compass will go crazy if there is no speedrunners in the same world

**"assassins-insta-kill-speedrunner"** - `true/false`, changes if the assassin can one shot the speedrunner

**"freeze-assassin-when-seen"** - `true/false`, changes if the assassin will be frozen in place if the speedrunner puts their crosshair over the assassin. Note if frozen in the air, it may trigger a "Flying is not enabled on the server disconnect", so it is recommended to disable it.

Once you've edited the file, save it and run `/assassin` and the plugin will reload.

{% hint style="success" %}
Join our [**Discord**](https://discord.gg/TYhH5bK) to become an **official writer**, **site updates**, and **much more**.
{% endhint %}

