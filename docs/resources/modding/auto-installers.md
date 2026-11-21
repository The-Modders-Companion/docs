!!! abstract "Summary"
    This page explains what auto-installers are and why they became a staple in the Skyrim modding community. There are also tips for choosing a setup and some personal recommendations.

## What are Auto-Installers?

Auto-installers are tools that can replicate a modded setup without redistributing the mods themselves. Instead, they automate the process of downloading the mods from their original source, installing them, and configuring them. In the Bethesda modding community, auto-installers replace mod packs.

The creators of pre-made setups distributed with auto-installers are known as **curators**.

### Features

All auto-installers share the following features:

- Install a list of mods, using the exact versions specified by the curator.
- Arrange mod and load order as determined by the curator.
- Apply INI edits configured by the curator.
- Bundle additional files (like custom configs) into the installation file.
- Playable with few or no extra steps after installation.

For the differences between available auto-installers, check the [Comparison](/resources/modding/auto-installers#comparison) section below.

## A Brief History

The Bethesda modding community has a long tradition of restrictive sharing permissions on mods. As a result, mod packs in the traditional sense – the wholesale repackaging and redistribution of mods – was never an option.

Though open permissions have become more common in recent years, attitudes toward mod packs have not changed. This is not to say that mod packs for Skyrim do not exist, but they are regarded as unethical ('mod piracy') and therefore shunned.

### The Dark Ages

In the olden days, the only acceptable method to share a setup from one PC to another were [manual guides](/resources/modding/manual-guides). Every step taken in the creation of a setup had to be painstakingly documented by the author and precisely followed by the user – a lengthy and error-prone process. However, for those who could not or did not want to invest the time into building a custom setup, following a manual guide was the only alternative.

### The Revolution

Everything changed with the advent of auto-installers in 2019. Because literally repacking mods into mod packs was impossible, the idea was born to build a framework that could automate the process of downloading, installing, and configuring mods.

The first attempt, [Automaton](https://github.com/metherul/Automaton), was unsuccessful, probably due in part to its use of the controversial term 'mod pack'. Halgari, one of the contributors to Automaton, then split off to develop his own tool: **[Wabbajack](https://www.wabbajack.org/)**. Positioning itself as an auto-installer for 'mod lists', Wabbajack overcame the initial suspicion and hostility, and has since established itself as a staple in the modding community. The unparalleled convenience of auto-installers massively boosted the popularity of pre-made setups and gave rise to curators as an entirely new type of content creators.

A few years later, Nexus Mods added a similar auto-installer feature to Vortex called **[Collections](https://www.nexusmods.com/collections?collectionStatus=listed&sort=downloads)**. Collections proved a massive success, not only for Bethesda games. Today, there are over 5,000 listed Collections for Skyrim SE alone.

### A New Age

Building a custom setup – especially a large and complex one – takes a great deal of time and effort (see my [Modding Primer](/resources/modding/primer)). For a single user, this work can be hard to justify. But with auto-installers, individual setups now have large userbases and entire teams of curators spend months on individual projects.

As a result, pre-made setups are becoming more and more ambitious, growing not only in quality and complexity but spawning entire communities with their own Discord servers, websites or wikis, and coverage on YouTube and Twitch. And the potential of auto-installers is far from exhausted.

## Criticism & Responses

Despite their success, auto-installers remain a controversial feature in the Skyrim modding scene. The main points of criticism are:

1. Users no longer interact with mod pages. They rarely endorse mods or leave feedback. Mod authors feel disassociated from their own community and users play with their mods without even knowing who created the content. 
2. Curators benefit from the hard work of mod authors. Having packaged together mods created by other people, they earn money from donations that mod authors feel rightfully belong to them.

These arguments were especially common in the early years. However, it has since become clear that 'traditional' modding – users building custom setups and interacting with mod authors in the process – has not gone away. In fact, engagement has increased, in part because auto-installers drew a large new audience into Skyrim modding. Since 2019, the number of active Skyrim SE modders on Nexus Mods has doubled.

### Donations

The second point – curators earning money – remains contentious. Some curators do earn significant sums from their Wabbajack lists or Collections.

However, it's important to keep in mind that most Wabbajack lists and some Collections are far more than a simple list of mods. JaySerpa, mod author and curator of the  popular [Gate to Sovngarde](https://www.nexusmods.com/games/skyrimspecialedition/collections/qdurkx) Collection, has created a video documenting [The Work Behind A Massive Skyrim Modlist](https://www.youtube.com/watch?v=Lr8SPWZJX-Q&t=63s). Like many other curators, Jay invests significant time into creating custom mods and patches for his setup, and this work is deserving of rewards like any individual mod.

Moreover, mod authors have benefitted considerably from auto-installers. In addition to popularising mods that previously went under the radar, pre-made setups have vastly increased overall download numbers. Thanks to the Donation Point system, mod authors receive considerable kick-back when their work is included in a Wabbjack list or Collection, and this has helped ease increase the acceptance of auto-installers.

## Comparison

This section compares the two major auto-installers: **Wabbajack** and **Collections**.

!!! note
    I am excluding [Nolvus](https://www.nolvus.net/appendix/installer/introduction) from this comparison because Nolvus is essentially a variant of Wabbajack created for a specific set of setups.

### Mod Manager

The key difference between **Wabbajack** and **Collections** is the mod manager they are used with.

- Wabbajack is a standalone tool that installs a Mod Organizer 2 instance for each individual WJ list. Every instance is completely separate.
- Collections is integrated into the official Nexus Mods mod manager, Vortex. Collections are installed into the same Vortex instance and separated by profiles.

While all mod managers fundamentally do the same thing – place files into the correct folders – MO2 and Vortex differ in various ways. Simply put, MO2 is geared toward advanced use whereas Vortex is built to be beginner-friendly.

These differences are crucial to curators because they use the mod manager to build their setup. As a result, most complex setups are built in MO2 and shared via WJ, while simpler and/or smaller setups tend be published as Collections.

### Other Differences

- **Combining setups:** Wabbajack setups (i.e., MO2 instances) are fully self-contained and cannot be combined with each other. Meanwhile, Collections can be combined, which has led to the creation of 'Add-on Collections'.
- **Binary patching:** Both Wabbajack and Collections offer binary patching, applying the curator's modifications of mod files to the user's installation. However, Collections limit binary-patching to 20% of the mod's size, whereas Wabbajack has no limitations.
- **Additional files:** Wabbajack setups can be bundled with fully-configured modding tools and even a separate installation of the game. This is not possible for Collections.
- **Optional mods:** Curators can add a group of optional mods to Collections that can be installed on top of the main setup. While Wabbajack does not have this feature, the installed MO2 instances can have multiple profiles with different configurations.
- **Popularity:** Due to being featured prominently on Nexus Mods, Collections receive considerably more downloads. There are also far more Collections than Wabbajack lists.

## Finding Setups

You can find all Wabbajack lists on the [Gallery](https://www.wabbajack.org/gallery?game=skyrimspecialedition) and all Collections on [Nexus Mods](https://www.nexusmods.com/games/skyrimspecialedition/collections?collectionStatus=listed).

I recommend checking YouTube for showcases.

### Criteria

While looking for a pre-made setup to install, consider the following points:

- **Game Version:** Most pre-made setups require the Steam version of Skyrim SE. Some setups also provide GOG support. The Anniversary Edition DLC is now also frequently a requirement. In addition, the setup may run on an older version of Skyrim SE; if so, WJ lists likely contain their own copy of the game while Collections use [Skyrim Runtime Swapper](https://www.nexusmods.com/skyrimspecialedition/mods/189855) or ask you to downgrade manually.
- **Purpose/Theme:** Pre-made setups differ greatly in scope and content (I listed the main 'types' below). If you simply want to play, you're probably looking for a full setup. If you want to build your own setup on top, grab a baseline or visuals-only list (ideally for WJ as MO2 is better for tinkering).
    - *Baseline setups* contain only 'essential' mods as chosen by the curator. Some specifically target mod authors or curators while others are for general use.
    - *Visuals-only setups* do not change gameplay or add content, making them ideal for a vanilla playthrough with better graphics or as a starting point for a custom setup.
    - *Full setups* often focus on a particular theme, such as 'vanilla plus' (no radical changes), survival, or 'dark fantasy'. Some are centered around a particular mod like [Legacy of the Dragonborn](https://www.nexusmods.com/skyrimspecialedition/mods/11802) or [Requiem](https://www.nexusmods.com/skyrimspecialedition/mods/60888).
- **Activity/Support:** While setups without recent updates are not necessarily broken (my WJ lists haven't been updated since 2023 and are still fine), it is often advisable to look for setups that are actively maintained and supported. Check the setup's changelog and Discord server.

### My Recommendations

- **Collection:** [Gate to Sovngarde](https://www.nexusmods.com/games/skyrimspecialedition/collections/qdurkx) (GtS) by [JaySerpa](https://www.nexusmods.com/profile/jayserpa?gameId=1704) is an incredible showcase for what ambitious pre-made setups can be. Meticulously curated with numerous custom mods and insane attention to detail, GtS is a performant list with many of the best content additions and heavy emphasis on immersion and survival.
- **Wabbajack:** [Keizaal](https://keiza.al/) by [TateTaylor](https://www.nexusmods.com/profile/TateTaylorOH) is a true remaster for Skyrim. Emphasising consistency and integration, Keizaal aims to be a native experience that never feels 'modded' while nonetheless overhauling many core gameplay systems and adding fresh content (including not one but two enormously adorable corgis!).