---
title: Advanced Positioning & Sizing
description: How to use Advanced Positioning and Sizing of elements.
published: true
date: 2023-12-24T08:33:23.512Z
tags: 
editor: markdown
dateCreated: 2023-12-24T08:32:46.076Z
---

# Advanced Positioning & Sizing

Advanced positoning/sizing allows you to have **full control over the position and size of your elements**. This is very powerful but also **a lot more time-consuming** than using FancyMenu's automated sizing and positioning.

# Toggling Advanced Positioning/Sizing Mode

To **enable** andvanced positioning/sizing for an element, **right-click** it and click on **Advanced Positioning** or **Advanced Sizing**.
The element will automatically switch to the advanced mode when you set an advanced position or size value.

To **disable** it and switch back to normal positioning/sizing, **clear all positioning/sizing values**.

> While an element is in Advanced Sizing/Positioning mode, resizing and/or moving the element could be disabled or restricted.
{.is-warning}

# Calculating Positions/Sizes

The reason why advanced positioning/sizing is so powerful is that you can use **placeholders** in the position/size values.

This allows you to use the **Calculator** placeholder (located in the **Advanced** placeholder category) in combination with placeholders of the **GUI** category, like **Screen Width**, **GUI Scale**, **Element Width** and more.

> You can add placeholders by clicking on the **Placeholders** button at the top-right side of the text editor. If you don't see this button, the content you want to edit does **not support** placeholders.
{.is-info}

To calculate something with the **Calculator** placeholder, replace the example expression with your own. You can use nested placeholders in the expression, so you can make use of the screen size, element size, etc. placeholders there.

For example, this placeholder will simply solve `1 + 1` and will show as `2` later:

`{"placeholder":"calc","values":{"expression":"1 + 1","decimal":"false"}}`

The `decimal` variable is set to `false`, which is important for most sizing/positioning calculations, so just set this always to `false` when working with advanced positioning/sizing.

The following calculator uses the **Screen Width** placeholder and divides it by `2`:

`{"placeholder":"calc","values":{"expression":"{"placeholder":"guiwidth"} / 2","decimal":"false"}}`
