---
description: Learn how Skript indentation works.
---

# Indentation

## OVERVIEW

If you experienced the error **"Error: Indentation error at line X, expected X tabs/spaces, but found X tabs/spaces"** or something similar, and you don't know how to fix it, read this tutorial.

## WHAT IS INDENTATION <a id="1-what-is-indentation"></a>

Indentation is placing text in code further to the right, to allow the parser to know this is a different section of the code. Most programming language don't care about indentation, their parser can handle it correctly without, but Skript can't, because of its rich, English-like syntax.  
That's why indentation is really important and you should always take care of it. See an example below.

```text
on script load: 
    if 1 = 1:  # Here I indentated with one tab, to clarify this is the section after the event.
        broadcast "How are you?"  # Here I indentated with two tabs, because this is a section after a condition, that already was indentated.    
```

## WHEN TO INDENT <a id="2-rules-of-indentation"></a>

* After an _event_.

```text
on script load: # Event
    # code
```

* After any _condition_.

```text
if attacker is a player: # Condition
    # code
```

* After any other _section_.

```text
while player is online: # Section
    # code
```

* After any _function_.

```text
function myFunc(): # A function is declared.
    # code
```

* Also, remind that **all** events, conditions, sections, command and functions **need a colon behind them!**

{% hint style="success" %}
Join our **[Discord](https://discord.gg/TYhH5bK)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}
