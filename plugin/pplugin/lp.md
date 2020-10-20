---
description: Learn how to use LuckPerms.
---

# LuckPerms

### _This tutorial was submitted by PandaChan. Find out how you can submit a tutorial_ [_here_](../contribute.md)_._

## OVERVIEW

Luckperms is a group managing plugin that is usually recommended to be used on Minehut, it gets actively updated so most bugs won't be there for too long!

## DEPENDENCIES

This plugin does not have any dependencies right out of the box, but you'll want to note that if you would like to use prefixes and suffixes, you'll need Essentials, EssentialsChat and Vault. 

## SETUP

LuckPerms has an online editor that you can learn more about with [here!]()and an ingame editor \(uses commands\) but today I'll mostly be explaining all the commands The group we will be creating will be called 'Example' but you can name this whatever you want, keep in mind that there is already a default group that exists, if you want to add permissions to that group just skip to the giving permissions part.

## CREATING A GROUP

First of is the most important thing about using a group managing plugin, creating a group! To create a group all you have to do is: `/lp creategroup (group)` So in our case this will turn into: `/lp creategroup Example`

## ADDING A PREFIX

A prefix is a short tag infront of someone's name, usually this is used to display a user's rank. To give someone a prefix you have to do: `/lp group (group) meta setprefix (prefix)`

For us this will become: `/lp group Example meta setprefix "[Example] "` 

You can use any colour codes for this, just add it before the prefix and it should show a fancy colour ingame!

## ADDING PERMISSIONS

Permissions are quite important for a server, this allows users to execute certain commands from a plugin. To find the permission nodes you need for a certain plugin you can look up '\(plugin\) permission nodes' on Google, today I'll be using Essentials nodes as example. To set a certain permission for a group you do: `/lp group (group) permission set (node) true`

For us this turns into: `/lp group Example permission set essentials.home true` 

This allows users from this group to use the command /home, this can be changed into any permission node you want to give the group.

## ADDING USERS TO GROUPS

Now that the group has been created, a prefix has been added and any permission nodes have been given to the group, users should be added to the group. To add a user to a group all you have to do is: `/lp user (user) parent set (group)` 

So for us this will turn into: `/lp user Steve parent set Example`

## EXTRA INFORMATION

Now everything should be set up, of course there is much more to this plugin than just these commands, any other commands can be found [here](https://github.com/lucko/LuckPerms/wiki/Command-Usage).

I also **highly** recommend checking out the online editor, this can be found using `/lp editor`in game and is a lot easier to use!

{% hint style="success" %}
Join our **[Discord](https://discord.gg/TYhH5bK)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}
