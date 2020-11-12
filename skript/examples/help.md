---
description: Custom /help command for your server.
---

# Example: Custom /help

## OVERVIEW

This tutorial will show you how to create a custom `/help` command for your server.

## CODE

```
command /help:
  trigger:
    send "Help.."
    send "1) /help | Returns this command."
    send "2) /home | Return home."
```

## EXPLAINED

This is a very bad way of going about this, as it's very limited and hardcoded. A better way might be using variables for lines or an external text file.

{% hint style="success" %}
Join our **[Discord](https://discord.gg/TYhH5bK)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}
