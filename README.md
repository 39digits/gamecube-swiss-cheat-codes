# GameCube Cheat Codes for use with Swiss

## Introduction

This repository will contain the cheat files for a small selection of the GameCube discs I own.

Why cheat in the first place? The GameCube era felt like many companies were still trying to work out the best defaults for the 3D generation and many first party Nintendo titles have inverted X axis on camera controls. That would be fine if there were settings in-game to change this but most times there were none to be found. It is possible to load a "cheat" to invert the inverted controls - meaning pushing the C Stick right swings the camera right and vice versa in the same way we're used to doing in modern games.

I prefer to run retro games plugged into my HDMI TV. I am using a NTSC GameCube DOL-001 model with the [EON GCHD MK-II](https://www.eongaming.tech/). The DOL-001 model is very important as it includes both Digital AV Out as well as Analog AV Out. The later model DOL-101 only has Analog AV Out.

The EON GCHD plugs into both the Digital AV Out and Analog AV Out to provide beautifully clean HDMI output.

Another very important part of the setup is to use a NTSC GameCube rather than PAL. This is because only NTSC games allow you to boot in 480p Progressive Scan Mode by holding the B button upon booting a game. This ability is completely removed from PAL games and as such PAL games cannot be started in Progressive Scan Mode at all. Progressibe Scan Mode is required for the EON GCHD to give you a clean image - if you don't you may as well not use the expensive GCHD at all.

The ability to load cheats requires some extra hardware as detailed in the setup below.

## Booting ISOs

There are four key elements to running ISOs of your owned discs:

- ActionReplay for US
- SD Card Reader
- 2Gb SD card with the latest [Swiss DOL](https://github.com/emukidid/swiss-gc)
- Large capacity SD card with the ISO rips

ActionReplay is usually used as a cheat system but also allows us to boot homebrew software (e.g. Swiss) off of an SD card inserted into the Memory Card slots. This is all we need the ActionReplay disc to do - boot our homebrew OS.

I am using an SD card reader to hold rips of my owned games to avoid wear and tear on my NTSC discs and the GameCube's laser. There are numerous versions of SD card readers out there including WiiKey and SDGecko.

I have two SD cards - a large capacity card with all of the ISOs and another 2Gb card running Swiss. It's important to use a card smaller than 4Gb to boot Swiss as this is the maximum capacity card that the ActionReplay software can read.

To begin, put the ActionReplay for US disc into the NTSC GameCube and the SD Card Reader into Memory Slot B (keeping Memory Slot A for your actual memory card). Ensure the SD card with Swiss is in the reader and turn the GameCube on. ActionReplay will boot and show the contents of the SD card at which point you should select the Swiss DOL to boot the homebrew software.

Once Swiss loads, remove the lower capacity SD card from the reader and pop the card containing the ISOs into the reader. Press B (to get to the Menu) and press A on the first menu item. Tell Swiss to re-scan the SD card and a list of your ISOs will now appear.

## Booting into Progressive Scan Mode

Many NTSC games support 480p Progressive Scan Mode - to do so simply hold down the B button until prompted with a message after you boot the game. When the game loads it will ask if you wish to start in Progressive Scan Mode instead.

If the game does not support Progressive Scan Mode you can force it by selecting the ISO in Swiss and pressing X for the settings. Change the video mode to 480p and boot the game normally (no need to hold down B).

## Loading Cheats

Swiss supports WiiRD format cheats stored in text files placed into a folder named `cheats` in the root of the SD card.

It is also very important that the cheat file be named the same as the identifier for the game itself. You can find this by doing a `more` on the ISO in the commandline.

Super Mario Sunshine, for example, has the code GMSE01 for the NTSC version. I have a file named `GMSE01.txt` with many available cheats with the C Stick invert option right at the top (as that is honestly the only one I really care about using).

Navigate to the ISO of the game you want to enable a cheat against and press A to go to the game's detail screen in Swiss. Press Y to be shown a list of cheats if a corresponding file is found in the `cheats` directory. Press A to enable any you wish to use.

Load the game as per normal (remember to hold B for 480p mode) and the cheats will be enabled.

Now enjoy the X axis the way it is meant to be experienced :)
