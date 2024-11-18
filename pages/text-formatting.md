---
title: Text Formatting
description: How to format text with Markdown and Minecraft's formatting codes.
published: true
date: 2024-06-12T08:35:04.774Z
tags: 
editor: markdown
dateCreated: 2023-12-23T10:10:33.171Z
---

# Text Formatting

FancyMenu has lots of features to make text content in layouts *fancier*!

Text elements have full **Markdown** support with some cool extras and most other text content supports **Minecraft's text formatting** system and button labels even have support for **Minecraft's text components** that allow you to use custom Fonts and more.

# Markdown

FancyMenu's **Text elements** have full Markdown support, which means you can format text content by adding special characters to it.

For example, to make text look bold, you add `**` before and after the bold text, so `**Some bold text that's very bold.**` will look like that:
**Some bold text that's very bold.**

FancyMenu's Markdown even has some special stuff that makes it even more powerful!

> Markdown does **NOT WORK** for other text-based stuff like button labels. It only works for **TEXT ELEMENTS**. For everything else, please use [Minecraft's formatting codes](/text-formatting#minecraft-text-formatting).
{.is-danger}


## Fonts

You can show text in a custom font loaded via resource pack by adding `%!!<font_name>%` before the text and `%!!%` after.

A valid font included in the base game is `uniform`, so to display text in the `uniform` font, do this:
`%!!uniform%this is a custom font%!!%`

This will display `this is a custom font` in the `uniform` font.

## Text Color (HEX)

Showing text in a specific HEX color is possible by adding `%<HEX_color>%` before the text and `%#%` after.

A valid HEX color for green is `#77fc03`, so to show text in this color, do this:
`%#77fc03%this text is green!%#%`

This will show `this text is green!` as `#77fc03` (green).

Make sure that the HEX color is starting with `#`!

## Text Alignment

You can align text lines by starting a line with the specific alignment formatting code, then nothing else, then the text lines you want to show with that specific alignment and then the alignment code again on an extra line.

All text content is **left-aligned by default**, so there are only formatting codes for **centered** and **right-aligned**.

### Centered

To center text lines, use the formatting code `^^^`.

Example:
```
This text is not centered.

^^^
This text is centered.
This text is also centered.
^^^

This text is not centered anymore.
```

### Right-Aligned

To show text lines as right-aligned, use the formatting code `|||`.

Example:
```
This text is not right-aligned.

|||
This text is right-aligned.
This text is also right-aligned.
|||

This text is not right-aligned anymore.
```

## Headlines

To show **a line of text** as headline (bigger and underlined), add `# ` (very big), `## ` (big) or `### ` (small) before the text line.

Example:
`## Big Headline`

## Bold

Add `**` before and after text to make it look **bold**.

Example:
`**bold text content**`

## Italic

Add `_` OR `*` before and after text to make it look *italic*.

Example:
`*italic text content*`

## Strikethrough

Add `~` before and after text to make it look ~~strikethrough~~.

Example:
`~strikethrough text content~`

## Hyperlinks

You can add hyperlinks to text content that open a website when clicked.

Text that should appear as [hyperlink](https://google.com) needs to get wrapped in `[ ]`, followed by the actual link wrapped in `( )`.

So if you want to make `example text content` clickable and open `https://example-website.net`, do this:
`[example text content](https://example-website.net)`

## Images

Markdown supports displaying images in text content.

FancyMenu supports Minecraft resources, local resources and web resources in Markdown.

To add an image, start a text line with `![](`, then the [URL, Resource Location or Path to the resource](/resources) and then `)`.

So to show the Web resource `https://example-website.net/image.png`, do this:
`![](https://example-website.net/image.png)`

Images can also be **hyperlinks** by wrapping the whole image text line in a **hyperlink** like that:
`[![](https://example-website.net/image.png)](https://example-website.net)`

> Local resources need to be in `/config/fancymenu/assets/` !
{.is-warning}

## Quote

To format text as a quote, start a text line with `> `.
This will format all following lines as quote until it finds an **empty** line.

Example:
```
This will not look like a quote.

> This will look like a quote.
This will also look like a quote.

This will not look like a quote anymore.
```

## Bullet Lists

To show text as a bullet list like that:
- Entry 1
- Entry 2
  - Sub-Entry

You simply need to start a line with `- `.

Example:
```
- Entry 1
- Entry 2
  - Sub-Entry
```

## Separation Line

To add a separation line to your text that has the width of a whole text line, simply start a line with `---` and then add nothing else.

It will then look something like that:

---

## Code Blocks

Code blocks can help you display text as `plain text` without Markdown trying to format it, or simply to display text in a code-like style without auto-wrapping of text lines.

A single-line code block (between other text) starts and ends with \` , which is actually really difficult to show in a Markdown text..

A line of text containing a single-line code block looks like that:

![single_line_code_block](https://github.com/Keksuccino/FancyMenu/assets/35544624/e78fd38b-7b1a-4f00-9b11-797d964b3b43)

Multi-line code blocks wrap multiple lines in one big code block and start with a line that only contains \`\`\` then the text content and then \`\`\` again:

![multi_line_code_block](https://github.com/Keksuccino/FancyMenu/assets/35544624/bf8c77eb-a97e-48cd-9270-8302c2995856) 

# Minecraft Text Formatting

Minecraft itself has a pretty good formatting system that works similar to Markdown, where you add special characters to your text content to format it.

To read more about Minecraft's formatting system, please take a look at [this Minecraft wiki page](https://minecraft.wiki/w/Formatting_codes).

> The wiki will say the formatting code prefix is `§`, but in FancyMenu you need to replace that with `&`. Everything else stays the same.
{.is-warning}

# Minecraft Text Components

Minecraft's text component system is pretty powerful for **single-line** text content like **button labels**.

In Vanilla Minecraft you can use it in the `/tellraw` and `/title` commands (and probably other places).
It is formatted text serialized to JSON, so you can add formatting attributes to text content.

To learn more about text components in detail, please take a look at [this Minecraft wiki page](https://minecraft.wiki/w/Raw_JSON_text_format).
To learn more about fonts in Minecraft, take a look at [this Minecraft wiki page](https://minecraft.wiki/w/Resource_pack#Fonts).

To make FancyMenu detect a button label as **text component**, set nothing but the serialized component text as label, just like that:
`{"text":"Button Label Text","font":"uniform"}`

The example above will show the button label `Button Label Text` in the `uniform` font.

> You can use FancyMenu's placeholders in the `text` value of components.
{.is-info}
