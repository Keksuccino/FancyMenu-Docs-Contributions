---
title: Open GUIs by Command
description: How to open Vanilla and Custom GUIs via command.
published: true
date: 2024-04-10T07:59:16.655Z
tags: 
editor: markdown
dateCreated: 2023-12-22T05:50:27.215Z
---

# Opening GUIs by Command

FancyMenu comes with a command that lets you open Vanilla and Custom GUIs via command.
You can even remotely open GUIs for **other players** when installing FancyMenu on both **server and clients**.

To open a GUI, just use the command `/openguiscreen <screen_identifier> <target_player>`.

Replace `<screen_identifier>` with the actual menu identifier of the GUI you want to open.
This can be the identifier of your Custom GUI (made with FancyMenu) or the normal menu identifier of a Vanilla/mod GUI.

To get the **menu identifier of Vanilla/mod GUIs**, open the menu you want to know the identifier of and enable FancyMenu's **debug overlay** via **Customization -> Debug Overlay**, then you can click on the identifier shown as first line to copy it to your clipboard.

![copy_identifier](https://github.com/Keksuccino/FancyMenu/assets/35544624/dd6c53d9-d2bd-4810-be03-3741e326bd5a)

Leave the `<target_player>` argument empty to open the GUI for your client or choose a player (or multiple players) to open the GUI for.
Keep in mind that the other player needs to have FancyMenu installed on their client.

# Closing GUIs by Command

In the rare case you need it, there's also a `/closeguiscreen <target_player>` command that closes the current screen.
