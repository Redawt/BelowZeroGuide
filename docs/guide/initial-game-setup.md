# Installing the game
<small>
:material-information-box:
This section tells you how to properly install the game, and avoid issues caused by previous mod setups.
</small>

!!! info "Need help?"
    If you run into any issues at any point in the guide, feel free to ask for help on our [Discord Server :simple-discord:](https://discord.com/invite/BaKsm7Fn4A) in the [**#support-and-bugs-frost :simple-discord:**](https://discord.com/channels/238420126985224192/1242558041610522634) channel.

---
## Enabling File Extensions
Before we start, it is important to enable file extensions in Windows.

By default, File Explorer will not show file extensions (such as .exe, .dll, or .esp). These extensions are very important when going through the guide, so it is highly recommended to enable visible file extensions: 

1. Open File Explorer
2. Select the **View** tab at the top
3. Enable ==File name extensions== in the **Show** section

![File Extensions Image](../assets/images/file_extensions.webp)

---
## Making a Clean Install of Fallout 4
This section explains how to make a Clean Install of Fallout 4 to ensure its properly installed and no left-over files from previous mods are present.

### Choosing a Location
==A clean installation== is not only required to get rid of any potential leftover mod files, but also to make sure the game is installed in a safe location. Here is what you need to know when choosing where to install your game:

* **Avoid any default Windows folders**: This includes but is not limited to `C:\Program Files`, `C:\Program Files x86`, your `Desktop` and your `Documents` folders. This is because users lack write access to Program Files, while Desktop and Documents are often managed by OneDrive. This can cause many issues with the game and any modding tools.

    An example of a safe location is `C:\Games`

* **Install on an SSD if possible**: Having the game on an SSD will drastically improve loading times and decrease stuttering.


### Uninstalling the game

!!! warning ""
    **If you never installed the game before, go directly to the ==Installing the game== part.**

!!! danger ""
    **If you already uninstalled the game, make sure to follow step 4, 5 and 6 to ensure there are no leftovers.**

=== "Steam"
    1. Open Steam and go to your ==Library==
    2. Find ==Fallout 4== in the list
    3. Right-click on it and select ==Manage -> Uninstall==
    4. Navigate to `Steam\steamapps\common\` and, if present, delete the **Fallout 4** folder
    5. Navigate to `Documents\My Games` and delete the **Fallout4** folder
    6. Navigate to `AppData\Local` and delete the Fallout4 folder

=== "GOG"
    1. Open GOG Galaxy
    2. Select ==Fallout 4== in the ==Installed== list, click on the Customization button (the one next to "Play")
    3. Select ==Manage Installation -> Uninstall==.
    4. Navigate to `Fallout 4` folder that previously contained the game, if present, and delete it
    5. Navigate to `Documents\My Games` and delete the **Fallout4** folder
    6. Navigate to `AppData\Local` and delete the Fallout4 folder


### Installing the game
!!! info ""
    Set the game's language to English during or after installing it.
    Non-English versions can cause issues with certain mods, and all mods featured here are in English.

!!! warning ""
    It is strongly recommended installing the games outside any default Windows folders (such as `Program Files (x86)`), as the strict Windows file protections of these folders can break certain mods/tools.

=== "Steam"

    ### Making a new Steam library

    1. Completely exit out of Steam using Task Manager or System Tray.
    2. Download the ==steam_library_setup_tool-3.2.exe== file from [here](https://github.com/LostDragonist/steam-library-setup-tool/releases).
    3. Once downloaded, run the file and add a new entry by clicking ==Add Row==.
    4. Type the chosen path under ==Path==, e.g. `C:\Games\Steam`
    5. Click ==Accept== then ==Yes== if prompted to create a new folder.
    6. The tool will ask to exit, select ==OK==.

    ![Steam Library Tool Setup](/assets/images/Steam Library Tool Setup.webp)

    ### Installing the game in Steam
    1. Open Steam and go to your ==Library==
    2. Find ==Fallout 4== in the list and select ==Install==
    3. Under ==Install to:==, select the library folder created with the tool, which is the second `C:\` entry if you are installing on the main drive. If you already had another steam library (for example on an external drive), you can chose that one instead.
    3. Select ==Next== then wait for the install to finish
 
    <small>
    :material-information-box:
    If you still do not see your new library, restart your PC.
    </small>

    ### Disabling Automatic Steam Updates

    This will prevent Steam from automatically installing Fallout 4 updates, which will break modding support considerably until they gain wide modding support (and the guide's).

    1. In your ==Steam Library==, right-click on ==Fallout 4==, and click on ==Properties==
    3. Click on the drop-down at the top of the right pane underneath **Automatic Updates**
    4. Set it to ==Wait until I launcht the game==.

    <small>
    :material-information-box:
    Since MO2 bypasses Steam's "play" button, Fallout 4 will never automatically update because you will launch the game through MO2.
    </small>


=== "GOG"
    ### Installing the game in GOG
    1. Select ==Fallout 4== in your GOG Library
    2. Click the ==Install== button
    3. Select a save installation folder at ==Install to==
    4. Select ==English== as the language
    4. Click ==Install==

    *No other steps are required for installing the game.*
---
## Key Terminology
Now that the game is installed, there are two folders from it that will be referred to in the guide often:

  - ==Root== folder (where the game is installed): 
    - `Steam\steamapps\common\Fallout 4`

  - ==Data== folder (where all of the game's assets are located):
    - `Steam\steamapps\common\Fallout 4\Data`

---
## Generating Fresh .INI Files

1. Run ==Fallout4Launcher.exe== from the game's ==Root== folder
2. Click OK to both pop-ups that say **Detecting Video Hardware**
    - If there aren't any pop-ups, navigate to `Documents\My Games\Fallout4` and delete all the files ending in **.INI** then retry
3. Click **OK** then **Exit**

<!-- 
### Disabling the [High Resolution Texture Pack/DLC](https://fallout.fandom.com/wiki/High_Resolution_Texture_Pack) from Bethesda
When you installed the game again, it might be possible that you accidentally installed the **High Resolution Texture Pack/DLC** from Bethesda. This DLC takes a lot of disk space, has several bugs/issues, and texture mods achieve much better results.
You should uninstall it.

??? info "Uninstalling the High Resolution Texture Pack/DLC"
    1. Go to your Steam Library by clicking "Library" at the top
    * Click on **Fallout 4**
    * Click on **Support** to the right of Fallout 4
    * Scroll to the bottom, if you have the season pass or a lot of dlc, click **Show all DLC**
    * Click on **High Resolution Texture Pack**
    * Click on "I want to remove this permanently from my game library"
    * **!!! Make sure it says High Resolution Texture Pack at the top, or you'll remove the entire game with no refund !!!**
    * Click **OK**

    **Note for GOG users**: Do the equivalent steps via GOG, unless the High Resolution Texture Pack was not downloaded.
-->

---
--8<-- "docs/mods/utilities/simple-downgrader.md"

--- 
## Removing Creation Content (CC)
=== "Steam"
    #### Description
    * This step removes CC content that has not been patched for FROST and will cause issues
    * These CC files have been added by the Next-Gen update, and while they work on the downgraded version of Fallout 4, they are not yet patched for FROST and should be removed

    #### Uninstallation instructions
    * Open the  **Data** folder (`Steam\steamapps\common\Fallout 4\Data`) in the Windows Explorer
    * Delete the following files from it:
        * `ccBGSFO4044-HellfirePowerArmor.esl`
        * `ccBGSFO4115-X02.esl`
        * `ccBGSFO4116-HeavyFlamer.esl`
        * `ccBGSFO4110-WS_Enclave.esl`
        * `ccBGSFO4096-AS_Enclave.esl`
        * `ccFSVFO4007-Halloween.esl`
        * `ccBGSFO4046-TesCan.esl`
        * `ccSBJFO4003-Grenade.esl`
        * `ccOTMFO4001-Remnants.esl`

=== "GOG"
    GOG users can skip this step.

---
<small>
:material-information-box:
**Note:** You can now move on to the next section.
</small>