# Vanilla+ Templates
Welcome to the Vanilla+ Templates project, a series of map and mod files designed to streamline StarCraft2 campaign modding for the Custom Campaign Manager. This README file will walk you through how to get started with using the Vanilla+ Template for a campaign as well as the additional functionalities we've provided. Please be sure to read this guide carefully before contacting us with questions, if you aren't willing to read all this, you're not going to make it very far modding SC2.
Let's get started!

-Orcawarrior2 and JamesFire 

# Table of Contents
- [Vanilla+ Templates](#vanilla-templates)
- [Table of Contents](#table-of-contents)
- [Campaigns](#campaigns)
- [Download](#download)
- [What's Inside](#whats-inside)
  - [Map Files](#map-files)
  - [Mod Files](#mod-files)
    - [Base Mod (VanillaPlusCMP\_BASE.SC2Mod)](#base-mod-vanillapluscmp_basesc2mod)
    - [Extender Mod (VanillaPlusCMP\_EXT.SC2Mod)](#extender-mod-vanillapluscmp_extsc2mod)
- [What's Not Inside (Your Mod!)](#whats-not-inside-your-mod)
- [Vanilla+ Banks](#vanilla-banks)
- [Rules](#rules)


# Campaigns
Vanilla+ Templates support the five Blizzard SC2 campaigns, *Wings of Liberty*, *Heart of the Swarm*, *Legacy of the Void: Prologue*, *Legacy of the Void*, and *Nova: Covert Ops*. We will always abbreviate them as WOL, HOTS, LOTV:P, LOTV, and NCO respectively in this project. We will also use **CMP** when we need to refer to a generic campaign, if you see this just mentally replace it with the abbreviation for the campaign you are working with. Vanilla+ does not provide support for custom campaigns such as StarCraft Mass Recall.

# Download
Download the folder of your desired campaign, and the VanillaPlusLibrary file.

# What's Inside
So you just downloaded the template of your chosen campaign, what did you just get? 
## Map Files
The first thing you'll notice is a large set of map files for the entire campaign. All of these are completely vanilla, except for their dependencies and preload info. We will explain both of these edits further on.
## Mod Files
Every Vanilla+ Template comes with two mod files one that ends in _BASE and one that ends in _EXT. 
### Base Mod (VanillaPlusCMP_BASE.SC2Mod)
This mod connects your project to the vanilla dependencies made by Blizzard. It is crucial for providing the base level functionality of the campaign. We may update this mod to use more depenencies, add additional functionality for trigger work, or to fix bugs present in the vanilla game. It is absolutely crucial that you **do not edit the base mod file**. Doing so can adversely harm our ability to patch the templates and other mods that rely on this template.
### Extender Mod (VanillaPlusCMP_EXT.SC2Mod)
This mod file is empty, like very much empty. However, all of the map files use this as their one and only dependency, which means all of the map files use the extender's dependencies as their own with absolutely no changes in between. Note that we call this an **extender** mod not an **extension** mod, they may achieve a similar affect as extension mods on Battle.net but they are very different. Please be careful to use the correct term in discussions to avoid confusion.
### Trigger Library (VanillaPlusLibrary.SC2Mod)
The Base Mods all have a dependency on a mod file who's sole purpose is to be a trigger library, providing useful premade triggers.

# What's Not Inside (Your Mod!)
There's one thing that's missing from this download and that's the file mod *you* need to make. Now it's time for some actual step by step instructions on getting started.

1. Copy both the Base Mod and Extender Mod to your StarCraft II\Mods folder.
2. Open the editor and click on File -> New... or press Ctrl-N
3. Select Dependent Mod and click Next
4. Choose Custom dependencies, click on Modify... and then Add Other...
5. Select and add the VanillaPlusCMP_BASE.SC2Mod file you copied in step 1.
6. Save your new mod with any name you want. Place it (or a copy of it) into your StarCraft II\Mods folder.
7. Open the VanillaPlusCMP_EXT.SC2Mod file in the editor.
8. Go to File -> Dependencies. And remove VanillaPlusCMP_BASE.SC2Mod.
9. Press Add Other... and select your mod file.
10. Congratulations, now all of the map files are loading your new mod file.

# Vanilla+ Banks

VanillaPlusLOTVPrologue
VanillaPlusLOTV
VanillaPlusNCO

# Rules
