<div align="center">

![banner](./images/banner.png)

</div>

A guide on how to **download** and **install mods** in **The Witcher 3 (Wild Hunt)** on PC. 

With that said, we've included instructions for using [Vortex](https://www.nexusmods.com/about/vortex/), the recommended mod manager by [Nexus Mods](https://www.nexusmods.com/), and how to install mods manually if preferred.

This guide is focused on **Windows**, but users using Linux and running The Witcher 3 through **Steam Proton** and/or **Wine** should be able to use many of the steps listed below without any issues!

## Table Of Contents
* [Requirements](#requirements)
* [Game Version Notes](#game-version-notes)
    * [Running Mods On Linux (Proton/Lutris)](#running-mods-on-linux-protonlutris)
* [Backup Your Game Files!](#backup-your-game-files)
* [Installing Vortex Mod Manager](#installing-vortex-mod-manager)
* [Where To Download Mods](#where-to-download-mods)
* [Installing Mods Through Vortex](#installing-mods-through-vortex)
* [Manual Mod Installation (Advanced)](#manual-mod-installation-advanced)
* [Script Merger - Fix Conflicting Mods](#script-merger---fix-conflicting-mods)
* [Mod Limit Fix (Optional)](#mod-limit-fix-optional)
* [Conclusion](#conclusion)
* [See Also](#see-also)

## Requirements
* The Witcher 3 installed via Steam, GOG, or Epic Games
* A free [Nexus Mods](https://www.nexusmods.com/witcher3) account (optional, but recommended)
* [7-Zip](https://www.7-zip.org/) or equivalent archive manager (for manually installing mods mostly)

## Game Version Notes
The Witcher 3 has several versions, including the **Next-Gen update (v4.0+)**. Mods made for older versions (v1.32) may not be compatible with Next-Gen without patches.

* **Steam and GOG** versions are the most mod-friendly.
* **Epic Games** version works, but Vortex support may be limited.
* You can toggle between classic and Next-Gen versions via Steam’s beta settings.

### Running Mods On Linux (Proton/Lutris)
The Witcher 3 is rated **Gold** on [ProtonDB](https://www.protondb.com/app/292030). Mods work fine in most cases, but Script Merger may require **Protontricks** or **Wine Mono**.

## Backup Your Game Files!
We strongly recommend **backing up your game folder and saves** before installing mods. This gives you a fallback in the case a mod causes game crashes or corrupts your installation altogether.

Here are some common paths to the game files.

- **Steam**:`C:\Program Files (x86)\Steam\steamapps\common\The Witcher 3`
- **Epic Games**: `C:\Program Files\Epic Games\The Witcher 3`

The most common save files location is:

```
C:\Users\<user>\Documents\The Witcher 3\gamesaves
```

**WARNING** - Keep note of the folder locations mentioned above as you will need them later on in the guide!

## Installing Vortex Mod Manager
[Vortex](https://www.nexusmods.com/about/vortex/) (mod manager) is considered the easier and safest way to manage mods in The Witcher 3.

If you'd like to use Vortex, please perform the following steps.

1. Download Vortex from [here](https://www.nexusmods.com/site/mods/1?tab=files).
2. Install and launch Vortex.
3. Under the **Games** tab, search for The Witcher 3 and click **Manage**.
4. If the game is not detected, manually set the path to `witcher3.exe`.

## Where To Download Mods
The best place for Witcher 3 mods is [Nexus Mods](https://www.nexusmods.com/witcher3).

Additional websites that provide mods in The Witcher 3 include the following.
* [ModDB](https://www.moddb.com/games/the-witcher-3-wild-hunt/mods)
* [GitHub](https://github.com/) (mostly for tools or mod patches)

**TIP** - We recommend checking the **requirements**, **description**, and **user posts** before installing a mod.

## Installing Mods Through Vortex
To download and install a mod through Vortex, perform the following steps.

1. Log into your Nexus Mods account.
2. Find a mod on Nexus Mods' website and click the **Mod Manager Download** button.
3. Now in Vortex:
    * Go to the **Mods** tab.
    * Enable the mod.
    * Click **Deploy Mods** if prompted.
4. Launch The Witcher 3 and test if the mod is active.

Some mods may still require merging scripts. Please see the section on **Script Merger** below.

## Manual Mod Installation (Advanced)
Some users prefer manually installing mods or a mod may not be compatible with Vortex.

In either case, you may perform the following steps to download and install mods manually. 

1. Find the mod from Nexus Mods' website.
2. Download the mod manually by clicking the download link.
3. Extract the mod files using a tool such as [7-Zip](https://www.7-zip.org/).
4. Copy the mod folder into your `Mods` folder inside of the game's folder.
    * `The Witcher 3\Mods\modExample`
    * Create the `Mods` folder if it doesn't exist!
5. For mod settings or configuration files, place them in the following folder.
    * `The Witcher 3\bin\config\r4game\user_config_matrix\pc`

You should now enable the mod menu.

Firstly, edit the following file using a text editor such as Notepad.

```
\Documents\The Witcher 3\user.settings
```

Next, and add the following under the `[General]` section.

```ini
DBGConsoleOn=true
```

Save and that should be it! Launch The Witcher 3 and test the mods you've installed.

## Script Merger - Fix Conflicting Mods
Many mods in The Witcher 3 modify the same scripts and will **conflict**.

To resolve these issues, it is recommended you use a tool called [Script Merger](https://www.nexusmods.com/witcher3/mods/484).

To download and use Script Merger, perform the following steps.

1. Download Script Merger from [here](https://www.nexusmods.com/witcher3/mods/484).
2. Launch it and select your Witcher 3 folder.
3. Click **Refresh** to detect installed mods.
4. Click **Merge Scripts** and resolve any conflicts.
    * Auto-merge works most of the time.
    * Manual merge may be required for complex mods.

**NOTE** - If conflicts aren't resolved, your game may crash at startup.

## Mod Limit Fix (Optional)
The Witcher 3 has a hard limit on how many mods can be loaded by default.

Fortunately, you can install a mod called **Mod Limit Fix** to remove this limitation entirely!

1. Download it from [here](https://www.nexusmods.com/witcher3/mods/3643).
2. Follow the instructions provided to patch `witcher3.exe`.

We highly recommend this individual mod if you plan to use many mods (50+).

## Conclusion
That’s it! You should now know how to install and manage Witcher 3 mods using Vortex and manual methods. Tools like **Script Merger** and **Mod Limit Fix** may be essential to some mod-heavy setups.

Modding The Witcher 3 can dramatically enhance graphics, gameplay mechanics, and immersion. Or just add fun random chaos to your next playthrough!

## See Also
* [Nexus Mods - The Witcher 3](https://www.nexusmods.com/witcher3)
* [Script Merger](https://www.nexusmods.com/witcher3/mods/484)
* [Mod Limit Fix](https://www.nexusmods.com/witcher3/mods/3643)
* [Vortex Mod Manager Guide](https://wiki.nexusmods.com/index.php/Vortex)
* [ProtonDB - Witcher 3](https://www.protondb.com/app/292030) (for Linux users)

This guide will be **updated over time**. Found an error or have feedback? Let us know!

Happy modding!