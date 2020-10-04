---
description: Learn how to use PermissionsEx.
---

# PermissionsEx

![](../.gitbook/assets/ezgif.com-webp-to-png.png)

## OVERVIEW

PermissionsEx is an easy to use Permission Manager which you can use on your server to create groups, add permissions, and many more. 

## MUST DO

Before starting to create groups with PermissionsEx, you need to give yourself a certain permission node _\(even if you're op!\)_. 

In the console, run the command `/pex user <your name> add permissions.*` . Then do `/pex reload` in console too. Now you have permission to do the PermissionsEx commands in game**.**

## CREATING GROUPS

To create a group, run the command `/pex group <group> create`. After creating a group, we can start adding permissions to the created group. To add yourself or someone to the group, do  `/pex user <username> group set <rank>`

## ADDING AND REMOVING PERMISSIONS

You can add permissions to groups or certain users. `/pex user/group <user/group> add/remove <permission> [world]`. The world is not needed but if specified, it will give the user the permission in only the certain world. If not specified, it will give the user or group permission in all worlds. In place of &lt;user/group&gt;, put the group or user you want want to add or remove the permission from. Doing `/pex user <user>` or `/pex group <group>` will show you a list of permissions from that group or permission.

#### ADDING AND REMOVING PERMISSIONS - Example

`/pex user _Tarna_ add essentials.kits.starter (Adds permission to user)  
/pex user _Tarna_ remove essentials.kits.starter (Removes permission from user)`

  
`/pex group default add essentials.kits.default (Adds permission to group)  
/pex group default remove essentials.kits.default (Removes permission from group)`

## PREFIXES AND SUFFIXES

You can add prefixes and suffixes to your created groups or even certain players. The command to add prefixes is `/pex user/group <user/group> prefix set "PREFIX"` and the command to add suffixes is`/pex user/group <user/group> suffix set "SUFFIX"`. If you want the prefix or suffix to be added to a group, use group and specify the group. If you want it for a player, use user and specify which user. For these prefixes and suffixes to show up in the chat, you need 2 additional plugins. Vault and some sort of Chat Format plugin. An example of a chat format plugin is EssentialsChat, which also needs EssentialsX. You can change the chat format in the essentials config.yml file. After editing the file, save it and do `/ess reload` for the changes to be saved.

#### PREFIXES AND SUFFIXES - Examples

`/pex user _Tarna_ prefix set "&cOWNER" (Adds prefix to user)`  
`/pex user _Tarna_ suffix set "&aBEST" (Adds prefix to user)`  
  
`/pex group admin prefix set "&4ADMIN" (Adds prefix to group)`  
`/pex group vip suffix set "&dDONATOR" (Adds prefix to group)`

## COMMANDS AND PERMISSIONS

#### Utility Commands

| Command | Permission | Description |
| :--- | :--- | :--- |
| pex | permissions.manage | Display help |
| pex toggle debug | permissions.debug | Enable/disable debug mode |
| pex user &lt;user&gt; toggle debug | permissions.debug.&lt;user&gt; | Enable/disable debug mode on one specific user |
| pex user &lt;user&gt; check &lt;permission&gt; | permissions.manage.&lt;user&gt; | Checks 1 specific permission against 1 specific user |
| pex reload | permissions.manage.reload | Reload the pex environment |
| pex config  \[value\] | permissions.manage.config | Print  value from plugin configuration. Specify \[value\] to set a new value |
| pex backend | permissions.manage.backend | Print the currently used backend |
| pex backend  | permissions.manage.backend | Change the permissions backend on-the-fly |
| pex hierarchy | permissions.manage.users | Print the complete user/group hierarchy |
| pex import  | permissions.manage.dump | Import users/groups from selected format |
| pex users cleanup  \[threshold\] | permissions.manage.users.cleanup | Remove "dead" users from the file. \[threshold\] is in days and defaults to 30 |

#### World Inheritance Management

| Command | Permission | Description |
| :--- | :--- | :--- |
| pex worlds | permissions.manage.worlds | Print the worlds PEX and the server know of |
| pex world  | permissions.manage.worlds | Print the  inheritance info |
| pex world &lt;world&gt; inherit &lt;parentWorlds&gt; | permissions.manage.worlds.inheritance | Set the parent worlds for .  can be just one world, or a comma-separated list of worlds. |

#### User Commands

| Commands | Permissions | Description |
| :--- | :--- | :--- |
| pex users list | permissions.manage.users | List all users defined in the permissions file |
| pex users | permissions.manage.users |  List all users defined in the permissions file \(alias to `users list`\) |
| pex user | permissions.manage.users |  List all users defined in the permissions file \(alias to `users`\) |

#### User's Permission Management

| Commands | Permissions | Description |
| :--- | :--- | :--- |
| pex user | permissions.manage.users | List the registered users |
| pex user  | permissions.manage.users.permissions.&lt;user&gt; |  List the permissions for &lt;user&gt; \(alias to `user <user> list`\) |
| pex user &lt;user&gt; prefix \[newprefix\] | permissions.manage.users.prefix.&lt;user&gt; | Get or set the prefix for &lt;user&gt; |
| pex user &lt;iser&gt; suffix \[newsuffix\] | permissions.manage.users.suffix.&lt;user&gt; | Get or set the suffix for &lt;user&gt; |
| pex user &lt;user&gt; delete | permissions.manage.users.&lt;user&gt; | Remove &lt;user&gt; from the permissions file |
| pex user &lt;user&gt; list \[world\] | permissions.manage.users.permissions.&lt;user&gt; | List the permissions for &lt;user&gt;. Shows the permissions assigned to the user directly as well as those assigned via the group the user is a member of. Specify \[world\] to list the users permission for a single world |
| pex user &lt;user&gt; add &lt;permission&gt; \[world\] | permissions.manage.users.permissions.&lt;user&gt; | Add &lt;permission&gt; to &lt;user&gt;. Specify \[world\] to grant/deny permission only in \[world\] |
| pex user &lt;user&gt; remove &lt;permission&gt; \[world\] | permissions.manage.users.permissions.&lt;user&gt; | Remove  from . Specify \[world\] to remove permission only from \[world\] |
| pex user &lt;user&gt; timed add &lt;permission&gt; &lt;lifetime in seconds&gt; \[world\] | permissions.manage.users.permissions.timed.&lt;user&gt; | Add timed &lt;permission&gt; to &lt;user&gt; for &lt;lifetime in seconds&gt; in \[world\] |
| pex user Muser&gt; timed remove &lt;permission&gt; &lt;lifetime in seconds&gt; \[world\] | permissions.manage.users.permissions.timed.&lt;user&gt; | Remove timed &lt;permission&gt; to &lt;user&gt; for &lt;lifetime in seconds&gt; in \[world\] |
| pex user &lt;user&gt; set &lt;option&gt; &lt;value&gt; \[world\] | permissions.manage.users.permissions.&lt;user&gt; | Set &lt;option&gt; to &lt;value&gt;. Set value to "" \(two double quotes\) if you want to remove the &lt;option&gt;. Specify \[world\] to set &lt;option&gt; only in \[world\] |

#### User's Group Management

| Commands | Permissions | Description |
| :--- | :--- | :--- |
| pex user &lt;user&gt; group list | permissions.manage.membership.&lt;user&gt; | List all groups the &lt;user&gt; is currently in |
| pex user &lt;user&gt; group add &lt;group&gt; \[world\] \[lifetime\] | permissions.manage.membership.&lt;group&gt; | Add &lt;user&gt; to &lt;group&gt;.  Optional param `lifetime` \(in seconds\) is used to make timed membership. You can replace world by '\*' if the group of the user is applied for all worlds and you want applied a lifetime. |
| pex user &lt;user&gt; group set &lt;group&gt; \[world\] | permissions.manage.membership.&lt;group&gt; | Set &lt;user&gt; group to &lt;group&gt;. Note that this command removes the user from any other groups they are a member of. |
| pex user &lt;uesr&gt; group remove &lt;group&gt; \[world\] | permissions.manage.membership.&lt;group&gt; | Remove &lt;user&gt; from &lt;group&gt; |

#### Default Groups Management

| Commands | Permissions | Description |
| :--- | :--- | :--- |
| pex default group \[world\] | permissions.manage.groups.inheritance | Print the default groups for specified world. If \[world\] is not specified, it will apply to the global config. |
| pex set default group &lt;group&gt; &lt;value&gt; \[world\] | permissions.manage.group.inheritance | Set the default flag of &lt;group&gt; in \[world\]. Any number of groups can have this flag set. If \[world\] is not specified, it will apply to the global config. &lt;value&gt; is boolean 'true' or 'false'. |

#### Group Commands

| Commands | Permissions | Description |
| :--- | :--- | :--- |
| pex group | permissions.manage.group.list |  List all registered groups \(alias to `groups list`\) |
| pex groups | permissions.manage.group.list | List all registered groups \(alias to `groups list`\) |
| pex groups list | permissions.manage.group.list | List all registered groups |
| pex group &lt;group&gt; prefix \[newprefix\] | permissions.manage.groups.prefix.&lt;group&gt; | Get or set the prefix for &lt;group&gt; |
| pex group &lt;group&gt; suffix \[newsuffix\] | permissions.manage.groups.suffix.&lt;group&gt; | Get or set the suffix for &lt;group&gt; |
| pex group &lt;group&gt; create \[parents\] | permissions.manage.groups.create.&lt;group&gt; | Create &lt;group&gt;. Specify \[parents\] to set the groups it inherits from |
| pex group &lt;group&gt; delete | permissions.manage.groups.remove.&lt;group&gt; | Remive &lt;grouo&gt; |
| pex group &lt;group&gt; parents list | permissions.manage.groups.inheritance.&lt;group&gt; | List the parents for &lt;group&gt; |
| pex group &lt;group&gt; parents set &lt;parents&gt; | permissions.manage.groups.inheritance.&lt;group&gt; | Set the parent\(s\) for &lt;group&gt; \(single or comma-separated list\) |
| pex group &lt;group&gt; | permissions.manage.groups.permissions.&lt;group&gt; | List all &lt;group&gt; permissions  \(alias to `group <group> list`\) |
| pex group &lt;group&gt; list \[world\] | permissions.manage.groups.permissions.&lt;group&gt; | List all permissions for &lt;group&gt;. Specify \[world\] to list the group's permissions for \[world\] |
| pex group &lt;group&gt; add &lt;permission&gt; \[world\] | permissions.manage.groups.permissions.&lt;group&gt; | Add &lt;permission&gt; to &lt;group&gt; |
| pex group &lt;group&gt; remove &lt;permission&gt; \[world\] | permissions.manage.groups.permissions.&lt;group&gt; | Remove &lt;permission&gt; from &lt;group&gt;. Specify \[world\] if this permission should be removed only in \[world\] |
| pex group &lt;group&gt; timed add &lt;permission&gt; \[lifetime\] \[world\] | permissions.manage.groups.permissions.timed.&lt;group&gt; | Add timed &lt;permission&gt; to &lt;group&gt; with \[lifetime\] in \[world\] |
| pex group &lt;group&gt; timed remove &lt;permission&gt; \[world\] | permissions.manage.groups.permissions.timed.&lt;group&gt; | Remove timed &lt;permission&gt; for &lt;group&gt; in \[world\] |
| pex group &lt;group&gt; set &lt;option&gt; &lt;value | permissions.manage.groups.permissions.&lt;group&gt; | Set &lt;option&gt; &lt;value&gt; for &lt;group&gt;. Set value to "" \(two double-quotes\) if you want to remove the &lt;option&gt;. Specify \[world\] if the option should be set only in \[world\] |
| pex group &lt;group&gt; weight &lt;weight&gt; | permissions.manage.groups.weight.&lt;group&gt; | Prints the weight value of  &lt;group&gt; in 'calories' where a lower value has _more_ priority than a group with a higher value. i.e., 1 has more priority than 2, 2 more than 3, etc. If \[weight\] is defined when using this command, sets the weight value of &lt;group&gt; to \[weight\]. |

#### Group's User Management

| Commands | Permissions | Description |
| :--- | :--- | :--- |
| pex group &lt;group&gt; users | permissions.manage.membership.&lt;group&gt; | List all uesrs in &lt;group&gt; |
| pex group &lt;group&gt; user add &lt;user&gt; | permissions.manage.membership.&lt;group&gt; | Add &lt;user&gt; to &lt;group&gt; \(single or comma-seperated list\) |
| pex group &lt;group&gt; user remove &lt;user&gt; | permissions.manage.membership.&lt;group&gt; | Remove &lt;user&gt; from &lt;group&gt; \(single or comma-seperated list\) |
| pex promote &lt;user&gt; &lt;ladder&gt; | permissions.user.promote.&lt;ladder&gt; | Promote &lt;user&gt; on &lt;ladder&gt;. If &lt;ladder&gt; is not specified, the default ladder \(named default\) will be used. |
| pex demote &lt;user&gt; &lt;ladder&gt; | permissions.user.demote.&lt;ladder&gt; | Demote &lt;user&gt; on &lt;ladder&gt;. If &lt;ladder&gt; is not specified, the default ladder \(named default\) will be used. |

{% hint style="success" %}
Join our **[Discord](https://invite.gg/minehutxyz)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}



