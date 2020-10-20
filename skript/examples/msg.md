---
description: Set up private messaging on your server with Skript.
---

# Private Messaging

## OVERVIEW

This tutorial will go over how to set up a private messaging system on your server using Skript, it assumes basic knowledge of Skript (read posts above if needed).

## HOW TO SET UP PRIVATE MESSAGING

You can create a messaging system using the [Message effect](https://skripthub.net/docs/?id=1130) in a custom command, here is a basic example:

```vb
command whisper <player> <text>:
  trigger:
      send "%player% whispers to you: %arg-text%" to arg-player
      send "You whispered to %arg-player%: %arg-text%" to player
```

There are 3 components to this command:
`<player>`: The player to send a message to.
`<text>`: The text to send to said player.
The send lines: Sends the message to the requested player, and notifies the player that the message went through.

You are able to add aliases to the command by adding `aliases: /alias-1, /alias-2` to the command, right before the trigger.
Note that you cannot have `/msg` or `/tell` as an alias because it is occupied by Minehut's own messaging system.

You can add a usage message to the command by adding `usage: usage message` before the trigger. Example: `usage: &c/whisper (player) (message)`.

{% hint style="success" %}
Join our **[Discord](https://discord.gg/TYhH5bK)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}
