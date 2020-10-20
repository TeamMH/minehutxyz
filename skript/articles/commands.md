---
description: Learn how to make commands with Skript!
---

# Commands

### _This tutorial was submitted by Goose. Find out how you can submit a tutorial_ [_here_](../contribute.md)_._

## HOW TO REGISTER A COMMAND

Registering a command is very simple in Skript. This is what a command in Skript can have:

```text
command /name <arguments>: # keep in mind that arguments and the slash before the command name are optional
    (parameters) # parameters are optional, they will be explained in detail later
    trigger:
        # your code
```

## **ARGUMENTS \(optional\)**

Arguments are parts of a command that a user can type out after the command's name. A argument can be anything from basic text to times of the day. They can be anything that is a `type` in Skript, I won't go into what types are here, but you can find a list of types [here](https://docs.skunity.com/syntax/types). The argument can be plural aswell: string -&gt; strings, integer -&gt; integers. An argument cannot use the `object` type.

To make an argument required, surround it with angle brackets like this:  To make an argument optional, surround it with brackets AND angle brackets like this: \[\&lt;\&gt;\]

## **PARAMETERS \(optional\)**

There are many types of parameters that you can use with your code. Here's a list of most, if not all parameters that you can use:

**permission** - A permission required to run the command.

**permission message** - A message sent to the user if they don't have the permission required to use the command.

**cooldown** - A cooldown for the command.

**cooldown bypass** - A permission required to bypass the cooldown of a command. 

**cooldown storage** - A variable that the cooldown is stored in, it will stay even after the server restarts. 

**description** - A description for the command. 

**aliases** - A list of aliases for your command, \(ex. `/alias1, /alias2, /alias3`\), the slash in the aliases is optional. 

**usage** - A message sent to the user if they used the command incorrectly. 

**executable by** - Specifies who can use the command, it can be `console`, `players`, or`console and players`.

## **GETTING INPUTTED ARGUMENTS** 

You can use the syntax below to get the arguments of an entered command!

```text
[the] last arg[ument][s]
[the] arg[ument][s](-| )%number%
[the] (1st|2nd|3rd|4-90th) arg[ument][s]
[the] arg[ument][s]
[the] %type%( |-)arg[ument][( |-)%number%]
[the] arg[ument]( |-)%type%[( |-)%number%
```

#### **Examples**

```text
command discord:
    trigger:
        send "&aYou can join our discord here! https://discord.gg/WjuNvdM"
```

```text
command cake:
    aliases: /getcake, /receivecake, /givemecake
    description: Receive a cake, only usable once per day!
    permission: cake.is_a_lie
    permission message: &cNo cake!
    cooldown: a day
    cooldown message: &cOnly cake once per day!
    cooldown storage: {cake::%player's uuid%}
    cooldown bypass: cake.gobble
    trigger:
        give player cake
        send "&aYou have received cake!"
```

{% hint style="success" %}
Join our **[Discord](https://discord.gg/TYhH5bK)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}
