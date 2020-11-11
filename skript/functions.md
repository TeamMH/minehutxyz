---
description: Learn how to use functions in Skript!
---

# Functions

## **OVERVIEW**

Learn how to use functions in Skript!

## **WHAT ARE FUNCTIONS**

Functions are used to perform tasks, and most languages have them. Functions are global across scripts.

## **COMPONENTS OF A FUNCTION**

You have 4 parts of a function: The name, the parameters, the return type, and the code it runs. The name is what you call the function with, and the parameters are like command arguments, they can be ANYTHING, including objects. To access the value of a parameter, you use the local variable `{_%parameter name%}`, if the parameter was plural \(ex. `objects`, `strings`, `numbers`\), you would use `{_%parameter name%::*}`. Plural parameters can also be specified with only one thing. In that case, the variable used to access the value will still be `{_%parameter name%::*}`, it'll just be set to the one value. Your function does not need to have parameters.

The return type can also be anything, just like a parameter. It also does not need to be specified, but if you are gonna return something, you have to specify.

{% hint style="danger" %}
If you're returning something, there **cannot** be a delay.
{% endhint %}

## **HOW TO MAKE FUNCTIONS**

The typical function looks like this:

```text
# Do not put [ :: return type] if you aren't returning anything.
function name(parameter_name: parameter_type) :: return type:
    # code to be ran
```

You can call a function in your code by putting `function_name(parameters, if any)`. In order to save the output of a function, use `set {_var} to name(parameters)`.

## **EXAMPLES**

```text
function say_hi(p: player):
    send "Hi there!" to {_p}

on join:
    say_hi(player)
```

```text
function kill(victim: player, attacker: player):
    make {_victim} respawn
    add 1 to {deaths::%{_victim}%}
    add 1 to {kills::%{_attacker}%}
    send "&cYou were killed by %{_attacker}%&c!" to {_victim}
    send "&aYou killed %{_victim}%&a!" to {_attacker}

on death:
    kill(victim, attacker)
```

{% hint style="success" %}
Join our [**Discord**](https://discord.gg/TYhH5bK) to become an **official writer**, **site updates**, and **much more**.
{% endhint %}

