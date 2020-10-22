---
description: Learn how to create a bossbar with Skript
---

# Example: Bossbar | Download this at https://github.com/TeamMh/minehutxyz/blob/master/skript/downloads/bossbar.sk?raw=true

## OVERVIEW

A bossbar is useful in many different cases. A bossbar can be found at the very top of the screen, and using Skript we can easily configure the message to something useful.

## CODE

{% hint style="info" %}
Skript addon **skRayFall** is required!
{% endhint %}

```
on join:
  create bossbar titled "&aWelcome to the server." and id "bossbar::%player's uuid%" for player with progress 100 with colors blue
```

## EXPLAINED

This creates a bossbar with the text `"&aWelcome to the server."`.
We use the `player's uuid` in the bossbar id for future use, incase we need to change a specific player's bossbar.
`progress 100` will fill up the bossbar completely, and `colors blue` will set it to the colour blue.
