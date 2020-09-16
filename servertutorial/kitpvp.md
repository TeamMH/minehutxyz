---
description: KitPVP can be a well-visited gamemode on minehut if your server is well made. Here are some tips for making one!
---

# KitPVP

## Necessary Plugins

Plugins are very important for kitpvp, here are a few that are needed to make a good kitpvp on minehut!

Essentials - Has TONS of features like expanding on vanilla commands, and adding more. However, the important part is its kit capabilities.

Skript - Basically a requirement to make a unique server on a 12 plugin budget, which is important to do if you want to get more players. Just a great tool overall to do a lot with.

A permission plugin - You want either "Permissions EX" or "LuckPerms" to manage what privileges you want to give players.

Vault - Helps Essentials' built in economy system work and also your permission plugins (for prefixes and suffixes). Definitely a must-have.

WorldEdit + WorldGuard - Unless you want breaking blocks and PvP in spawn, you want this. It lets you manage areas and either build quickly or set different rules that apply in that area.

## Optional Plugins

There are a few plugins that are good for additional features as well. Here are some good ones.

ProtocolSupport (or ViaVersion, ViaBackwards, and ViaRewind, they are less buggy, but fill up more plugin slots) + OldCombatMechanics - Allows 1.8 players to join and it will also use 1.8 pvpo mechanics, much like Hypixel does.

Skript Addons - There are tons of other plugins that give skript more functionality and options to do, such as TuSKe or SkQuery

Buycraft/CraftingStore - If you want to sell ranks, you will want this plugin!

HolographicDisplays - Allows you to put floating text around, can be good for directing newer players.

EssentialsChat/Spawn - These are two of the most widely used essential addons, as it allows you to have the ability to customize chat, or set spawnpoints for people.

**The following plugins require a seperate plugin called ProtocolLib**

Matrix Anticheat - A pretty great anticheat that can sniff out hackers pretty well. 

SuperVanish - The best plugin if you want to appear as if you are offline to players on your server.

## Your Map

Make sure that you have some sort of confined area to PvP in, otherwise people would spread out too much and less encounters would occur, and that would at that point just defeat the point of the server.

## Configuring your server

Now, the main thing left is to configure your server. Fist things first, op yourself through the dashboard.

**So let's figure out the more necessary plugins! We are starting with the in console files for now. If you need help with other plugins, check if they are in the plugins section of this forum.**

Essentials - Toward the beginning of the config, change the nick prefix setting to '', and change op color to none. It just looks better. Also, if you have essentials spawn, scroll down until you find the spawn section, and there is a setting that changes what kit you get on join, change that to the kit you want new players to automatically get. I will let you figure out your essentials chat, as it is very customizable.

Skript - While it doesn't need configuration, you need to put skripts in the console, you can't code from in game!

**Now, let's do some in-game stuff.**

Essentials - First, you want to have kits. Basically, creating a kit is easy. Just do /createkit <kit name> <cooldown in seconds> and your inventory will get copied to a kit. Additionally, If you have essentials spawn, do /setspawn where you want people to respawn.

WorldEdit - If you want to make larger scale builds, this tool can help you out. If you need more help, check out our WorldEdit tutorial at this link (https://minehut.xyz/plugin/worldedit)

WorldGuard - This is very important to do! First things first, select your "Spawn" region using your WorldEdit wand, then use the command "/rg define spawn", which defines a new region. Then, paste these commands in to ensure there can't be grifing! (/rg flag spawn pvp deny - Blocks PVP in spawn.) (/rg flag spawn passthrough deny - Blocks building or breaking in spawn.) (/rg flag __global__ passthrough deny - Blocks placement or breaking of blocks globally.) If you need more help, check out https://minehut.xyz/plugin/worldguard!

Permissions Plugin - You can use whichever permission plugin you'd like, learn how to use LuckPerms [here](https://minehut.xyz/plugin/lp) and learn how to use PermissionsEX (or PEX) [here](https://minehut.xyz/plugin/pex).
  
## Congrats!
You have finished all the super important aspects of making a KitPvP server!
