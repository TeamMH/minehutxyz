---
description: Learn how to use GroupManager.
---

# GroupManager

### _This tutorial was submitted by Goose. Find out how you can submit a tutorial_ [_here_](../contribute.md)_._

## **OVERVIEW**

GroupManager is an easy to use permission manager for controlling your server. You can create groups, assign permissions to groups and user, and much more!

## **GROUPS**

You can create a group by performing the command `/mangadd (new group name)`, after we've made the group, we can now modify the group! To give a user a group, run the command `/manuadd (player) (group)`, and to remove a user from a group, run `/manudel (player)` To delete a group, run `/mangdel (group name)`.

To list all the groups you've created, run `/listgroups`.

## **PERMISSIONS**

To add permissions to a group, run `/mangaddp (group name) (permission) [permission2] [permission3 ...]`. To remove permissions from a group, run `/mangdelp (group name) (permission) [permission2] [permission3 ...]`.

To add permissions to a user, run `/manuaddp (player) (permission) [permission2] [permission3 ...]`. To remove permissions from a user, run `/manudelp (player) (permission) [permission2] [permission3 ...]`.

#### **MODIFYING PERMISSIONS EXAMPLE**

`/manuaddp UntitledGoose honk.bonk` `/mangaddp owner permission1 permission2` `/mangdelp owner permission2`

## **PREFIXES AND SUFFIXES**

To add a prefix/suffix to a group, run `/mangaddv (group name) (prefix OR suffix) (value)`. To add a prefix/suffix to a user, run `/manuaddv (player) (prefix OR suffix) (value)`.

To remove a prefix/suffix to a group, run `/mangdelv (group name) (prefix OR suffix) (value)`. To remove a prefix/suffix to a user, run `/manudelv (player) (prefix OR suffix) (value)`.

For the prefixes and suffixes to show up in chat, you'll need Vault and a chat format plugin. One chat plugin is EssentialsChat, which also requires EssentialsX to work. You can change the chat format in the config.yml for the Essentials folder, located at `/plugins/Essentials/config.yml` in your File Manager, once you edit the config.yml file, you can press Save and then run `/ess reload`.

#### **PREFIXES AND SUFFIXES EXAMPLE**

`/manuaddv UntitledGoose prefix &e[&fHONK&e]` `/mangdelv owner suffix &cawesome`

## **OTHER COMMANDS**

You can get a list of commands [here](https://www.spigotmc.org/resources/groupmanager-1-7-1-16.40615/)!

### \_\_

{% hint style="success" %}
Join our **[Discord](https://invite.gg/minehutxyz)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}

