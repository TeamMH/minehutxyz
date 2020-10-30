---
description: >-
  CoreProtect is an extremely useful plugin when creating a server, some of its
  features being rollback and inspecting specific blocks!
  [https://gamedb.gg/games/minecraft/coreprotect-commands/]
---

# CoreProtect

{% hint style="info" %}
This tutorial was made by PandaChan. Lean how to contribute [here](/contribute.md).
{% endhint %}

## OVERVIEW

CoreProtect is a fast, efficient, data logging and anti-griefing tool. Rollback and restore any amount of damage. Designed with large servers in mind, CoreProtect will record and manage data without impacting your server performance.

## DEPENDENCIES

The only plugin you need for CoreProtect to work is of course CoreProtect itself! Besides that, no other plugins are needed.

## USING THE INSPECT COMMAND

There's not much to explain about this command but it is quite useful, all you have to do is `/co i` and you see everyone that has interacted with a certain block. This is extremely useful when trying to figure out who stole the diamonds from your chest or who went into your farm and killed all your animals :\( If you want to disable the inspect command all you have to do is `/co i`again!

## USING THE ROLLBACK COMMAND

The rollback feature is used to rollback all the blocks within a certain radius from you, mostly used when something gets griefed The command itself looks quite difficult but it gets easier once you get the hang of it. Here's the command `/co rb u:(user) t:(time) r:(radius) a:(action) b:(blocks e:(exclude)` Here's what everything means!

* u:\(user\) specifies the user the rollback is for
* t:\(time\) specifies the amount of time you want to rollback, this is done in weeks \(w\), days \(d\), hours \(h\), minutes \(m\) and seconds \(s\). For example this can turn into `t:1w,2d,4h,30m,2s`
* r:\(radius\) specifies what you want to rollback, this can be the number of blocks \(r:10\), a specific world \(r:\#world\_nether\), a selected worldedit \(r:\#we\) or globally \(r:\#global\)
* a:\(action\) specifies the specific action you want to rollback, though there are quite a few actions you can specify, I'll only mention a few here, blocks placed \(a:+block\), items taken out of a container \(a:-container\) or mobs killed \(a:kill\) are just a few examples of the many actions out there!
* b:\(blocks\) specifies which blocks you want to rollback specifically, if you want to rollback cobblestone and dirt for example this will turn into `b:4,3`\(list of IDs can be found here [https://gamedb.gg/games/minecraft/item-ids-item-spawning-guide/](https://gamedb.gg/games/minecraft/item-ids-item-spawning-guide/)\)
* e:\(exclude\) specifies the blocks you want to exclude from the rollback, so if you want everything except a certain block to be rollbacked, you use this. So if you don't want obsidian to be rollbacked for example you use `e:49`

## EXTRA

There are a few other commands besides the ones mentioned above, one of them being `/co purge t:(time) r:(world)`. What this does is delete the data stored by CoreProtect, this being things you can see in core inspect or everything you can rollback. It's useful to clear this out sometimes because it can lag the server, the highest you can delete with this is one month.

{% hint style="success" %}
Join our **[Discord](https://discord.gg/TYhH5bK)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}
