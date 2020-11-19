---
description: JSON Load Common Error
---

# J-SON Read

## OVERVIEW

This error is normally caused by a corrupted json file.

## ERROR EXAMPLE

```text
[Server thread/ERROR]: Encountered an unexpected exception
java.lang.NullPointerException: null
    at net.minecraft.server.v1_16_R3.JsonList.load(JsonList.java:192) ~[spigot.jar:git-Paper-261]
```

The main thing you're looking for is the `JsonList.load` keyword.

## FIX

1. Delete `ops.json`, `whitelist.json`, `banned-ips.json`, `usercache.json` and `banned-players.json`. Make sure to **delete the whole file** and not just the content of them.
2. Restart your server.
3. You may need to re-op, re-whitelist, or re-ban users.

