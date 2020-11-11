---
description: An easy to follow, indepth tutorial on the skript addon Vixio.
---

# Vixio - An easy to follow, indepth tutorial on the skript addon.

### *This tutorial was submitted by Centrect. Find out how you can submit a tutorial [_here_](../contribute.md)*

## OVERVIEW

Vixio is a skript addon avaliable on Minehut. Using Vixio you can make advanced links into Minecraft through Discord and vice versa, using a Discord bot.
With Vixio you can send all your minecraft server chat into a discord channel, and vice versa, you can send server reports to a staff channel, you can send suggestions, view online players, all through Discord and Vixio.


## HOW TO DO

Firstly, you are going to want to install Vixio. This tutorial will need a basic knowledge of skript. If you do not know how to use Skript, please follow one of our other tutorials.

https://i.imgur.com/p5RWtBn.png

Next, go to plugins > skript > scripts 
Create a new file, call it anything you like, but at the end make sure it has ".sk" at the end. You have now made your bots skript

On the first line, enter the following:

on skript load: 
    login to "(YOUR BOT TOKEN HERE)" with the name "(YOUR BOT NAME HERE)" # This makes the bot online.
    mark "(Your Bot Name) " as playing "(insert text here)" # This will be the bots status when it is online

(If you need advice on how to create a discord bot, please check out Minehuts official tutorial: https://bit.ly/3lDNLHs)


Next, lets assume you want to send your server chat to a channel in discord. 
Start by creating a dedicated channel for your server chat. 
Next, right click on your channel and click "Copy ID"
Now enter this line of code into your skript file for your bot

on chat:
    send "%player%: %message%" to channel with id "(insert channel ID here" with "(Bot Name Here)"
    
Give that a test and see if it works!

Next, lets make it so whenever someone types a message into your server chat channel, it sends it right into the server.

All you need to do for this one is enter this line of code into your skript file

guild message receive seen by "Evara":
	set {_chat} to channel with id "(insert channel ID here)" 
	if the discord id of event-channel is discord id of {_chat}:
		broadcast "&d&lDISCORD &3> &d%event-member% &7> %event-string%" # You can edit the text inside the quotation marks to be whatever you want. Just ensure that you remember the %event-member% etc
    
(You can edit the text inside the quotation marks on the last line to be whatever you want. Just ensure that you remember the %event-member% etc)
     

Now lets get a bit more advanced.

We are now going to make our bot play music inside a channel, This is very similar to the likes of Groovy and Rythm, but you can make it yourself!

(Full credit for this part goes to the official Vixio discord server.)

discord command play <text>:
    prefixes: /
    executable in: guild
    trigger:
        if arg-1 contains "discord":
            cancel event
            reply with "You cannot play Discord files!" # This actually crashed my server multiple times, therefore I had to block discord files.
        else:
            join voice channel of event-member
            play arg-1
            reply with "▶ Now playing %arg 1%"

discord command pause:
    prefixes: /
    executable in: guild
    trigger:
        pause the track event-bot is playing
        reply with "⏸ Paused!"

discord command resume:
    prefixes: /
    executable in: guild
    trigger:
        resume the track event-bot is playing
        reply with "▶ Resumed!"

discord command stop:
    prefixes: /
    executable in: guild
    trigger:
        stop the track event-bot is playing
        make event-bot leave voice
        reply with "⏹ Stopped!"


discord command info:
    prefixes: /
    executable in: guild
    trigger:
        if event-bot is playing:
            make embed:
                set title of embed to title with text "▶ %discord name of track event-bot is playing%" and link "%url of track event-bot is playing%"
                set the colour of the embed to Cyan
                add field named "Time remaining" with value "%difference between position of track event-bot is playing and duration of track event-bot is playing%" to embed
                add field named "Author" with value "%authors of track event-bot is playing%" to embed
                set the footer of embed to footer with text "(Feel free to edit this to whatever you want)"
                set the timestamp of embed to now
            reply with last created embed
        else:
            make embed:
                set title of embed to title with text "⏹ No track playing"
                set the footer of embed to footer with text "(Feel free to edit this to whatever you want)"
                set the timestamp of embed to now
            reply with last created embed
            
(NOTE: I tried to edit the prefixes, but to no avail, I recommend not touching this part unless you know what you are doing)


Congratulations! You now have a functional discord bot!

Enjoy!


{% hint style="success" %}
Join our **[Discord](https://invite.gg/minehutxyz)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}
