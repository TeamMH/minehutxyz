---
description: Learn how to use variables in Skript!
---

# Variables

## **WHAT ARE VARIABLES**

Variables are Skript's way of storing data, every variable has a name and value \(i.e, stored data\).

## **TYPES OF VARIABLES**

There are 5 types of variables: 'normal' variable, local variable, list variable, an option, and metadata tags.

* **Normal variables are like envelopes, they can only hold one thing.** You can set them to anything, but you cannot set them to multiple values. They look like `{variable}`, `{pog.champ}`, etc. 
* **Local variables** are variables that are saved, they are only saved in the trigger they are saved in, and cannot be accessed in other triggers. You can define a variable as local by putting a underscore \(\_\) before the variable's name, if done correctly, they look like `{_local.variable}`, `{_local}`, etc. They don't necessarily have to have a name, you can make a local variable named `{_}`.if you want. 
* **List variables** are like cardboard boxes, they can hold multiple values, and they can also be combined with local variables to become local list variables. List variables are slightly more complicated than normal variables. List variables can hold multiple values IF they end with`::*`, some examples of this are `{list::variable::*}`, `{_local::*}`, etc. A list variable can only hold one value if it has `::`in it, but no \* after. You can not make a list variable that ends with two colons and no asterisk, and you can't make a local list variable named `{_::*}`.

Options are 'variables' that you define at the top of your code. It looks like

```text
options:
    option1: pogchamp
    option2: hjonk
```

They can be used in your code by putting `{@(option name)}`, and they can be more than just strings and numbers. Skript parses them as if they are typed in your code normally. You could put any syntax in there, and if done correctly, Skript will accept it. An example of sending something to a player with an option:

```text
options:
    send: send "Hey there!" to player

on join:
    {@send}
```

## METADATA TAGS

Metadata tags can be attached to blocks and entities, and they are flushed after the server restarts. This is the syntax for metadata tags:

```text
metadata [(value|tag)[s]] %strings% of %metadataholders%
%metadataholders%'[s] metadata [(value|tag)[s]] %string%
```

Metadata holders are anything that can hold metadata. \(eg. an entity or block.\) Metadata tags can only hold data such as strings, numbers, integers, booleans \(true/false\), etc. They cannot store entities, and they can only hold one value. The %strings% you see in the syntax is the name of the metadata tags.

An example of using a metadata tag follows as such:

```text
on join:
    set metadata value "name" of player to player's name
    set metadata value "epic" of player to true
```

You can use variables like `{yes.no}`, but it is better practice to specify them as `{yes::no}`. List variables provide more functionality compared to 'normal' variables because you can do mass deletion, sorting, looping, and more with them.

## **HOW TO USE VARIABLES**

Using variables is fairly simple, and I've pretty much already summed it up above.

```text
set {_local} to player
set {_bonk} to "hello!"
set {greetings::*} to "hi", "hello", "hey", and "howdy"
set {pog.champ} to true
set metadata value "nerdiness-level" of player to 1
```

{% hint style="success" %}
Join our [**Discord**](https://discord.gg/TYhH5bK) to become an **official writer**, **site updates**, and **much more**.
{% endhint %}

