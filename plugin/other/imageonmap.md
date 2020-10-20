---
description: Learn how to use the ImageOnMap plugin.
---

# ImageOnMap

## OVERVIEW

Have you ever wanted to view an image on an ingame map? ImageOnMap provides just that. ImageOnMap allows you to load a picture from the Internet to a Minecraft map.

## PLUGIN

### ToMap Command
Firstly, make sure you have a free inventory slot, as the plugin will give you a map.
The main command we will be using is **/tomap <url>**. You can resize the maps by adding the width and height after the keyword resize, for example **/tomap url resize 2 4**. 
You can also change the scaling method by replacing the resize keyword to **resize-stretched** to stretch the image to the surface *(the image may be distorted)*, or **resize-covered** to to ensure the image covers the whole surface *(the image will never be distorted, but some parts may be lost near the borders)*.
The permission node for this is **imageonmap.new**.

### Maps Command:
**/map**s is another command which opens a GUI to see, retrieve and manage user's maps.
You can retrieve any created maps, or manage created maps. Maps can be renamed (for organization), deleted (but they won't render in-game anymore!), or partially retrieved (for posters maps containing more than one map).
Permission: **imageonmap.list**, **imageonmap.get**, **imageonmap.rename** and **imageonmap.delete** for actions into the GUI.

{% hint style="success" %}
Join our **[Discord](https://discord.gg/TYhH5bK)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}
