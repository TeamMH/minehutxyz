---
description: Learn how events work.
---

# Events

## OVERVIEW & EXAMPLE

Events are called when something happens. So when a player clicks on something, takes damage, dies, when a mob does something, or even when the environment does something else completely independent of entity interaction. This will allow you to make something happen when something else happens. For example:

```text
on death:
    send "&cYou died!" to victim
    send "&6You killed &c%victim%&6!" to attacker
```

You can aslo use parameters in certain event syntaxes to use more particular events and be more specific, like this:

```text
on death of player: # difference is the use of "of player" which only checks when the victim is a player
    send "&cYou died!" to victim
    send "&6You killed &c%victim%&6!" to attacker
```

## INDENTATION

All events must follow the rules of indentation. Read all about indentation [here](indentation.md).

## ALL EVENTS

All events can be found [here](http://de.njol.ch/projects/skript/doc/events), the njol documentation.

{% hint style="success" %}
Join our [**Discord**](https://discord.gg/TYhH5bK) to become an **official writer**, **site updates**, and **much more**.
{% endhint %}

