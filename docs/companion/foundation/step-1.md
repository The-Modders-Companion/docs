---
icon: material/numeric-1-circle
---

!!! abstract "Summary"
    This page covers all necessary prerequisites, including a clean reinstall of Skyrim SE and (optionally) the Creation Kit.

## A New Journey

A new journey begins! Starting from a blank slate and taking the first steps has always been the most exciting part for me, and I hope this will be fun for you as well. We have a long way to go, so grab a cup of coffee or tea and put on some music. Here's [a lovely ambient mix of the Skyrim soundtrack](https://youtu.be/hFd1Kqkh2-k?si=bMJzbPm_9zgCqJ0H) that I quite enjoy myself. It'll put you in the right mood.

## Requirements

Before diving in, please make sure that you meet all requirements:

- You should have a **file archiver** like [7ZIP](https://www.7-zip.org/) installed. I also recommend using the text editor [Notepad++](https://notepad-plus-plus.org/downloads/) for modifying configuration files.
- I will assume that you are using a **recent version of Windows** (10/11). Modding on Linux is possible but I have no experience with it and can thus give no advice.
- **Some tech literacy** is inevitably required. You need to know how to create new files and folders, handle archived files, and install software.

Please follow along with the instructions carefully. ==The most important prerequisite – and the one most often ignored – is the ability to read.== Thirty seconds saved by skimming can easily turn into thirty minutes of tedious troubleshooting. Remember to take regular breaks!

### Nexus Account

We will source the vast majority of our mods and tools from [Nexus Mods](https://www.nexusmods.com/). Other sites exist but none with as many mods.

In order to download mods from Nexus Mods, you need an account.

- If you do not have a Nexus Mods account yet, go ahead and [create one now](https://users.nexusmods.com/register).

!!! note "Nexus Premium"
    Nexus Mods offers a Premium subscription which removes ads, increases download speeds, and automates the installation of Collections or Wabbajack lists.
    
    I recommend holding off on Premium until you have progressed enough in your modding journey to know that you will stick with it for a while. When building a larger mod setup, paying for a month or so of Premium can be well worth the asking price. This is also a great way of giving back to Nexus Mods for their service, especially for those of us with ad blockers installed.

### Skyrim Version

The regular **Steam** version of Skyrim is the best option for modding and all instructions in the *Companion* were written for this version. Whether you own the **Anniversary Edition DLC** or any individual Creations is irrelevant.

- :check_mark: [Steam](https://store.steampowered.com/app/489830/The_Elder_Scrolls_V_Skyrim_Special_Edition/) – for modding on PC
- :warning: [GOG](https://www.gog.com/en/game/the_elder_scrolls_v_skyrim_special_edition)
- :warning: [Steam](https://store.steampowered.com/app/489830/The_Elder_Scrolls_V_Skyrim_Special_Edition/) – for modding on the SteamDeck
- :warning: [Steam VR](https://store.steampowered.com/app/611670/The_Elder_Scrolls_V_Skyrim_VR/)
- :x: [Epic Games Store](https://store.epicgames.com/en-US/p/skyrim)
- :x: [XBOX Store / PC Game Pass](https://www.xbox.com/en-GB/games/store/the-elder-scrolls-v-skyrim-special-edition-pc/9P03JGQ4S1GC/0010)
- :x: Any console version

??? warning "Why I do not support the GOG version"
    I initially planned to add instructions for both the Steam and GOG versions but ultimtely decided against it. The main reason is the added complexity for my Clean Install instructions as well as later optional instructions for the Stock Game Folder method (which already adds a lot of conditional steps).

    There are other reasons: The GOG version is currently locked to an equivalent of SSE patch 1.6 with no way to up- or downgrade. Setting up the Creation Kit [seems to be pretty complicated](https://www.gog.com/forum/elder_scrolls_series/skyrim_creation_kit/page1). And not all SKSE plugins support the GOG version.

Modding the **PC VR** version or on the **SteamDeck** is not substantially different but will require some extra steps. These are not covered in the *Companion* because I am not familiar with them. You can find some links and resources for modding on the SteamDeck in the Skyrim Versions article linked below.

!!! tip "Skyrim Versions"
    Check my article on [Skyrim Versions](/resources/modding/skyrim-versions) for more information.

### File Name Extensions

Make sure that **file name extensions** are set to visible in Windows Explorer. This will enable you to tell apart files by their extensions.

- Open the **Windows Explorer**.
    - ==**Windows 10:**== In the **View** tab/ribbon, make sure the **File name extensions** box is ticked.
    - ==**Windows 11:**== Go to **View** 🠆 **Show** and make sure **File name extensions** is checked.

<center>Enable file name extensions on Windows 10:</center>
![File Name Extensions (Win10)](/companion/foundation/assets/file-name-extensions-win10.png)

<center>Enable file name extensions on Windows 11:</center>
![File Name Extensions (Win11)](/companion/foundation/assets/file-name-extensions-win11.png)

## Monitor Calibration (optional)

Correct monitor calibration can improve colour balance and brightness, ensuring that Skyrim (and any other game) looks as intended. 

!!! tip
    Let your monitor run for 30-60 minutes before calibrating it.

Many monitors can be adjusted directly via a button and an in-built menu. You should be able to find instructions by looking up the model on Google.

You can also adjust monitor settings through software:

- **Windows 10:** Control Panel 🠆 Colour Management 🠆 Advanced 🠆 Calibrate display
- **Windows 11:** Settings 🠆 System 🠆 Display 🠆 Colour management 🠆 Colour calibration
- **NVIDIA:** Control Panel 🠆 NVIDIA Control Panel 🠆 Adjust Desktop Color Settings
- **AMD:** *Unfortunately, I never owned an AMD GPU so I cannot give advice here.* :frowning:

To help you find the sweet spot for your monitor, check out these resources:

- [CLF ENB - monitor calibration help](https://i.imgur.com/k1v8p1M.png) (Imgur link – sorry, Brits!)
- [Photo Friday Monitor Calibration Tool](https://www.photofriday.com/info/calibrate)
- [Lagom: LCD monitor test images](http://www.lagom.nl/lcd-test/)

### Dynamic Range

It is recommended that you set monitor's **Dynamic Range** to *Full* if it is connected to your PC via DisplayPort or HDMI. Instructions for NVIDIA- and AMD-based systems can be found [here](https://pcmonitors.info/articles/correcting-hdmi-colour-on-nvidia-and-amd-gpus/).

## Uninstalling Skyrim

If you ever modded Skyrim before, chances are you have left-over files in various directories. We will thus begin with a full reinstall of the game to make sure we start with a clean slate.

If you currently have Skyrim installed, please begin by uninstalling the game.

- Find **Skyrim Special Edition** in your **Steam Library**.
- Right-click the game and select **Manage** 🠆 **Uninstall**.
- Click **Uninstall** again in the message box that follows to confirm.

![Uninstall Skyrim](/companion/foundation/assets/uninstall-skyrim.png)

### Creation Kit

If you have the Creation Kit for Skyrim SE installed through Steam, uninstall it in the same way.

### Mod Files

> Skip this step if you never modded Skyrim on this PC before.

Steam will uninstall all vanilla files but it will not touch mod files. Any leftover files added by mods must be deleted manually.

- Navigate to where the game was installed. This is most likely `C:\Program Files x86\Steam\steamapps\common\`.
- If there is still a **Skyrim Special Edition** folder in this location, delete it.

### INI Folder

> Skip this step if you never launched Skyrim on this PC before.

When clean-installing Skyrim, the **INI Folder** should be cleared out as well – not only to remove clutter but also to ensure that a fresh set of INI files can be acquired later on.

- Navigate to `C:\Users\<Your User Name>\Documents\My Games\Skyrim Special Edition\`.

!!! failure "Warning"
    If you have save files that you want to keep, make a backup of the **saves** folder now.
 
- Delete the entire **Skyrim Special Edition** folder.

The folder and its contents will be regenerated upon launching the game after the reinstallation.

And that is all! Skyrim SE is now completely removed from your system.

## Game Language

While Skyrim supports various languages natively, mods generally do not. In principle, it is still very possible to play modded Skyrim in a language other than English. Third-party translations are often available and creating translations is not overly complicated.

Nonetheless, modding the game in another language other than English adds a fair amount of additional work and complexity. You will likely have to update existing translations and translate the remaining mods yourself.

**I strongly encourage beginners to start with an English setup.** You can still translate your mods later on when you have a better understanding of their inner workings.

!!! failure "Warning"
    The *Companion* will assume that you are using an English-language installation of Skyrim.

### Set Language to English

> Skip to the next step if you never changed the game language before.

- Right-click **The Elder Scrolls V: Skyrim Special Edition** in your Steam games library.
- Select **Properties** and switch to the **Language** tab.
- Ensure that the language is set to **English**.

![Steam Skyrim English](/companion/foundation/assets/steam-skyrim-english.png)

## Installation Directory

Before reinstalling Skyrim, we need to select an adequate location. There are two aspects to keep in mind:

1. **Skyrim should be installed on your fastest drive** – ideally an SSD – which will reduce load times. Running Skyrim from an HDD negatively impacts performance, causing stuttering and frame drops.
2. Additionally, **Skyrim must ^^not^^ be located within UAC-protected folders** because this can prevent modding tools from properly accessing the game files.

### UAC-Protected Folders

Your Steam installation is probably located inside `C:\Program Files x86\Steam\`. By default, all Steam games are installed within this folder under `\Steam\steamapps\common\<Game>\`.

The problem is that `C:\Program Files\` and `C:\Program Files x86\` are so-called **UAC-protected folders** (UAC = user account control 🠆 [click here to read more](https://learn.microsoft.com/en-us/windows/security/application-security/application-control/user-account-control/?source=recommendations)). UAC-protected folders in Windows are special because they require admin privileges for read/write permissions. This can break functionality in modding tools.

### Stock Game Folder

There is one caveat ...

The location of your main installation of Skyrim doesn't matter ^^if^^ you use a separate copy of the game for modding. This can be done with the so-called **Stock Game Folder** method, a trick that Wabbajack curators came up with to allow the installation of multiple fully self-contained setups.

I will explain the advantages of a stock game folder in more detail later on. For now, suffice it to say that a stock game folder may be overkill if you only want to run a single setup of mods (though it is still very useful for version control). However, if you choose to use the method, you are free to put your main installation of Skyrim on a slower drive or inside UAC-protected folders.

## Steam Libraries

When installing a game through Steam, you can select any of your **Steam Libraries** as the installation folder. A Steam Library is simply a folder on one of your hard drives that has been configured in Steam as an installation directory for games. The default Steam Library is contained within the Steam installation folder itself: `\Steam\steamapps\`.

If you installed Steam under `C:\Program Files x86\` you will need to create a new Steam Library in a different location. Once set up, the new Steam Library can be selected as the installation directory upon installing a new game.

> Skip ahead to [Reinstalling Skyrim](/companion/foundation/step-1/#reinstalling-skyrim) if you already have a Steam Library in a suitable location.

### Option 1 – On the same drive

By default, you can only have **one** Steam Library per hard drive. If you want to create a second Steam Library on the same hard drive that you installed Steam on, please use [LostDragonist's Steam Library Setup Tool](https://github.com/LostDragonist/steam-library-setup-tool/wiki/Usage-Guide) and follow the instructions from the link.

### Option 2 – On a different drive

If you want to create a new Steam Library on a drive that is ^^not^^ `C:\`, follow these steps:

- Open the **Settings** in Steam and go to the **Storage** tab.
- Find the little ➕ icon near the top to add a new Steam Library.
- Select the desired hard drive.

![Add Steam Library](/companion/foundation/assets/add-steam-library.png)

## Reinstalling Skyrim

Now we can finally reinstall Skyrim.

- Find the game in the Steam Library tab and click the big blue **Install** button.
- As the installation location choose a Steam Library on your fastest hard drive and outside UAC-protected folders.
    - Example: `X:\SteamLibrary\steamapps\common\Skyrim Special Edition\`
- Proceed when the download is completed.

![Install Skyrim](/companion/foundation/assets/install-skyrim.png)

## First Launch

Last but not least we should make sure that our new installation of Skyrim launches properly. 

Running the game after reinstallation serves multiple purposes:

- To regenerate the `\Documents\My Games\Skyrim Special Edition\` folder. This includes the generation of a fresh set of INI files.
- To set up the registry keys, which is required for modding tools to recognise your installation.
- To detect issues with your vanilla game (i.e., file corruption during the installation).

!!! failure "Warning"
    Always launch Skyrim once after updating or reinstalling the game, or after verifying game files.

### Test Run

- Launch Skyrim through Steam.

A message box will pop up, informing you that Skyrim will now be configured based on your hardware. If the launcher is unable to detect your hardware, this is likely because you have a newer graphics card that is not recognised. You can ignore the warning.

- Click **OK** twice to confirm. We will configure the INI files later on.
- Click the **PLAY** option in the launcher and wait until you are in the Skyrim main menu.
- If you own the **Anniversary Edition DLC**, Skyrim will prompt you with a message box and proceed to download all creations. Wait for this process to finish.
- Quit the game from the main menu.

## Folder Structure Basics (optional)

Before you proceed with the next step, I highly recommend taking a moment to read [this article](/resources/modding/folder-structure) on folder structure and terminology. It's a quick read without additional instructions and will help you better understand the instructions in the next step.
