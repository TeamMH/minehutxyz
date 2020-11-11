---
description: Learn how to customise your tablist with Skript.
---

# Example: Tablist

## OVERVIEW

This tutorial will show you how to create a customised tablist _\(TAB key\)_ on your server using Skript.

{% hint style="info" %}
Skript addon skRayFall is required!
{% endhint %}

## CODE

```text
on join:
  set tab header to "" and footer to "" for player
```

## EXPLAINED

Simple add in text between the `""`'s and you're all set. The tab header and footer will only be set when the player joins, so if you're looking to update it, it's better to use a function _\(below\)_.

## FUNCTION

```text
function tab(header: text, footer: text, P: player):
  set tab header to "%{_header}%" and footer to "%{_footer}%" for {_P}
```

