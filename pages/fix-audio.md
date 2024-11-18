---
title: Fix Audio Files
description: How to fix audio files in case FancyMenu fails to play them.
published: true
date: 2024-04-17T01:23:05.750Z
tags: wav, ogg, audio
editor: markdown
dateCreated: 2024-04-17T01:23:05.750Z
---

# Fixing Audio Files

Minecraft is a little bit picky about what audio files it plays.
Sometimes it happens that audio files work fine in other audio players, but FancyMenu failes to play them.
If that's the case, you can try to fix the audio file to make it work in Minecraft.

# OGG Files

In most cases it's pretty easy to fix OGG files.

90% of your audio file problems get solved by simply re-converting the file.

1. Go to https://convertio.co/ogg-mp3/ and convert your OGG to MP3.
2. Go to https://convertio.co/mp3-ogg/ and convert the MP3 you got in the last step back to OGG.

The file should work fine now.
If it still doesn't work, make sure it's not a super big audio file and check if the audio file plays in other audio players.

# WAV Files

For WAV files it's mostly an unsupported sample rate and similar things that make the audio not work correctly in Minecraft.

Make sure that your audio:

- Has a sample rate of 48KHz
- Has a bit rate of 16bit
- Is a valid WAV file that works outside of MC

You can easily (re)convert your audio to the correct bit and sample rate by using this website:
https://audio.online-convert.com/convert-to-wav

**IMPORTANT:**
Even if you think your audio already has the correct format, bit rate and sample rate, please re-convert it anyway using the website mentioned above.

# Other Causes

Sometimes it's not the file that's broken, but other things that are not configured correctly, etc.

## Volume Too Low

Maybe your Minecraft volume is too low for you to hear the audio.
Make sure the MASTER channel and all other channels are loud enough.

## Mod Conflict

Maybe another mod is incompatible with the audio system my mods use.
In that case, please open an issue on GitHub, thank you very much.