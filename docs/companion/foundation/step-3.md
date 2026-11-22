---
icon: material/numeric-3-circle
---

!!! abstract "Summary"
    This page primarily covers the Skyrim Script Extender and why it's important to keep track of your Skyrim version. I will also introduce the optional Root Builder plugin and close with some tips for keeping your workspace tidy.

## Root Folder Files

!!! note
    If you are familiar with root folder files ^^and^^ you don't want to use Root Builder, feel free to skip ahead to the next section.

Before we get to the Skyrim Script Extender, we need to talk about **root folder files** because – spoiler alert! – the Script Extender contains some of those.

To recap: Mod Organizer 2 exists to manage the contents of the data folder, which contains the vanilla game files. The vast majority of mods also belongs into the data folder.

What about the **root folder**?

Mods that belong into the root folder instead of the data folder are ^^rare^^. They typically hook into the game's engine in some way, which is why they must be located in the same directory as the game's executables – that is, the root folder.

Standard procedure involves managing data folder mods with a mod manager and dropping root folder mods directly into the root folder. This usually works fine because there are far fewer root folder mods and they clash very rarely.

That being said, there is an alternative that I strongly prefer and recommend.

### Root Builder

**Root Builder** is a plugin for Mod Organizer 2.

Root Builder allows you to install and manage files belonging into the root folder through Mod Organizer 2. When you launch the game or any tool through Mod Organizer 2, all root folder files will be temporarily copied into the actual root folder by the plugin. When the game or tool is closed, those files will automatically be removed again. Pretty neat, right?

### When to use Root Builder

Root Builder is completely optional. The plugin is very elegant but it does add some complexity as well. You should use Root Builder if:

- You use the default Skyrim installation (not Stock Game Folder) and share it with other MO2 or Vortex setups ^^or^^ you want to retain access to the vanilla game.
- You use ENBSeries with different presets and/or switch between ENBSeries and Community Shaders.

I personally still use Root Builder despite having a Stock Game Folder setup (i.e., a copy of the vanilla game) because I want to manage **all** my mod files in MO2. This allows me to use MO2 for version control and I always know which mod the files belong to.

!!! tip
    If you're unsure about Root Builder, I encourage you to give it a try. The *Companion* contains instructions to prevent a lot a issues with Root Builder, so its convenience should not come at a price for you.

### Installing Root Builder

**Root Builder** is hosted on Nexus Mods.

- Download the latest version of [Root Builder](https://www.nexusmods.com/skyrimspecialedition/mods/31720?tab=files) (click **Mod Manager Download**).
- In Mod Organizer 2, switch to the **Downloads** tab in the right pane.
- Right-click the downloaded mod and select Open File.
- Extract the **rootbuilder** folder to `\Mod Organizer 2\plugins\`.
- Restart Mod Organizer 2.

![Root Builder Installation](/companion/foundation/assets/root-builder-installation.png)

Root Builder can be configured through Mod Organizer 2 interface. The default configuration is perfectly adequate, however. I recommend leaving it unchanged.

## Introducing SKSE

### SKSE and Skyrim Updates

### Version Check

## Skyrim Version Control

### Stock Game Folder

### Downgrading Skyrim