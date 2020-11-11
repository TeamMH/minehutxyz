---
description: Learn how to edit the World Border on your Minehut server.
---

# World Border

## OVERVIEW

The world border appears as animated, diagonal, narrow stripes. When the border is not moving, the stripes are a translucent aqua color. If the border is expanding, the stripes appear green; if the border is shrinking, the lines appear red.

## COMMANDS

* `/worldborder set <sizeInBlocks> [timeInSeconds]` This sts the border to a square region with the specified size in blocks as the width and length.
* `/worldborder center <x> <z>` This sets the center of the area inside the world border to the specified  and  coordinates.
* `/worldborder add <sizeInBlocks> [timeInSeconds]` This adds or subtracts sizeInBlocks to/from the current world border width and length.
* `/worldborder damage buffer <sizeInBlocks>` This sets the number of blocks a player may safely be outside the world border before taking damage.
* `/worldborder warning time <timeInSeconds>` This causes the screen to be tinted red when a contracting world border reaches the player within the specified time. The default is 15 seconds.
* `/worldborder warning distance <sizeInBlocks>` This causes the screen to be tinted red when the player is within the specified number of blocks from the world border. The default is 5 blocks
* `/worldborder get` This returns the current width of the world border.

{% hint style="success" %}
Join our [**Discord**](https://discord.gg/TYhH5bK) to become an **official writer**, **site updates**, and **much more**.
{% endhint %}

