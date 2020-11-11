---
description: Learn how to create a scoreboard with Skript.
---

# Example: Scoreboards

## OVERVIEW

Scoreboards are useful tools that can provide players with useful information such as their balance, rank and many more things.

## CODE

### SKRAYFALL SCOREBOARD

```text
on join:
    set name of sidebar of player to "&6skRayFall"
    set score "First Line" in sidebar of player to 1
    set score "Second Line" in sidebar of player to 2
```

### SKBEE SCOREBOARD

#### IN ORDER TO USE SKBEE SCOREBOARDS IF YOU HAVE SKRAYFALL DISABLE "FAST SCOREBOARDS" IN THE SKRAYFALL CONFIG

```text
on join:
    set title of player's scoreboard to "&6&lServer Info"
    set line 1 of player's scoreboard to "&7• &eOnline: &f%size of all players%"
```

#### SKBEE BASIC STATISTICS SCOREBOARD

```text
on join:
    while player is online:
        set {_uuid} to {_p}'s uuid
        set line 2 of {_p}'s scoreboard to "&6Kills: &f%{kills::%{_uuid}%} ? 0%"
        set line 1 of {_p}'s scoreboard to "&6Deaths: &f%{deaths::%{_uuid}%} ? 0%"
        wait 1 second

on death of player:
    add 1 to {deaths::%victim's uuid%}
    if attacker is a player:
        add 1 to {kills::%attacker's uuid%}
```

{% hint style="success" %}
Join our [**Discord**](https://discord.gg/TYhH5bK) to become an **official writer**, **site updates**, and **much more**.
{% endhint %}

