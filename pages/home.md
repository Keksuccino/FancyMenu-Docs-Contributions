---
title: Getting Started
description: The world of FancyMenu awaits you! This is the beginning of something beautiful!
published: true
date: 2024-05-07T06:47:28.969Z
tags: 
editor: markdown
dateCreated: 2023-12-21T04:18:27.484Z
---

# FancyMenu v3

Just a little reminder that this is the documentation for **FancyMenu v3**.

If you're looking for the v2 docs, please go to [the FMv2 documentation](https://fm.keksuccino.dev) instead.

# For Developers

If your are a developer and want to make an addon for FancyMenu or integrate FancyMenu in your mod, better take a look at the [developer documentation](https://github.com/Keksuccino/FancyMenu-Dev-Docs/wiki).

# Getting Started

The first time using FancyMenu can be a bit overwhelming, but don't worry, most of it is actually pretty self-explaining once you start working with it!

> Please **keep in mind** that this page is just to get into FancyMenu and help you with your **very first steps**.
Make sure to also check out the rest of the documentation for more in-detail information about FancyMenu's features!
{.is-info}

# The Menu Bar

One of the first things you will notice when starting the game is the **menu bar** at the top of every menu.

The **menu bar** is your entry point to basically all of FancyMenu's features like **creating layouts** to **customize menus**, changing the **window title and icon** and much more.

![menu_bar](https://github.com/Keksuccino/FancyMenu/assets/35544624/7100521c-8893-4eea-b0c1-1f02f4025ed7)

# Your First Layout

Since you probably want to customize Minecraft's menus, let me tell you something about **layouts**!

Layouts are like customization layers for menus and they allow you to add new elements and customize existing ones.

To make a new layout for a **specific menu**:
1. Open the menu you want to create a layout for (the Title Screen for example)
2. Open the **Customization** tab of the **menu bar**

Customizations are disabled for all menus by default and you need to activate them for every menu you want to customize, so let's click on the **"Current Screen Customization: Disabled"** entry first, which will switch the toggle to **Enabled**.

![toggle_customizations](https://github.com/Keksuccino/FancyMenu/assets/35544624/1654b7b1-cbab-4321-908c-7e3bf3239e75)

After doing that, click on **Layouts -> New -> For Current Screen**.

This will open the **layout editor** where you can add elements to the layout and customize Vanilla and mod elements (like buttons).

![new_layout_current](https://github.com/Keksuccino/FancyMenu/assets/35544624/065c3dd7-b3df-4501-b721-118ed819a93f)

## Editing the Layout

Most customization options can be accessed by **right-clicking the editor background**.
Doing that will open a context menu with lots of options, like customizing the **menu backround** or **adding elements** to the layout.

<br>
<img width="300" alt="Screenshot_1" src="https://gist.github.com/assets/35544624/853c8084-eaf3-42d3-875e-c386f0eebdee">

## Adding Elements to Layouts

To add a new element to your layout, **right-click** the background of the editor.

In the context menu that opens, click on **New Element** and choose one of the many types of elements.

![add_element](https://github.com/Keksuccino/FancyMenu/assets/35544624/865a66c5-76a6-404d-b746-d57802b1c12f)

## Customizing Elements

To customize an element, **right-click** it, which will open a context menu with everything you can customize for that element type.

It doesn't matter if the element is a custom element added by you or a Vanilla element that was already part of the menu.

![element_customization](https://github.com/Keksuccino/FancyMenu/assets/35544624/cfa3c357-d6be-4ed9-a6f0-a63f751e545a)

## Positioning Elements

Every element in FancyMenu is connected to an **anchor point**.

Anchor points are necessary for calculating an element's position and if used correctly, they prevent elements from overlapping each other, going out-of-screen or move to the wrong place when resizing the window.

They are the origin point from where the element's position is getting calculated.

By default, elements are connected to the **"Center of Screen"** anchor point, which is basically just the exact center of the screen, no matter the window size.
So lets say an element is 2 centimetres away from the center of the screen while being connected to the **"Center of Screen"** anchor. In that case, the element will **always** be 2 centimetres away from the screen's center, no matter the window size.

You can see the anchor point an element is connected to when dragging it. This will (by default) also show all other anchor points. You can hover an anchor point while dragging an element to change the element's anchor to the hovered anchor point.

Elements itself can also work as an anchor point for other elements! Just hover an element while dragging another and the dragged element's anchor point will get changed to the hovered element.

![anchor_points](https://github.com/Keksuccino/FancyMenu/assets/35544624/25bff930-0b52-4d76-b0e9-3e1cbcf3c20e)

## Saving Your Work

Don't forget to save your work!

This can be done by pressing **CTRL + S** or by clicking on **Layout -> Save**!

![save_your_work](https://github.com/Keksuccino/FancyMenu/assets/35544624/93436ec9-343e-4d10-85d9-de8982712c4a)

*Congratulations! You can now make Minecraft's menus look a lot more beautiful!*
