---
description: 'Learn how to use Skript. [https://skriptlang.github.io/Skript/]'
---

# Basics

![](../.gitbook/assets/skript.jpg)
{% hint style="warning" %}
**Visit our** [**partner YouTube channel**](https://www.youtube.com/channel/UCgXFIH9h2Vf9Q1e86n_FVJA) **for even more tutorials!**
{% endhint %}

## OVERVIEW

Skript is a plugin that allows you to customize Minecraft's mechanics with simple scripts written in plain English sentences. You can easily create complex custom commands, triggers that execute effects under certain conditions, and scripts that just run periodically - all without having to know even the slightest bit about programming! The \(hopefully\) intuitive language has the advantage that you don't even need to learn much to be able to use Skript.

## VIEWING & ADDING SCRIPTS

To add/edit scripts, you'll need to navigate to your File Manager. Then, `Plugins -> Skript -> scripts`. This is where you'll spend most of your time while using Skript.

## SCRIPTING

Scripting is the term we use when writing code in Skript. **For a very detailed tutorial on scripting, visit our** [**partner YouTube channel**](https://www.youtube.com/channel/UCgXFIH9h2Vf9Q1e86n_FVJA)**.**

Firstly we will create a new file, let's name it `example.sk` _\(note, all scripts must end in **.sk**\)._ From here, we will want to edit this file. In this tutorial, we're going to be creating a welcome message that will be displayed to all users _\(eg, "Welcome {player} to the server!"\)_.

Now let's get to coding. We will start with the `on join:` event. This event triggers every time a player joins your server. _\(Read more about events_ [_here_](events.md)_\)._ After this, take a new line, then hit the TAB key, to indent one tab in _\(Read more about indentation_ [_here_](indentation.md)_\)**.**_ Now, we will want to use the `send "Welcome to the server."` effect. This will send any text we want to the user. Here's how the code will look.

```text
on join:
    send "Welcome to the server."
```

## RELOADING THE SCRIPT

After typing the code, you'll want to save the file _\(save button at the bottom-right of the webpage!\)_. Now, go in-game, and now we need to reload the script. To do this, we run the command `/sk reload (file name)`. In this case, we can use `/sk reload example`. If your code has been written correctly, you'll get a success message, with zero error messages.

## TESTING THE SCRIPT

Now that you've reloaded your script, once you join your server you will receive a welcome message saying "Welcome to the server.".

{% hint style="success" %}
Join our **[Discord](https://discord.gg/TYhH5bK)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}
