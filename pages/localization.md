---
title: Localizing Layouts
description: How to localize layout content.
published: true
date: 2023-12-24T08:20:27.143Z
tags: 
editor: markdown
dateCreated: 2023-12-24T07:59:54.994Z
---

# Localizing Layouts

FancyMenu lets you localize text content and even images and other element types.

# Text Content

FancyMenu allows you to add your own localizations to the game.
These can then be used in the **Localize Text** placeholder to localize a text to the current game language.

The following documentation focuses on how to load localizations via FancyMenu's own localization system, but instead of using FancyMenu's system, you can also use **Minecraft's localization system** and load your localizations via resource pack or a resource loader mod.

The **Localize Text** placeholder works with keys from both FancyMenu's and Minecraft's localization systems.

## Adding Text Localizations

To add your own localization files, you first need to create a localization directory in `.minecraft/config/fancymenu/custom_locals/`.
This directory should have a unique name, like your username.

In this case, I will name the directory `keksuccino`.
So now I have my localization directory in `.minecraft/config/fancymenu/custom_locals/keksuccino`.

![](https://user-images.githubusercontent.com/35544624/134380681-59f9bd02-aefd-4b67-9ee4-ca7568d23935.png)

This is the directory where you will put all your localization files.

### The First Localization File

Localization files contain all of your localized text content for different languages.
There's always one localization file per language.

This means that you put the same text content in multiple files, but in different languages.

To make the game being able to find the same localized content across multiple files, you need to give every localization a **unique** key (like an ID).

Because you will most likely not localize your content to every language in the game, you will need a **fallback language** that gets used when the game is set to a language your content is not localized to.

This is why the **first file you need to create** in your localization directory is the `en_us.local` file!
The `en_us.local` (English US) file is always the fallback language, so make sure to add it!

To do this, just open your **localization directory** and **right-click** into the folder to create a new **text document**.

![](https://user-images.githubusercontent.com/35544624/134384066-256c0495-30b6-42b5-95ff-bcb3d34e3f28.png)

> **IMPORTANT:** Now you will need to [turn on file extensions](https://cdn.discordapp.com/attachments/795308330746511390/801561308012347482/unknown.png) on Windows and maybe other systems, to see the `.txt` extension of your newly created text file.
{.is-warning}

Rename this text file to `en_us.local` (make sure to remove the old `.txt` extension).

![](https://user-images.githubusercontent.com/35544624/134384272-6891f062-5f7a-4ba0-bcbc-6c3c6d96924a.png)

Right-click it and click on **Open with -> Choose another app** (on Windows) and search and select the text editor of your choice in the list. Now enable the **Always use this app to open .local files** option at the bottom of the window and click **OK**.

![](https://user-images.githubusercontent.com/35544624/134385052-d569d8b5-ec15-44d2-b103-da7d3f6288a0.png)

Now you can open and edit `.local` files with your normal text editor.

### Localization File Content

You just created your first localization file (**English US**).
This means when the game language is set to English US, your text elements will be localized to the content in the `en_us.local` file (and in the case of this specific file, it will also get used if you don't have a localization file for the current game language).

But the file is still empty, so none of your text elements can get any content from it. Lets change this.

Open your `en_us.local` file with a text editor.

There's always one localization key with its value per text line, so line breaks will not work (and will break the localization file).

To add a new localization, just start with the **unique** key you've chosen for it, followed by an equals sign and the actual value.

![](https://user-images.githubusercontent.com/35544624/134387882-87d163d7-e974-4f42-b736-3e0c0e1f98e6.png)

Keys need to be **unique**, so you can't use the same key for more than one localization **in the same file**.

Just like for the first localization, you can now add more localizations to the localization file.

![](https://user-images.githubusercontent.com/35544624/134388902-b61b0fab-8e79-428b-ad53-3756e0f9fcf1.png)

Now you have your first (and most important) localization file ready to use.

### Adding More Languages

Now you have your text content localized to English, but well, it's **only** localized to English, so it's not really localized yet, right?

Well, no problem! Just like you've created and edited your `en_us.local` file, you can now make files for other languages!

In my example, I will create a file to localize my text content to German.

To do this, I will create a `de_de.local` file in my localization directory.

![](https://user-images.githubusercontent.com/35544624/134390071-97ea159f-5eb0-4695-89e5-6dbfa637c9c5.png)

You've probably noticed at this point that the names of your localization files can't be random.
You always need to use the **correct language code** for the localization file as file name.

If you want to know the correct language code (aka. local code) for a language, check out [this Minecraft wiki page](https://minecraft.fandom.com/wiki/Language).

Now I will add the exact same localizations as in the `en_us.local` file to my new `de_de.local` file, but will translate everything to German.

Make sure to **only translate the value** and **not the key**!

![](https://user-images.githubusercontent.com/35544624/134391225-0e44e7bc-b8bf-4f98-a5bc-d4564ba92686.png)

Now you have your default `en_us.local` file and one or more other localization files with the same content, but in different languages.

You can edit these files later to add more values or to edit existing ones.

## Using Text Localizations

Your localization files are ready now, so lets see if they work.

To use your localizations in text-based elements, you just need to edit the content of a text-based element (like labels of Button elements or Text elements) and click on the **Placeholders** button on the top-right side of the text editor. If there is no such buttton in the editor, then the text content you're editing does **not support** placeholders.

Search for the **Localize Text** placeholder and click on it to paste it to your text content.

Now replace the `localization.key` part of the placeholder with one of your own localization keys.

Well, and that's basically it. The placeholder should get replaced with the actual localized content when not in the text editor.

Keep in mind that the placeholder will always localize the text content to the current game language.

# Non-Text Content (Images, etc.)

FancyMenu also allows you to localize images and basically every element you want.

To do this, you will need to use **loading requirements**.
The **Is Game Language** requirement to be more specific.

The **Is Game Language** requirement allows you to show elements or layouts only if a specific game language is set, so you can, for example, make two Image elements that contains text and localize that image to a version with Japanese text when the language is set to Japanese or a version with English text, if the language is set to English.

To set loading requirements to an **element**, right-click it and click on **Loading Requirements**.

To set loading requirements to **whole layouts**, right-click the layout editor background and click on **Loading Requirements [Layout-Wide]**.