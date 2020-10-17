---
description: Learn how to format your text in Skript
---

# Text Formatting

## Coloring

You can set the color of your text two ways: color codes, and hex codes.
There are 16 color codes:
**&0 BLACK**, **&1 DARK BLUE**, **&2 DARK GREEN**, **&3 AQUA**, **&4 DARK RED**, **&5 DARK PURPLE**, **&6 GOLD**, **&e YELLOW**, **&f WHITE**
**&7 LIGHT GRAY**, **&8 DARK GRAY**, **&9 LIGHT BLUE**, **&a LIGHT GREEN**, **&b LIGHT BLUE**, **&c LIGHT RED**, **&d LIGHT PURPLE**

You can use these color codes by putting a "&" and then the number/letter right after.
You can use hex codes by putting "<##", a hex code (a 6 digit hexadecimal string), and a closing ">".

## Markdown

You can change the style of your text by making it bold, italics, obfuscated, and more!
There are 6 'markdown codes':
**&k OBFUSCATED**, **&l BOLD**, **&o ITALICS**
**&n UNDERLINE**, **&m STRIKETHROUGH**, **&r RESET**

You can use these the same way you'd use color codes.

## Text Attributes

With text attributes, you are able to do many things, for example, text that brings you to a link when clicked, or text that makes the player execute a command when clicked!
There are 4 types of attributes: url, cmd, suggest command, and tooltip. This is what each one does:
url; Requests to open a link in the user's browser when clicked
cmd; Makes the user execute a command when clicked (Note that you must put a / before the command name to make the command execute, otherwise the player will say the name in chat.)
suggest command; When clicked, it opens the user's chat and puts a command when clicked, but does not automatically execute it.
tooltip; When hovering over text, a blurb of text will appear.

In order to use them, you wanna put "<the attribute you want to use:value of the attribute>." In order to prevent future text from having the attribute, put a "<r>" (or "<reset>") in front of the text you want to have the attributes.

Here are some images of the attributes in action:

![](../.gitbook/assets/cmd.png)
![](../.gitbook/assets/suggest.png)
![](../.gitbook/assets/url.png)
![](../.gitbook/assets/tooltip.png)

{% hint style="success" %} Join our Discord to become an official writer, receive site updates, and much more. {% endhint %}
