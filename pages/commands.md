---
title: Commands
description: FancyMenu's commands and how to use them.
published: true
date: 2024-04-13T02:04:41.590Z
tags: 
editor: markdown
dateCreated: 2023-12-24T08:44:25.178Z
---

# Commands

FancyMenu adds some commands to the game that can be very useful when combining them with other mods like FTB Quests.

> FancyMenu needs to be on the **SERVER** (and client) to use commands in Multiplayer!
{.is-warning}

## /openguiscreen

The `/openguiscreen` command lets you open a GUI (Vanilla/mod and custom GUIs).
It can even remotely open GUIs for other players when FancyMenu is installed on both server and clients.

For a more in-detail description of this command, take a look at the [Open GUIs by Command](/opengui-command) page.

**Usage:** `/openguiscreen <screen_identifier> <target_player>`

## /closeguiscreen

The `/closeguiscreen` command lets you close the current GUI.

Huh? This is totally useless you say?
Well yes, but actually no.

This command is useful for when using mods that trigger commands on specific actions.
So yes, this command is absolutely useless when using it without other mods, but can be really helpful if you have the right mods installed!

**Usage:** `/closeguiscreen <target_player>`

## /fmvariable

The `/fmvariable` command allows you to set and get FancyMenu variables.

To execute this command as another player on servers, you can use the `/execute as` Vanilla command.
So lets say you want to execute the `/fmvariable` command as the player `ExamplePlayer`. In that case you would type:
`/execute as ExamplePlayer run fmvariable...`.

**Usage:** `/fmvariable <get_or_set> <variable_name> [<set_to_value>] [<send_chat_feedback>]`

### Get
To **get a variable value**, use the `get` sub-command like this:
`/fmvariable get some_variable`

Then the value of this variable will be printed to your chat.

### Set
To **set a varaible**, use the `set` sub-command like this:
`/fmvariable set some_variable new_value true`

The last argument here is to set if you want to receive chat feedback, which means if you want this command to print messages to your chat.
