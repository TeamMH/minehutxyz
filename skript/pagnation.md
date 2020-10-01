---
description: Learn how to make a pagnated GUI. This allowed people to make "pages" in a GUI, and is infinitly expandable.
---

{% hint style="info" %}
This tutorial was made by Blocksnmore. Lean how to contribute [here](/contribute.md).
{% endhint %}


# Comments

## What is "pagnation"?

Pagnation is making interactive GUI that have multiple pages. This is useful for things like a big shop or auction house. When loading a page, you can also load up what you want to add by saving to to a variable then adding it. If you need help ask on our discord server found [here](https://invite.gg/minehutxyz)!

Examples:
```
command /demo-gui [<integer>]: 
    trigger:
        set {_p} to player
        if arg 1 is not 2 or 3:
            wait 2 ticks
            open chest with 6 rows named "&bPage 1" to {_p} # Opens GUI
            wait 2 ticks
            loop integers between 0 and 54 - 1: # Formats all slots with gray stained glass panes as a filler
                format slot loop-number of {_p} with gray stained glass pane named "&r" to be unstealable
            format slot 53 of {_p} with paper named "&bNext Page" to run [make player execute command "/demo-gui 2"]
        else if arg 1 = 2:
            wait 2 ticks
            open chest with 6 rows named "&bPage 2" to {_p} # Opens GUI
            wait 2 ticks
            loop integers between 0 and 54 - 1: # Formats all slots with gray stained glass panes as a filler
                format slot loop-number of {_p} with gray stained glass pane named "&r" to be unstealable
            format slot 45 of {_p} with paper named "&bLast Page" to run [make player execute command "/demo-gui"]
```

{% hint style="success" %}
Join our **[Discord](https://invite.gg/minehutxyz)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}
