---
description: Learn how to contribute to Minehut.xyz
---

# Contribute

## How to Contribute

You can contribute to minehut.xyz by making a [pull request at our GitHub](https://github.com/TeamMH/minehutxyz). You will need a GitHub account for this.

## How to make a pull request

To make a pull request, you need to make a fork of the **minehutxyz** repository.

To fork the repository, click the `Fork` button at the top right of the page.

A category is just a folder with the name of the category, navigate to the category you want to add a page to. From here, click `Add file`, and then `Create new file`. Create a file with a short name, and put `.md` after the name, \(ex. `functions.md`, `download-world.md`, etc.\), and then open the file.

From here, you can edit the file. [_**Here's**_](https://raw.githubusercontent.com/TeamMH/minehutxyz/master/template.md) _**our template you must follow.**_

![](.gitbook/assets/example.png)

This is an example page, and this is the source:

```text
---
description: Description
---

# Title

{% hint style="info" %}
This tutorial was made by <name>. Lean how to contribute [here](/contribute.md).
{% endhint %}

## Section 1

Text

## Section 2

Text
```

To add a **description** to your page, add:

```text
---
description: Description for your page!
---
```

To add a **title** to your page, add:

```text
# title for your page
```

To add separate sections for your page, add:

```text
## Section

Put text here
```

You can, of course, put normal markdown in your page aswell. Once you're done making the page, click `Commit new file`.

Now, for Gitbook to register the page, open a file named SUMMARY.md, and then find the category you're adding a page to, and then under it, put `* [Title of your page](category/file-name.md)`. Then commit the file.

Now you can make a pull request! Go to your repository, then click the button labeled `Pull request`, it should be right next to a `Compare` button. Then, click `Create pull request`. Tada! You have made a pull request to our repository, and your page will appear on the Gitbook if we accept it.

{% hint style="warning" %}
Note that you need to delete your fork and refork it to update it. There is no way to auto update it \(unless your editing loccally, which you can learn how to [here](https://docs.github.com/en/free-pro-team@latest/github/collaborating-with-issues-and-pull-requests/syncing-a-fork).
{% endhint %}

