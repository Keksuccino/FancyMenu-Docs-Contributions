---
title: Custom GUIs
description: How to add a new GUI screen to the game.
published: true
date: 2024-01-30T08:26:46.175Z
tags: 
editor: markdown
dateCreated: 2024-01-30T08:26:08.730Z
---

# Custom GUIs

FancyMenu allows you to customize existing GUI screens, but it also allows you to add completely new ones and fill it with elements.

# Adding a New Screen

To add a new screen, navigate to **Customization -> Custom GUIs -> Manage Custom GUIs**.

![custom_gui_1](https://github.com/Keksuccino/FancyMenu/assets/35544624/23e704ee-ccb5-434d-b75f-f4418399d9b7)

In the next menu, click on **New GUI**.

![custom_gui_2](https://github.com/Keksuccino/FancyMenu/assets/35544624/035454e8-b089-4b9a-9092-89a193c0eacd)

Here you need to give your new GUI a unique identifier and you can customize other parts of the basic screeen behavior.
When you're done, press **Done**.

![custom_gui_3](https://github.com/Keksuccino/FancyMenu/assets/35544624/1fbed3f9-9c81-4c73-85c7-d152146c55d8)

Now you have a new empty GUI. To open it, select the GUI in the **Manage Custom GUIs** menu and click on **Open GUI**.

![custom_gui_4](https://github.com/Keksuccino/FancyMenu/assets/35544624/b2e6a4b7-540d-4bf2-9dce-09bfff11ae7e)

This will open the still pretty empty GUI screen. To make it less empty, just create a new layout for it like you would do with any other screen.

![custom_gui_5](https://github.com/Keksuccino/FancyMenu/assets/35544624/e7e06a5f-46b3-48f1-9ad9-96a7565c97a9)

# Opening the GUI via Action

The last part is to give normal users access to your GUI. The easiest way to do that is to use the **Open Screen or Custom GUI** action with a button, slider or ticker.

![custom_gui_6](https://github.com/Keksuccino/FancyMenu/assets/35544624/b5cc6518-3fc4-4715-96d4-44b65ab7831d)

# Opening the GUI via Command

You can also open your custom GUI via an [in-game command](./commands#openguiscreen).
This even allows you to remotely open the GUI for other users!