---
title: Panoramas
description: How to make and use custom background panoramas.
published: true
date: 2024-02-26T11:15:55.514Z
tags: 
editor: markdown
dateCreated: 2023-12-24T08:58:58.169Z
---

# Cubic Panoramas

FancyMenu supports loading custom 6-image panorama cubes as background for menus.

These panoramas are a special cubic panorama format used by Minecraft as background in the Title screen and is built out of 6 images (sides) that get rendered as cube (or skybox, to be more specific).

> **IMPORTANT**: If you're on Windows, don't forget to turn on [file extensions](https://cdn.discordapp.com/attachments/795308330746511390/801561308012347482/unknown.png), because otherwise you will not be able to see important parts of file names later!
{.is-warning}

# Making a Panorama

If you don't know how Minecraft handles their background panoramas and how to create these, you should check out [this video](https://www.youtube.com/watch?v=F7jMd3zsjZQ&t).
It will give you a very good understanding of how Minecraft's panoramas work and how to make one!

After watching the video, you will notice that creating these panoramas can be a bit time-consuming.
To save you some time, maybe think about using a mod that creates them for you.
You can find some of them by searching for `minecraft panorama mod`, but one of them is [Panoramica](https://www.curseforge.com/minecraft/mc-mods/panoramica) (made by me).

# Preparing the Panorama

After you got your 6 panorama images, you'll need to move them to the right place!

FancyMenu's panorama directory is located at `.minecraft/config/fancymenu/panoramas`.
This is the directory for all panoramas that you want to use in the mod.

## The Panorama Folder

Every panorama has its own folder.
You will need to create a new folder in `.minecraft/config/fancymenu/panoramas` if you want to add a new panorama.
In my example, I will name the folder `mypanorama`.

![1](https://user-images.githubusercontent.com/35544624/100791916-2802d380-341a-11eb-8e32-f9913e93a38c.png)

## Folder Content

After creating the folder, you will need to fill it.

### Properties File
Every panorama needs a properties file to work.
This file always needs to be named `properties.txt` and needs some important things written to it.

The content of a panorama properties file should always look like this:
```
type = panorama

panorama-meta {
  name = name_of_your_panorama
  speed = 1.0
  fov = 85.0
  angle = 25.0
  start_rotation = 0
}
```
Only the variables inside the `panorama-meta` section can be changed!

#### name
This has to be the **unique** name of your panorama.
It's not possible to load two panoramas with the same name!
You will use this name later to identify your panorama.

#### speed
The speed at which your panorama rotates.
This value is a speed multiplicator. For example, `1.0` is default speed, `2.0` doubles the speed and `0.5` will half it.
Negative values are not supported, use decimal values to slow the speed.

#### fov
The field of view.
The default FOV is `85.0`.
Using too big or small values here will break the panorama. Just play around with it to find the FOV you want.

#### angle
The vertical angle at which the panorama is viewed.
The default angle is `25.0`.

#### start_rotation
The rotation angle (horizontal) at which the panorama should start. Value between 0 and 360.

<br>

### Panorama Image Folder

The second mandatory thing your panorama folder needs is the actual image folder containing your panorama images.

This folder's name needs to be `panorama`.

Put all your panorama images in it, but don't forget to name them correctly like shown in the [video](https://www.youtube.com/watch?v=F7jMd3zsjZQ&t) above!

![3](https://user-images.githubusercontent.com/35544624/100791922-29340080-341a-11eb-8174-874a180d0485.png)

> Only PNGs are supported as panorama images!
{.is-warning}

### Panorama Overlay

The last step is **optional** and can be skipped if you don't want an overlay over your panorama.

If you want to add a vignette or other types of overlays to your panorama, you can add one named 'overlay.png'.
Keep in mind that only PNG is supported for the overlay and that the file name always needs to be 'overlay.png'!

### Checking Everything Again

You should now have a folder located at `.minecraft/config/fancymenu/panoramas`, containing a `properties.txt` file, another folder named `panorama` and maybe an overlay named `overlay.png`.

![2](https://user-images.githubusercontent.com/35544624/100791920-29340080-341a-11eb-8e26-98a7fd2ad7eb.png)

# Using the Panorama

After (re)starting the game or reloading FancyMenu via **Customization -> Reload FancyMenu**, you should now be able to set your panorama as menu background. To do this, right-click the layout editor background and click on **Menu Background**.