---
title: Modpacks
description: How to include layouts in a modpack.
published: true
date: 2024-10-19T08:43:52.029Z
tags: 
editor: markdown
dateCreated: 2023-12-22T05:28:46.511Z
---

# FancyMenu in Modpacks

Including your FancyMenu setup in a modpack is very easy and only takes some simple steps.

> This page is **ONLY** for FancyMenu setups made completely in **FancyMenu v3+**, so if you use a legacy setup (made in v2 and converted to v3), some steps could be different.
{.is-warning}

# Including the FancyMenu Setup in Your Modpack

You simply need to include FancyMenu's config folder, that's all.

1. Navigate to the root directory of the Minecraft instance you made your layouts in.
2. Open the `config` folder of the Minecraft instance.
3. Copy the `fancymenu` folder of the `config` folder to your desktop or somewhere else.
4. Navigate to the `config` folder of the **modpack** instance.
5. If there is already a `fancymenu` folder in the `config` folder, **delete** the existing `fancymenu` folder.
6. Move the `fancymenu` folder you copied in **step 3** to the `config` folder of the **modpack** instance.

That's it. Nothing more you need to do.

> Please keep in mind that old legacy setups made in FancyMenu v2 (even if converted to v3) allowed you to store layout assets outside FancyMenu's `/config/fancymenu/assets/` folder, so in that case you need to make sure you also include all of your assets in the modpack.
{.is-warning}

# Disabling the Menu Bar and Hotkeys

You surely don't want to keep FancyMenu's menu bar visible in your modpack, so you should disable it. But since people can still press the hotkey to make it visible again, let's do something a little bit more *aggressive*.

Navigate to `/config/fancymenu/options.txt` and open the file in a text editor.

Now set `modpack_mode` to `true` and save the file.
This will completely disable all overlays and hotkeys.

To be able to edit your layouts again, set the config option back to `false`.

# Disabling the Welcome Screen

This shouldn't be needed in most cases, but if you didn't close the Welcome screen yet (the screen that tells you to read the documentation), make sure to set `show_welcome_screen` to `false` in `/config/fancymenu/options.txt`.

The screen only shows once and disables itself when clicking on the **Open Documentation** button, so again, doing this manually shouldn't be needed in most cases.

<br>
<img width="630" alt="Screenshot_1" src="https://github.com/user-attachments/assets/4383b39f-f55a-4eb8-8142-34a425474bb3">
