---
description: Learn how to make a paginated GUI. This allowed people to make "pages" in a GUI, and is infinitly expandable.
---

# Pagination [[Download](https://github.com/TeamMh/minehutxyz/blob/master/skript/downloads/pagnation.sk?raw=true)]

{% hint style="info" %}
This tutorial was made by [Blocksnmore](https://github.com/Blocksnmore), and [ReportCardsMC](https://github.com/ReportCardsMC). Lean how to contribute [here](/contribute.md).
{% endhint %}


## What is "pagination"?

Pagination is making interactive GUI that have multiple pages. This is useful for things like a big shop or auction house. When loading a page, you can also load up what you want to add by saving to to a variable then adding it. If you need help ask on our discord server found [here](https://invite.gg/minehutxyz)!

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

```
command /demo-shop [<number = 1>]:
  trigger:
    close player's inventory
    set {_items::*} to "grass block:5:10", "stone:3:7", "cobblestone:1:5", "andesite:1:2", "dirt:0.5:1", "bedrock:0:1000", "podzol:15:20", "white wool:10:20", "red wool:10:20", "green wool:10:20", "lime wool:10:20", "magenta wool:10:20", "black wool:10:20", "pink wool:10:20", "white concrete:10:20", "red concrete:10:20", "green concrete:10:20", "lime concrete:10:20", "magenta concrete:10:20", and "black concrete:10:20" #Format "Item:Sell Price:Buy Price"
    set {_lines} to 2 # Max at 5 please
    set {_max-pages} to rounded up size of {_items::*} / ({_lines} * 9)
    set {_page} to rounded arg-1
    set {_page} to 1 if {_page} <= 1
    set {_page} to {_max-pages} if {_page} > {_max-pages}
    
    open chest with ({_lines} + 1) rows named "&3SHOP &f» &bPage %{_page}%" to player
    set {_current} to (({_page} - 1) * ({_lines} * 9))
    set {_nextpage} to {_page} + 1
    set {_lastpage} to {_page} - 1
    format gui slot (numbers between ({_lines} * 9) and ({_lines} * 9 + 8)) of player with air to do nothing
    if {_lastpage} >= 1:
      format gui slot ({_lines} * 9) of player with red stained glass pane named "&cPrevious Page" to run:
        make player execute "/demo-shop %{_lastpage}%"
    if {_nextpage} <= {_max-pages}:
      format gui slot ({_lines} * 9 + 8) of player with lime stained glass pane named "&aNext Page" to run:
        make player execute "/demo-shop %{_nextpage}%"
    set {_slot} to 0
    loop ({_lines} * 9 + 1) times:
      if {_items::%{_current}%} is set:
        set {_split::*} to split {_items::%{_current}%} at ":"
        set {_item} to {_split::1} parsed as Item
        set {_sell} to {_split::2} parsed as number
        set {_buy} to {_split::3} parsed as number
        format gui slot {_slot} - 1 of player with {_item} named "&a%{_item}%" lored "&bCost (Buy): &f$%{_buy}% &7(Left Click)||&bCost (Sell): &f$%{_sell}% &7(Right Click)" to run:
          if click type is left mouse button:
            if {money::%player's uuid%} >= {_buy}:
              give player {_item}
              remove {_buy} from {money::%player's uuid%}
            else:
              send "&cInvalid Funds"
          else if click type is right mouse button:
            if player's inventory contains ("%{_item}%" parsed as item type):
              remove 1 of {_item} from player's inventory
              add {_sell} to {money::%player's uuid%}
      else:
        format gui slot {_slot} - 1 of player with air to do nothing
      add 1 to {_current}
      add 1 to {_slot}
    format gui slot (numbers between ({_lines} * 9 + 1) and ({_lines} * 9 + 7)) of player with air to do nothing
      
```


{% hint style="success" %}
Join our **[Discord](https://discord.gg/TYhH5bK)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}
