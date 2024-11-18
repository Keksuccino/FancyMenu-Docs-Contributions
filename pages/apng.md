---
title: APNGs
description: How to make FancyMenu-compatible APNG images.
published: true
date: 2024-05-04T10:06:45.075Z
tags: 
editor: markdown
dateCreated: 2024-01-22T02:45:15.784Z
---

# Animated PNG Images

APNGs are an animated version of PNG images, making it possible to have the same features as with a GIF, but in full, lossless PNG quality!

FancyMenu has built-in APNG support, but it's a bit picky about what APNGs are supported.
It needs **uncompressed** APNGs that are **not interlaced**.

# Making APNG Animations

You would be surprised how difficult it is to find a good APNG editor, especially with options to disable compression and interlacing.

A great choice for an editor is [ScreenToGif](https://www.screentogif.com/), which is actually a tool to record GIFs and APNGs of your screen, but it's also great to make normal APNGs by skipping the record part and directly loading into the editor!

## Open The Editor

The first thing you see after opening [ScreenToGif](https://www.screentogif.com/) is this screen. Click on **Editor** here.

![screentogif_2](https://github.com/Keksuccino/FancyMenu/assets/35544624/a8d34313-b841-4fb6-bf3a-ff02c39792cb)

## Load the Frames

Now you need your PNG frames. Drag-&-Drop them into the editor.

![screentogif_dragndrop](https://github.com/Keksuccino/FancyMenu/assets/35544624/ba4ad4a5-484e-46f1-8efd-90ba764462d8)

## Frame Delay

To configure the delay between frames, select the frame(s) you want to edit, switch to the **Edit** tab and in the **Delay (Duration)** section, click on **Override**.

![screentogif_delay](https://github.com/Keksuccino/FancyMenu/assets/35544624/a5d93139-3192-4090-b243-e5c0fe299963)

## Looping

The looping behavior can be configured in the **Save As** menu. Take a look at the next step for how to open this menu.

## Exporting the APNG

Now you're ready to switch to the **File** tab again to click on **Save As**.

In the save menu, make sure to:
- Set the file type to **APNG** (first setting, you maybe need to scroll to the top of the menu first)
- Disable **Detect Unchanged Pixels**

> You can also configure the **looping behavior** in the that menu! Disabling **Looped Apng** will make the APNG not loop at all, and when enabling it you can choose between a specific number of loops or infinite looping.
{.is-info}

![screentogif_save](https://github.com/Keksuccino/FancyMenu/assets/35544624/954353da-45ed-4df8-9f06-c78a0a469fc8)

## Using the APNG in FancyMenu

Now you can copy your APNG file to `/config/fancymenu/assets/`. Then you will be able to use it for nearly everything that accepts images.

> It is **really important** that the APNG file name ends with `.apng`!
> FancyMenu will not be able to identify the image as APNG if it's not ending with `.apng`.
{.is-warning}

![screentogif_use_apng](https://github.com/Keksuccino/FancyMenu/assets/35544624/2322da62-4013-451e-9a8b-3df0bf92df54)