---
description: Official Minehut.xyz API Documenation
---

# API Documenation

## **OVERVIEW**

Our API allows developers to utilize our articles for their own use. 

The API is currently updated manually, so please alert us of any issues on our [github](https://github.com/TeamMH/minehutxyz/issues).

## FULL

{% hint style="success" %}
**`api.minehut.xyz/articles`**
{% endhint %}

* Returns the article list, and all details on the articles on the API.

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

