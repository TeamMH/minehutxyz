# Custom Domain 

---
description: How to connect a custom domain to your Minehut server.
---

#OVERVIEW

This tutorial will show you how to connect your own domain to your Minehut server. For example `mydomain.com` will bring you to your server!

# HOW TO CONNECT YOUR CUSTOM DOMAIN

First, you will need a **custom domain**, for this guide we will be using CloudFlare.

If you are using a different provider than cloudflare. Transfer the **nameservers** to cloudflare and **register** the domain under cloudflare.

Then, When you are in dashboard **click** on your Website, your dashboard should look something like this https://imgur.com/a/LS36LWP.

Third, **Click** on your domain, after doing that you should see this page https://imgur.com/a/lFYRWcN.

After that, **press** on DNS on the top of the website. Then press on **add record**. Under Type choose SRV it must look like this https://imgur.com/a/efJubea.

Finally you must fill out the Fields. Names is what will be used as the ip **@** will be your raw domain example: candymine.tk, you must also set Service to **_minecraft**, Priority **1**, weight **1**, and port **25565** and set Target to **the targeted server** for example: minehut.com. It should look something like this: https://imgur.com/a/FImS97r. Then **press save** now you can join your server through your custom domain!
