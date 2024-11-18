---
title: Incompatibility List
description: A list of mods that are known to be incompatible with FancyMenu.
published: true
date: 2024-06-05T06:58:12.567Z
tags: 
editor: markdown
dateCreated: 2023-12-21T09:38:10.367Z
---

# List of Incompatible Mods

The following mods are known to be incompatible with FancyMenu in some way.

Some of the mods have workarounds to make them work with FancyMenu.
If that's the case, it will be written after the mod name in the list below.

**In case you found an incompatible mod that isn't part of this list already, please tell me via Discord!
Thank you very much!**


## Forge Mods

- OptiFine (works for the most part, but you should use [these alternatives](./optifine-alternatives) instead)
- [Custom Main Menu](https://www.curseforge.com/minecraft/mc-mods/custom-main-menu)
- [Pack Menu](https://www.curseforge.com/minecraft/mc-mods/packmenu)
- [Main Menu Scale Mod](https://www.curseforge.com/minecraft/mc-mods/main-menu-scale)
- [Terraria Craft](https://www.curseforge.com/minecraft/mc-mods/terraria-craft)
- [VanillaFix](https://www.curseforge.com/minecraft/mc-mods/vanillafix) (Useable, but some users have noticed problems with the VanillaFix crash screen. Sadly I wasn't able to reproduce this.)
- [Fossils and Archeology Revival](https://www.curseforge.com/minecraft/mc-mods/fossils) (Works ingame, but the custom main menu by this mod isn't supported. It can be disabled in its config.)
- [RandomPatches](https://www.curseforge.com/minecraft/mc-mods/randompatches-forge) (Works if `patchMinecraftClass` is set to `false` in its mod config)
- [Smooth Scrolling Everywhere](https://www.curseforge.com/minecraft/mc-mods/smooth-scrolling-everywhere)
- [The Dalek Mod](https://www.curseforge.com/minecraft/mc-mods/the-dalek-mod) (Works if the custom main menu of this mod is disabled in its config)
- [Custom Loading Screen](https://www.curseforge.com/minecraft/mc-mods/better-loading-screen)
- [Replay Mod](https://www.replaymod.com/download/) (Works when setting `mainMenuButton` from `DEFAULT` to `BIG` in `.minecraft/config/replaymod.json`)
- [Crash To Main Menu](https://www.curseforge.com/minecraft/mc-mods/crash-to-main-menu)
- [Ice and Fire](https://www.curseforge.com/minecraft/mc-mods/ice-and-fire-dragons) (Works if the custom main menu is disabled in its mod config)
- [Essential Mod](https://www.curseforge.com/minecraft/mc-mods/essential-mod) (COMPLETELY BREAKS customization for some newer builds of FancyMenu. For older builds, buttons and other elements added by this mod aren't customizable)
- [Sound Filters](https://www.curseforge.com/minecraft/mc-mods/sound-filters) (The audio extension will not work with this mod installed)
- [Minecraft Comes Alive](https://www.curseforge.com/minecraft/mc-mods/minecraft-comes-alive-mca) (works just fine, but the menus of the mod aren't customizable)
- [Skin Layers 3D](https://www.curseforge.com/minecraft/mc-mods/skin-layers-3d) (Works fine in 1.16+, but breaks 1.12)
- [Not Enough Animations](https://www.curseforge.com/minecraft/mc-mods/not-enough-animations) (Works fine in 1.16+, but breaks 1.12)
- [Supplementaries](https://www.curseforge.com/minecraft/mc-mods/supplementaries) (Randomly crashes the game when customizing its config screen. If that happens, manually delete the layout from `.minecraft/config/fancymenu/customization`)
- [MineTogether](https://www.curseforge.com/minecraft/mc-mods/creeperhost-minetogether) (Seems to break layouts when GUI scale is bigger than 2)
- [Jurassicraft](https://www.curseforge.com/minecraft/mc-mods/jurassicraft) (Game will crash on start when enabling customizations for Jurassicraft GUIs. To fix this, manually delete all Jurassicraft GUIs from `config/fancymenu/customizablemenus.txt`.)
- [Stylish Effects](https://www.curseforge.com/minecraft/mc-mods/stylish-effects) (Main menu fails to load layouts when shown for the first time)
- [Sound Physics Remastered](https://www.curseforge.com/minecraft/mc-mods/sound-physics-remastered) (The audio extension will not work with this mod installed)
- [EnhancedVisuals](https://www.curseforge.com/minecraft/mc-mods/enhancedvisuals) (Seems to break animations, makes backgrounds translucent and probably more)
- [MalisisCore](https://www.curseforge.com/minecraft/mc-mods/malisiscore) (Breaks main menu customization)
- [QuestCraft](https://github.com/QuestCraftPlusPlus/QuestCraft) (Game fails to load)
- [BetterFPS](https://www.curseforge.com/minecraft/mc-mods/betterfps) (Buttons and menus of this mod aren't customizable)
- [Controllable](https://www.curseforge.com/minecraft/mc-mods/controllable) (Custom buttons added to menus with FancyMenu aren't clickable via Controllable's "Virtual Mouse" feature)
- [Debugify](https://www.curseforge.com/minecraft/mc-mods/debugify) (Only incompatible in 1.18.2. Can be fixed by using [Modern Debugify](https://www.curseforge.com/minecraft/mc-mods/modern-debugify) instead.)
- [Chat Colors](https://www.curseforge.com/minecraft/mc-mods/chat-colours) (Crash on startup)
- [Remove Reloading Screen](https://www.curseforge.com/minecraft/mc-mods/rrls) (Incompatible on MC versions before 1.20.4. Works fine in MC 1.20.4+!)
- [Modern Online Picture Frames](https://www.curseforge.com/minecraft/mc-mods/online-picture-frame) (Crash; Can't fix on my end, see [this](https://github.com/Keksuccino/FancyMenu/issues/776))
- [Optiscale](https://www.curseforge.com/minecraft/mc-mods/optiscale) (Breaks FancyMenu's UI. UI buttons aren't clickable.)

## Fabric Mods

- OptiFine (works for the most part, but you should use [these alternatives](https://fm.keksuccino.dev/en/wiki/general/verified/optifine-alternatives) instead)
- [Mod Menu](https://www.curseforge.com/minecraft/mc-mods/modmenu) (**WORKS FINE** in most cases, but if you experience a duplicated or uncustomizable Mods button, change your Mod Menu button settings to "Adjacent": Main Menu > Mods > Mod Menu > Mods Button: Adjacent)
- [Bedrockify](https://www.curseforge.com/minecraft/mc-mods/bedrockify) (Compatible when you disable all menu modifications of the mod, at least for the menus you want to customize)
- [Slight Gui Modifications](https://www.curseforge.com/minecraft/mc-mods/slight-gui-modifications)
- [ThonkUtil](https://www.curseforge.com/minecraft/mc-mods/thonkutil) (works, but currently adds an unremovable text to the main menu)
- [Essential Mod](https://www.curseforge.com/minecraft/mc-mods/essential-mod) (COMPLETELY BREAKS customization for some newer builds of FancyMenu. For older builds, buttons and other elements added by this mod aren't customizable)
- [Minecraft Comes Alive](https://www.curseforge.com/minecraft/mc-mods/minecraft-comes-alive-mca) (works just fine, but the menus of the mod aren't customizable)
- [Skin Layers 3D](https://www.curseforge.com/minecraft/mc-mods/skin-layers-3d) (Works fine in 1.16+, but breaks 1.12)
- [Not Enough Animations](https://www.curseforge.com/minecraft/mc-mods/not-enough-animations) (Works fine in 1.16+, but breaks 1.12)
- [MineTogether](https://www.curseforge.com/minecraft/mc-mods/creeperhost-minetogether) (Seems to break layouts when GUI scale is bigger than 2)
- [Stylish Effects](https://www.curseforge.com/minecraft/mc-mods/stylish-effects) (Main menu fails to load layouts when shown for the first time)
- [Colormatic](https://www.curseforge.com/minecraft/mc-mods/colormatic) (Huge lag when starting MC and breaks FM's audio stuff)
- [Sound Physics Remastered](https://www.curseforge.com/minecraft/mc-mods/sound-physics-remastered) (The audio extension will not work with this mod installed)
- [Replay Mod](https://www.replaymod.com/download/) (Works when setting `mainMenuButton` from `DEFAULT` to `BIG` in `.minecraft/config/replaymod.json`)
- [EnhancedVisuals](https://www.curseforge.com/minecraft/mc-mods/enhancedvisuals) (Seems to break animations, makes backgrounds translucent and probably more)
- [QuestCraft](https://github.com/QuestCraftPlusPlus/QuestCraft) (Game fails to load)
- [Remove Reloading Screen](https://www.curseforge.com/minecraft/mc-mods/rrls) (Incompatible on MC versions before 1.20.4. Works fine in MC 1.20.4+!)
- [DungeonZ](https://www.curseforge.com/minecraft/mc-mods/dungeonz) (Crash)
- [Modern Online Picture Frames](https://www.curseforge.com/minecraft/mc-mods/online-picture-frame) (Crash; Can't fix on my end, see [this](https://github.com/Keksuccino/FancyMenu/issues/776))

----------

Tags: #conflict #crash #bug #glitch #issue #conflicting #incompatible #mod #not-working #problem #fix #help