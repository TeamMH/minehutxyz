---
description: Learn how to create a custom /discord command.
---

# Example: /discord | Download this at https://github.com/TeamMh/minehutxyz/blob/master/skript/downloads/discord.sk?raw=true

## OVERVIEW

We will be creating a `/discord` command that will allow users to click the text and it will bring them to your discord.

## CODE

```
command /discord:
  trigger:
    send "&7> Click <link:DISCORD_INVITE>&c&lHERE<reset>&7to join our discord."
```

## EXPLAINED

The command `/discord` will send this message, and we can use `<link:LINK> <reset>` to make the text clickable.
