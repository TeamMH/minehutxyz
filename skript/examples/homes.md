---
description: Learn how to use and make homes for yourself and server members. Including permissions, multiple home managment and home deletion.
---

# Home | Download this at https://github.com/TeamMh/minehutxyz/blob/master/skript/downloads/homes.sk?raw=true

{% hint style="info" %}
This tutorial was made by [Rqdioqctive](https://github.com/Rqdioqctive). Lean how to contribute [here](/contribute.md).
{% endhint %}


## What are homes?

Homes are a way for you and your server members to easily access their bases and/or saved destinations around the world. Below are chunks of a home skript explained.

Examples:
```
command /sethome: #command to sethome
  permission: skript.sethome #permission for sethome
  permission message: &cInsufficient permissions! #message if they dont have permission
  trigger:
    set {home::%player's uuid%} to player's location #sets home location
    send "&7Set your home to your location!" #sends message
```

In the above skript, we are making a new command called `/sethome` and having its permission be `skript.sethome`. It sets a variable, `{home::%player's uuid%}` which stores our location, then sends us a message of confirmation.

{% hint style="warning" %}
These skripts use `player's uuid`, so even if you change your Minecraft username, your variable will not be last because UUIDs do not change unlike usernames.
{% endhint %}

```
command /home: #command to teleport to home
  permission: skript.home #permission for home
  permission message: &cInsufficient permissions! #message if they dont have permission
  trigger:
    if {home::%player's uuid%} is set: #checking if home location is set
      teleport player to {home::%player's uuid%} #teleports player
      send "&7Teleported to your home!" #sends message
    else: #if they dont have a home set
      send "&cNo valid home!" #sends error message
```

In the above skript, we are making a new command `/home` which will teleport us to our location from before and having its permission be `skript.home`. It checks to see if our variable, `{home::%player's uuid%}`, has been set. If yes, then it will teleport us to the location of our home and send us a message of confirmation, however, it will send us an error message if the variable isn't set.

{% hint style="info" %}
These skripts use `comments`, so that they can explain all/most of the lines to you. These are marked by the `#` symbol, so if you wish to remove them then delete all text after & along with the `#`.
{% endhint %}

```
command /delhome:
  permission: skript.delhome
  permission message: &cInsufficient permissions!
  trigger:
    if {home::%player's uuid%} is set: #checking if home location is set
      delete {home::%player's uuid%} #deletes the home location from existence
      send "&7Deleted your home!" #sends message
    else: #if they dont have a home set
      send "&cNo valid home!" #sends error message
```

In the above skript, we are making a new command `/delhome` which will delete our home variable/location if we don't want to store it anymore. Its permission is `skript.delhome` and it checks to see if our variable, `{home::%player's uuid%}`, is once again set. If yes, then it deletes the variable & gives us a message of confirmation, however, it will send us an error message if our variable is not set.


{% hint style="success" %}
Join our **[Discord](https://discord.gg/TYhH5bK)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}
