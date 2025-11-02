# Troubleshooting

<small>
:material-information-box:
This **optional** section tells you what to do in case you run into issues.
</small>

---

!!! info "Don't have any issues?"
    This section is optional and should only be read in case you ran into issues. If you followed sections 1-10 properly, you can start playing FROST, or you can go to [Section 12 "Adding more mods"](../adding-more-mods) if you want to add some additional mods.

## What went wrong?

If followed this guide, and noticed an issue (CTDs, FPS drops, game doesn't start, ...), several things can be the cause of that.

1. You didn't follow the guide correctly
    * You have incompatible mods lingering in your game's Data folder, this is why a [clean slate](../initial-game-setup#making-a-clean-install-of-fallout-4) is required.
    * You didn't read the [**Requirements**](../introduction/requirements.md) section
    * You did not sort your mods correctly
    * ...
2. The guide has an issue, considering that this guide was remade recently errors could have slipped in
3.  If you are using a third-party antivirus, add exclusions to the folder Mod Organizer 2 is in. If that doesn't work, try disabling the antivirus completely and rely solely on Windows Defender (which should work fine once exclusions are present).
4. Your hardware or drivers cause an issue (unlikely, but this can happen)
5. Certain settings in mods need to be changed (unlikely, but this can happen and is often related to 4.)
6. One of the mods from the Below Zero guide has a bug causing your issue
7. You've added additional mods, and they directly or indirectly cause the issue
8. You used quicksaves (they can cause issues with save files in modded setups)
9. You've installed or uninstalled certain mods mid-playthrough


**In any of those cases, we will help you to fix the issue.**


---
## Check for warning messages in MO2

MO2 has several spots where warning triangles can appear.

However, most of the time they indicate that something is wrong that you need to fix.

Here are some of the spots where warning triangles can show up in MO2:

![mo2 profiles menu](../assets/images/mo2_warning_spots.png "MO2 Warning locations")

If warning triangles show up besides a plugin in the plugins section of MO2, you either forgot to install a requirement for the mod, or accidentally installed a patch for a mod that you do not need.


!!! info "Note about the "Overwrite Directory" warning"
    You can ignore the “Overwrite directory” warning in most cases.

    Mod Organizer 2 (MO2) isolates each mod in its own folder, keeping the game’s directories clean and making it easy to see which files belong to which mod. 
    It tricks the game into thinking the mod files are in the game folder, while they actually remain separated.

    Some mods or tools (e.g., F4SE, Creation Kit, Bodyslide, xEdit) generate files or folders at runtime, such as Looksmenu presets, custom mod files or log files.
    Since MO2 doesn’t know where to store these new files (=which isolated folder), it puts them in the default “Overwrite” folder and shows a warning.

    You can disable this warning in MO2’s settings, or configure MO2 to route those generated files into [their own dedicated folder :fontawesome-brands-youtube:{ .youtube }](https://www.youtube.com/watch?v=Ksp_yPq637s).



---
## Help yourself

Before asking us for help though, you should try:

1. Run your load order through the **[Automatic Load Order Checker](../load-order-setup#automatic-load-order-checker)** from this guide
2. Visit the [**FROST Discord :simple-discord:**](https://discord.com/invite/BaKsm7Fn4A) and check out the [**#support-faq :simple-discord:**](https://discord.com/channels/238420126985224192/1244543694359756932) channel. It contains instructions about fixing common issues.
3. Make sure that you did not forget to install a mod you've downloaded when following this guide.

---
## We will help you

If you were not able to fix your issue, we will provide custom support tailored to your issue on the [**FROST Discord :simple-discord:**](https://discord.com/invite/BaKsm7Fn4A) in the [**#support-and-bugs-frost :simple-discord:**](https://discord.com/channels/238420126985224192/1242558041610522634) channel.

Keep in mind that we only offer help in reasonable cases (= you tried your best actually following the guide). 
If you skipped a lot of instructions of the guide, or added dozens or hundreds of mods to your FROST setup, or act unfriendly, we might refuse to help you. 