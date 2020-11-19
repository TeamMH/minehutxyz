---
description: Learn how to make a One Player Sleep Skript
---

# Example: One Player Sleep

## OVERVIEW

This tutorial will show you how to allow only one player on your server to sleep, for the entier server to turn to day time.

## CODE

```text
on bed enter:
  cancel event
  set time of event-world to day
  broadcast "World %event-world% has been set to day time as %player% has slept!"
```

## EXPLAINED

The function `on bed enter:` is self explanitory, it triggers when a player enters a bed.

The cancel event will kick the player out of the bed.

Then, the time of the world the event was triggered in will be set to day.

Then, it broadcasts the world that was set to day and the player that triggered it.

{% hint style="success" %}
Join our [**Discord**](https://discord.gg/TYhH5bK) to become an **official writer**, **site updates**, and **much more**.
{% endhint %}

