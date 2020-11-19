---
description: Official Minehut.xyz API Documentation
---

# API Documentation

## **OVERVIEW**

Our API allows developers to utilize our articles for their own use.

The API is currently updated manually, so please make a bug report on our [github](https://github.com/TeamMH/minehutxyz/issues/new/choose).

## ARTICLES FULL

{% hint style="success" %}
**`api.minehut.xyz/articles`**
{% endhint %}

* Returns the article list, and all details regarding the articles currently on the API.
* Contains **FAQs** and **plugins**. _\(Skript has it's_ [_own endpoint_](https://minehut.xyz/api#skript-full)_\)_

### RETURNS

```text
{
  "articles": [
    "logs",
    "plugins"
  ],
  "logs": {
    "title": "Logs",
    "description": "How to retrieve your latest.log",
    "path": "/faq/panel/logs",
    "url": "https://minehut.xyz/faq/panel/logs",
    "type": "faq"
  },
  "plugins": {
    "title": "Installing Plugins",
    "description": "Learn how to manage plugins on your Minehut server.",
    "path": "/faq/panel/plugins",
    "url": "https://minehut.xyz/faq/panel/plugins",
    "type": "faq"
  }
}
```

_Note: this is a very short example, the API contains much more than these 2._

## SPECIFIC ARTICLE

{% hint style="success" %}
**`api.minehut.xyz/articles?article={article}`**
{% endhint %}

* **Example \| `api.minehut.xyz/articles?article=logs`**
* Returns information on the specified article.

### RETURNS

```text
{
  "title": "Logs",
  "description": "How to retrieve your latest.log",
  "path": "/faq/panel/logs",
  "url": "https://minehut.xyz/faq/panel/logs",
  "type": "faq"
}
```

## SKRIPT FULL

{% hint style="success" %}
**`api.minehut.xyz/skript`**
{% endhint %}

* Returns the article list, and all details regarding the articles currently on the API.
* Contains **only skript**.

```text
{
  "skripts": [
    "basic",
    "events",
    "indentation",
    "commands",
    "variables",
    "functions",
    "comments",
    "syntax",
    "formatting-text"
  ],
  "basic": {
    "title": "Basics",
    "description": "Learn how to use Skript. [https://skriptlang.github.io/Skript/]",
    "path": "/skript/basics",
    "url": "https://minehut.xyz/skript/basics",
    "type": "skript"
  },
  "events": {
    "title": "Events",
    "description": "Learn how events work.",
    "path": "/skript/events",
    "url": "https://minehut.xyz/skript/events",
    "type": "skript"
  }
```

_Note: this is a very short example, the API contains much more than these 2._

