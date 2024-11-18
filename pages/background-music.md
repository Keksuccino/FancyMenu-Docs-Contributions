---
title: Menu Background Music
description: How to customize the music played in menus.
published: true
date: 2024-08-24T21:12:58.326Z
tags: 
editor: markdown
dateCreated: 2024-03-07T04:34:08.380Z
---

# Menu Background Music

It's possible to replace Minecraft's default menu background music with custom tracks or just disable the normal Vanilla music that plays in menus.

# Disabling Vanilla Music

FancyMenu has multiple ways to disable Vanilla menu music. This can be useful if you plan to play other audio tracks in screens or if you just don't want music to play at all in some screens.

## Globally

If you want no music in menus at all, this is the easiest way to do that.

To globally disable the Vanilla menu music, go to FancyMenu's menu bar at the top of screens and click on **Customization -> Settings** and disable **Play Vanilla Menu in Music**.

<br>
<img width="600" alt="Screenshot_3" src="https://gist.github.com/assets/35544624/d829a35e-f23f-42a9-ad79-193de73b499b">

> Disabling Minecraft's default music will disable it in every screen, not just the current one.
{.is-info}

## Per Screen

If you want more control over where Vanilla menus music should play, you should use the **Music Controller** element. This element gets added to layouts like every other element by **right-clicking the editor background** and then clicking on **New Element -> Music Controller**.

By **right-clicking** the element you can customize what types of music that plays in menus should be disabled (normal menu music and world music that keeps playing in screens that don't pause the game, like the Inventory screen).

> This element supports **loading requirements**, so you have even more control over when Vanilla music should play!
{.is-info}


# Adding Custom Music

Now we can add the actual custom background music.

If you want to play the same custom music in all screens, you should use a **universal layout**, which gets loaded in every screen that has customizations enabled.

When using a universal layout, the music will **continue playing** when going from one menu with the layout enabled to another one with the same layout enabled.

If you want to play different music per screen, use normal layouts.

In this example we will use **universal layouts**.

Add a new **Audio** element to the universal layout, which will act as our background music player.

<br>
<img width="400" alt="Screenshot_2" src="https://gist.github.com/assets/35544624/bddf8f46-47c5-4a00-a6f7-b5ca1df8ae67">

Now add music tracks to it that should play in the background.

<br>
<img width="300" alt="Screenshot_4" src="https://gist.github.com/assets/35544624/824dcb90-3bd5-4c0b-96d0-e581a7c2f9f7">

That's basically it already.
You can also set the Audio element to shuffle mode and change its sound channel if needed.

Save the layout and leave the editor.

# Enabling Customizations for All Menus

We used a **universal layout** in this example, because we want our background music to play in multiple screens.

Since layouts only load in screens that have **customizations enabled**, we need to enable them now for every screen we want our music to play.

To do that, click on **Customization** and enable **Current Screen Customization**.

<br>
<img width="320" alt="Screenshot_5" src="https://gist.github.com/assets/35544624/2f6527b7-ae14-4e82-abc6-3572cc6490b2">

Repeat this for every screen you want your custom background music to play.

And that's it! You now have custom background music in your Minecraft menus!