---
icon: material/numeric-2-circle
---

!!! abstract "Summary"
    This page introduces Mod Organizer 2 and covers the installation process as well as some basic adjustments to the interface. We will also briefly discuss profiles and create a new profile for your setup.

## Why Mod Organizer 2?

!!! tip
    If you are already familiar with Mod Organizer 2 and its virtual file system, feel free to [skip ahead to the next section](/companion/foundation/step-2/#installing-mo2).

Your mod manager is your workspace where you install, view, and modify your mods. It is the heart and soul of your setup and – if you enjoy tinkering – you will probably spend more time here than in-game. That's why it's important to choose the right tool.

There are two viable mod managers for Skyrim SE: [Vortex](https://www.nexusmods.com/vortex) and [Mod Organizer 2](https://www.nexusmods.com/skyrimspecialedition/mods/6194) (MO2).

**Vortex** is the official mod manager of Nexus Mods. Vortex takes a jack-of-all-trades approach and works with most of the moddable games supported by the website. By contrast, **Mod Organizer 2** was specifically designed for modding Bethesda games. While Vortex is perfectly fine for simple modded setups with minimal custom edits, ==MO2's at-a-glance interface and its approach to asset management make it the superior tool for building complex setups== for Skyrim and other Bethesda games.

!!! failure "Warning"
    All instructions in the *Companion* were written with Mod Organizer 2 in mind.

### MO2's Virtual File System

Arguably the best feature of Mod Organizer 2 is the **Virtual File System**, for VFS for short. Here is how it works:

Instead of extracting mod files into the data folder directly, Mod Organizer 2 stores them in separate, self-contained mod folders. No files ever actually conflict with or overwrite each other. From these files, MO2 builds a virtual **data folder** at runtime.

Your folder structure will look like this:

```
\Mod Organizer 2\mods\Mod 1\<files from mod 1>
\Mod Organizer 2\mods\Mod 2\<files from mod 2>
\Mod Organizer 2\mods\Mod 3\<files from mod 3>
```

Conflicts between mods are simulated in MO2 and resolved based on their order: If two mods contain the same files, the one placed lower in the mod order will overwrite in the virtual data folder. But because the files never *actually* conflict, you can always change which files are overwritten by changing the order of the two mods via drag-and-drop. You can also review and compare the files without having to reinstall and overwrite, and you will always know which mod any given file belongs to. In this way, Mod Organizer 2 vastly simplifies file management.[^1]

[^1]: More recent versions of Vortex also feature self-contained mod folders. However, there is no VFS, so files are still deployed (via hardlinks) to the data folder.

And that is why Mod Organizer 2 is going to be your best friend. Cherish it!

## Installing MO2

### Prerequisites

Mod Organizer 2 has two requirements. Chances are that already have them installed, but I recommend (re)installing them to be sure:

- Download [.NET Framework 4.8](https://dotnet.microsoft.com/en-us/download/dotnet-framework/thank-you/net48-web-installer) and follow the instructions in the installer.
- Download the [Microsoft Visual C++ Redistributable](https://aka.ms/vs/16/release/vc_redist.x64.exe) and follow the instructions in the installer.

To finalise the installation you may be required to restart your PC.

### Downloading MO2

Mod Organizer 2 is hosted on the Nexus and on Github. Dev builds for testing are available on [Discord](https://discord.com/invite/ewUVAqyrQX).

- Open the [Mod Organizer 2](https://www.nexusmods.com/skyrimspecialedition/mods/6194) Nexus page.
- Switch to the **Files** tab.
- Click the **Manual Download** button for Mod Organizer 2 under **Main Files**.

If you do not have Nexus Premium, you will need to click **Download** again on the next page after a brief countdown.

![Download MO2](/companion/foundation/assets/download-mo2.png)

### Installer Configuration

- Save the downloaded executable to a convenient location and run it.
- If there is a Windows warning, click **More Info** and **Run anyway**.[^2]
- In the MO2 installer, accept the license agreement and proceed to the next page.

[^2]: All files uploaded to Nexus Mods are scanned for malicious code via [VirusTotal](https://www.virustotal.com/gui/home/upload). You can view the report by clicking the checkmark in front of the file name. Files exceeding a certain size are reviewed manually. 

You will be asked where to install Mod Organizer 2. Once again, **selecting an SSD is highly recommended** as it will improve load times and in-game performance. However, you should be aware that all your mods will be contained within the MO2 folder, potentially adding up to 100GB and beyond, depending on the size of your setup.

For now, make sure you have ^^at least 50GB of free space^^ on whichever hard drive you choose. That will be sufficient to get started.[^3]

[^3]: To give you some perspective: My personal setup with several thousand mods plus downloads takes up around ~500GB.

!!! failure "Warning"
    Do not install MO2 into a UAC-protected folder such as `C:\Program Files\`.

![MO2 Installation Directory](/companion/foundation/assets/mo2-installation-directory.png)

### Instance Setup

After the initial installation process, the **Instance Manager** will open where we will create a new portable instance. MO2 instances are self-contained and allow you to create as many copies of Mod Organizer 2 as you need for various games or different setups.

- Click **Next** and **Create a portable instance** to proceed.
- Select **Skyrim Special Edition**.
- Select the version of the game you own and want to mod (ideally **Steam**).
- Configure the profile settings as follows:
    - Enable *Use profile-specific game INI files*.
    - Enable *Use profile-specific save games*.
- Disable **Automatic archive invalidation** (unnecessary for Skyrim SE).
- Leave the location for data files unchanged.
- Check the summary and click **Finish**.

![MO2 Instance Manager](/companion/foundation/assets/mo2-instance-manager.png)

### First Launch

Mod Organizer 2 should launch automatically.

- You will be prompted to view the tutorial – this is up to you.
    - *If you continue following the Companion you can safely skip the built-in tutorial.*
- If asked whether MO2 should handle NXM links, click **Yes**.
    - *This enables automatic downloads from Nexus Mods through MO2.*
- If asked about the **Category Setup**, select **Do Nothing**.
    - *You can import Nexus Mods categories later or create a custom set.*

Mod Organizer 2 will now open properly.

!!! tip
    Right-click the MO2 icon on your taskbar and pin it for quick access.

## MO2 Settings

Open the **Settings** by clicking the first icon on the right in the toolbar.

![MO2 Open Settings](/companion/foundation/assets/mo2-open-settings.png)

### Settings: General

Under **Download List**, I highly recommend checking **Show meta information** and **Compact list**. This will affect the **Downloads** tab in the right pane of MO2 where all downloaded files will appear. As the list grows, a more compact view with information about the file version and type will become useful.

![MO2 Downloads Comparison](/companion/foundation/assets/mo2-downloads-comparison.png)

I personally do not use the **Hide downloads after installation** option. The list of downloads in my MO2 setup is thousands of files long, and, yes, hiding files after installing them would keep the downloads tab clean. All hidden mods can quickly be made visible again by ticking the **Hidden files** box at the bottom of the **Downloads** tab, and individual files can be hidden and unhidden at will. Nonetheless, I prefer the simplicity of leaving everything visible and using the search bar to find what I am looking for. Once you start installing mods, you should make your own choice.

### Settings: Themes

While I personally prefer light mode in the majority of my apps and programs, I realise that my opinion is rather unpopular. Under **Style**, you can try out various other themes. If you are looking for a simple dark theme, I recommend the **1809 Dark Mode** option for now. It is similar to the default light theme and will make following along with my screenshots easier.

!!! failure "Warning"
    Always restart Mod Organizer 2 after changing the theme.

The **Colors** section below affects the colors in which mods and separators will light up when highlighting them. I strongly suggest not tampering with them until you have a proper understanding of mod order and asset conflicts.

### Settings: Mod List

Even before you install any mods, the left pane in MO2 is cluttered with the official master files and the various creations (if you own them). There are several ways in which we can deal with creations, including copying them over into MO2 to be managed as mods (because that is fundamentally what they are). However, I prefer to treat the creations like the official master files and leave them untouched in the data folder.

To remove a bit of clutter, I then hide external mods in MO2. Since we will not ever install files into the actual data folder, this will merely hide the official master files and creations in the MO2 UI. Alternatively, you can move those files under their own separator (we will discuss the creation of separators later on). 

![MO2 Hide External Mods](/companion/foundation/assets/mo2-hide-external-mods.png)

### Settings: Paths

Since we set up MO2 as a portable instance, all file paths to the various directories are currently within the MO2 installation itself: `/%BASE_DIR%/`, the base directory. We already discussed the potential size of the mods folder which should nevertheless be located on a fast drive, ideally an SSD.

However, ==the downloaded archives from which the mods are installed do ^^not^^ need to be on an SSD.== They are only required for the initial installation and merely serve as backups afterwards. I do still recommend keeping the archives. You may want to reinstall a mod later on (i.e., to choose different options if they come with an installer), or to revert any modifications.

If you want to keep the downloaded files but SSD storage space is a concern, you can change the **Downloads** directory to a different drive. Pick the hard drive with the most amount of space – any HDD will do.[^4]

[^4]: Keeping downloaded archives on a faster drive can speed up mod installation, including for Wabbajack lists. Nevertheless, SSD / NVME space is precious and you may prefer to use it for more mods or other games.

!!! note
    This is a recommendation, not a requirement. Manage your disk space as you see fit.

### Settings: Workarounds

Finally, you can enable archive parsing. This will allow MO2 to read the contents of BSAs (archives) and show file conflicts between loose and packed files. While archive parsing can slow down MO2, I never found the impact very noticeable.

- Check the box for **Enable archives parsing (experimental)**.

![MO2 Archive Parsing](/companion/foundation/assets/mo2-archive-parsing.png)

## MO2 Interface

Close the **Settings**.

Now we get our first proper look at MO2. If the interface seems daunting, do not feel discouraged! You will get used to it faster than you may think. Much of the UI simply makes a great deal of sense, which is why it will quickly become easy to navigate.

At this point, I am not going to discuss the purpose of the various parts of MO2's interface – without context, the details would be difficult to memorise. For now, please have a look at the five primary components of the UI which I will refer to by the names given below.

- (1) **The toolbar** allows you quick access to a number of sub menus.
- (2) **The profile drop-down** allows quick switching between MO2 profiles.
- (3) **The executables drop-down** is where you select and run the game or modding tools.
- (4) **The left pane** is the mod order. This is where all your mods will appear once installed.
- (5) **The right pane** contains various tabs like the Plugins tab for managing the load order.

![MO2 UI Overview](/companion/foundation/assets/mo2-ui-overview.png)

### Disable Log (optional)

First, I always disable the log at the bottom. I have never needed it and it takes up space.

![MO2 Disable Log](/companion/foundation/assets/mo2-disable-log.png)

### Customise Left Pane

The ==left pane== of Mod Organizer 2 represents the mod order. This is where all your mods will show up.

- Right-click the columns at the top to configure which columns are displayed.
- Enable all columns marked with a :check_mark: in the list below. I recommend matching my order as well (you can drag-and-drop columns to sort them).

![Adjust MO2 Columns](/companion/foundation/assets/adjust-mo2-columns.png)

- :check_mark: **Conflicts:** Displays little icons to show overwrites.
- :check_mark: **Flags:** Not necessary, but recommended. Shows if a mod has custom notes.[^5]
- :check_mark: **Content:** Very helpful because it shows you which types of assets are contained in a mod.
- :x: **Category:** Uses Nexus categories by default. Separators are much better for sorting.[^6]
- :x: **Nexus ID:** The ID of the respective mod (the numbers at the end of its URL).
- :x: **Source Game:** Somewhat useful when mixing Skyrim LE and Skyrim SE mods but that is very rare nowadays.
- :check_mark: **Version:** Helpful for tracking updates. Will turn red when an update is available.
- :x: **Installation:** Displays the date of installation. Not sure what you would need this for.
- :check_mark: **Priority:** Shows the mod's position in the mod order.
- :question_mark: **Notes:** See short notes at a glance. (AKA my favourite thing about MO2 – very optional but I'll introduce some potential usecases later.)

[^5]: There are also flags to remind you to endorse mods and to show the tracking status. The tracking feature never worked properly for me in MO2 and the only mods I have not endorsed are my own, so I typically disable both **Endorsement Integration** and **Tracking Integration** in the MO2 settings (Nexus tab). Disable these features or leave them active – it is up to you.

[^6]: You can make custom categories which can be quite useful. Instructions will follow later.

!!! Tip
    If your mod order ever gets completely messed up for no apparent reason, it's probably because you (accidentally) clicked a different column. When that happens, just click the **Priorities** column to restore the mod order.
