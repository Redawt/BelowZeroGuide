# General

## Where can I get help?

You can get help over at the [**FROST Discord :simple-discord:**](https://discord.com/invite/BaKsm7Fn4A).

## How much disk space is needed?

You need around 15 GB of disk space for the MO2 instance, and the downloaded and installed mods from this guide (the mods from the additional mods section are not included in this number!).
Additionally, you need the disk space for Fallout 4, which is around 33-36 GB (depending on if you also have the Creation Kit installed).
So you need around 55 GB of free disk space, that way you have a additional space left for other mods.

## My game crashes, has FPS issues, objects flicker/disappear, ...

Please read the [Troubleshooting Section](../../guide/troubleshooting) and the [compatibility FAQ section](../faq-compatibility).

## Any mod recommendations?

Yes, we have recommendations for additional mods that either work out of the box or need a patch, like weapon mods.
Check out the [Additional Mods Section](../../additional-mods).

## Why does this guide require downgrading Fallout 4?

1. It makes it easier to offer support for GOG and Steam users
2. Several mods are not compatible with the Next-Gen version of Fallout 4
3. The Next-Gen version of Fallout 4 has some bugs that would require installing additional bug fixes
4. The FROST development team did not have the time to ensure that FROST runs properly with the Next-Gen version

## Can I have a downgraded and a non-downgraded version of Fallout 4 at the same time?

Yes, this is possible. You need to own the game to times though, on GOG and on Steam.
The GOTY version on both platforms costs 10 dollars/euros on sale.
You would need to use the GOG version for your FROST setup, and your Steam version for your non-FROST setup.
Additionally, this only works properly if you use MO2, Vortex might not be able to properly handle two different game versions.


## Why is this guide centered around using MO2? Why not Vortex or NMM?

**Vortex** was created around the idea of LOOT managing the load order, making modding seem simple and easy (see below why that's a bad idea).
While the option to manually order plugins exists, it's designed to be as unintuitive as possible - the user needs to select the position of every plugin from a dropdown menu, based on relative position to other mods (load X after Y, load X before Z), or use a graphical, node based interface.
Additionally, it does not track generated files, and the deployment logic can be confusing to the user. 

**Nexus Mod Manager (NMM)** is outdated/abandoned, have no virtual file system or even dynamic movement of mods with loose files, which can lead to complete mod or game reinstalls in case the user wants to change the load order, or installed mods in a wrong order. There is a community maintained version of NMM that still gets updates, but it still has most of the flaws mentioned above.

## Why should I not use LOOT?

The LOOT doesn't really have any idea about your mods and their inner structure - it just orders them based on tags in a masterlist managed by volunteers, meaning that it's impossible to account for every single mod and combination of mods. If you use LOOT (or any other auto-sorting feature for mods), chances are your load order gets messed up.

## Where are save files stored?

You may have noticed that when playing the game through MO2, your save files will not appear in the `Documents` folder like normal. This is because the guide makes use of profile-specific saves, a feature that redirects them to the profile folder of your instance. You can access all of them quickly by selecting the **Saves** tab of MO2 on the right pane. 

!!! warning "Don't reuse saves!"
    Do not re-use vanilla saves or any save from different mod setups! A new character is required for a functional game.

## Why is PANPC not hosted on Nexusmods?

In 2021, Nexusmods tried to secretly change their Terms of Service. Those changes allow Nexusmods to keep your mods on their platform by any means (you can not ask them to delete your files from their servers), to **change** them, **redistribute them**, etc. Basically they have the right to do with your mods what they want. 
After an initial backlash (some people noticed the secret ToS change), they gave everyone a few weeks to completely delete their mods, and then went through with the ToS changes.

This among some other past bad decisions from Nexusmods turned away many mod authors, who decided to host their mods elsewhere. Please respect the decision of those mod authors. Those mod authors are aware that this makes it a bit less convenient for you, but this is about trust and copyright


## Is it safe to validate game files?

Verifying game files will revert the executable downgrade. You can solve this by re-running the downgrader.

