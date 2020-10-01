---
description: Connect a custom domain to your Minehut server.
---

# Custom Domain

### _This tutorial was submitted by Conutik. Find out how you can submit a tutorial_ [_here_](../contribute.md)

## Overview

This tutorial will teach you how to attach your domain to your Minehut server.

## How to connect your domain

First, you will need a **custom domain**, for this guide we will be using CloudFlare.

If you are using a different provider than CloudFlare. Transfer the name servers to CloudFlare and register the domain under CloudFlare.

When you are in your CloudFlare dashboard, click on your domain. You should be redirected to a page that looks like the following:
![](../.gitbook/assets/domain2.png)

Now, you wanna click on "DNS" at the top of the website. Then click "Add Record". Under "Type", choose "SRV". It'll look like this:
![](../.gitbook/assets/domain3.png)

Now you must fill out the fields:
- Names is the ip, @ will be your raw domain. Example: candymine.tk
- You have to set the service to "_minecraft"
- You have to set the priority to 1
- You have to set the weight to 1
- You have to set the port to 25565
- You have to set the target to the targeted server. If you want your domain to point to Minehut's lobby, you'd put "minehut.com", otherwise, put "(your server's name).minehut.gg"

Once your done, it should look something like this:
![](../.gitbook/assets/domain4.png)

After all that, click the Save button. Now you're all done and you can join your server with the custom domain.

{% hint style="success" %}
Join our **[Discord](https://invite.gg/minehutxyz)** to become an **official writer**, **site updates**, and **much more**.
{% endhint %}

