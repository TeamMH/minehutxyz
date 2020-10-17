---
description: Learn how to read and use syntax.
---

# Syntax

## What is syntax?

Syntax defines the way to write code with Skript, if you use invalid syntax, your code will error.

## How do I read syntax?

Let's use the following syntax as an example:
```
make %players% (say|send [the] message[s]) %strings%
force %players% to (say|send [the] message[s]) %strings%
```
As you can see, there are multiple syntaxes. You can use either syntax you want, let's learn how to read it!

1. The parts with no brackets or percent signs around them are required in your code, you can not leave them out or change them!
2. The parts with brackets (**[ ]**) are OPTIONAL, you do not need to put those parts in your code, but you can if you want!
3. The parts with parentheses (**( )**) are OPTIONS, you can use either option. Options are separated by pipes (**|**), this is easy to understand in our example syntax. Looking at **(say|send)** says that you can either put **say** or **send**.
4. The parts with percent signs (**% %**) are EXPRESSIONS, you have to fill this in yourself. In this case, you'd fill it in with a string. (ex. "hello!")

Note that you can optional parts of syntax in options, and vice versa! This occurs in our example syntax.

## Examples

Syntax:
```
send [the] action bar [with text] %string% to %players%
```
Code:
```
send action bar "hello!" to all players
```

Syntax:
```
break %blocks% [naturally] [using %itemtype%]
```
Code:
```
break target block using player's tool
```

Syntax:
```
broadcast %strings% [(to|in) %worlds%]
```
Code:
```
broadcast "Hey there!" and "Hello!" in world "world"
```

{% hint style="success" %}
Join our **[Discord](https://invite.gg/minehutxyz)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}

