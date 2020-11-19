---
description: 'A simple, yet in-depth tutorial on the popular plugin MineResetLite.'
---

# MineResetLite

{% hint style="info" %}
This tutorial may need the plugin **WorldEdit**
{% endhint %}

## OVERVIEW

MineResetLite is a popular plugin avaliable on Minehut that enables you to make easy mines that reset over time. Using positions you can make cubes of pure ores, or mixes of loads of ores! It is a brilliant plugin if you are trying to make a SkyGen server. With MineResetLite, you can even add potion effects inside the mines, and using Skript you can disable item drops, or add special perks to go along with it!

## HOW TO DO

Firstly, you need to install MineResetLite, if you do not know how to install a plugin, follow one of our other tutorials.

Once you have installed the plugin, restart your server and it should be there!

**Next, lets dive ingame and do some commands,**

Firstly, you want to set your regions, use the commands **/mrl p1** and **/mrl p2** in the spots you want to make your mine, similar to how WorldEdit uses the //pos1 and //pos2 feature.

**Once this is complete, you have created your mine region, time to create the mine.**

Type **/mrl create \(mine name\)** into your Minecraft server chat box, and name it something that is easily rememberable. You can delete a mine by typing **/mrl delete \(mine name\)**. This will only work with a mine that exists.

**Setting Mine Blocks**

You can set the blocks that will appear inside the mine by doing the command **/mrl set \(mine name\) \(block\) \(amount \[Percentage\]\)**. This sets the blocks inside the mine.

EG: /mrl set Mine1 iron\_ore 50% & /mrl set Mine1 coal\_ore 50%

**Setting Mine Flags**

You can set the flags of the mine, which enable the mine to perform various functions, such as resetting every 10 minutes, and silently resetting, as well as resetting when 50% of the blocks are gone.

**Flags:** **Make mines reset after 25% of blocks are still unmined:** /mrl flag \(mine name\) resetPercent 25%

**Make mines reset after 1 minute:** /mrl flag \(mine name\) resetDelay 1

**Make mines reset silently:** /mrl flag \(mine name\) isSilent true

_Alternatively, you can use this blank template for flags: /mrl flag \(minename\) \(flag\) \(value\)_

{% hint style="success" %}
Join our [**Discord**](https://discord.gg/TYhH5bK) to become an **official writer**, **site updates**, and **much more**.
{% endhint %}

