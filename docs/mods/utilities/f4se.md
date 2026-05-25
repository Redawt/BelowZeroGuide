## [Fallout 4 Script Extender](https://www.nexusmods.com/fallout4/mods/42147)
:material-tag-outline: `Required` | 
:material-crosshairs-question: `Specific Version` | 
:material-car-shift-pattern: `Manual Installation`

Extends the scripting capabilities of the game.

### Installation Instructions
1. Download **[Old Files - Fallout 4 Script Extender (F4SE) 0.6.23 :material-tray-arrow-down:](https://www.nexusmods.com/fallout4/mods/42147?tab=files&file_id=253313)** from Nexusmods
2. From the downloaded archive, extract ==everything== to the game's Root folder. You can do this easily with either ==7-Zip== or the ==Windows Explorer==, or any other Archive Tool.

    ![F4SE in Root folder](../assets/images/f4se-explorer.gif "How to extract F4SE.")
    

???+ question "What is the Root Folder?"
    If you do not know what the Root folder is, read the Key Terminology section from the Initial Setup page.

### Check if F4SE was correctly installed

Make sure your root folder looks similar to this:

![F4SE in Root folder](../assets/images/after-f4se-installation.png "F4SE in Root folder")


### Add F4SE to MO2

Once F4SE is installed as instructed above, restart MO2 and you should see a new option in the top right drop-down: 

![F4SE in MO2](../assets/images/select_f4se.png "F4SE in MO2")


### Enabling steamloader

=== "Steam"

    Steam users don't need to follow this step, only GOG users.

=== "GOG"

    In MO2 you need to enable add a flag to F4SE so that MO2 can properly start Fallout 4.
    Vortex users do not need to do this step.

    1. Open the **drop-down menu** for the executables in MO2, and select **Edit**
    ![MO2 Exectuable Image](../assets/images/MO2-Edit-Exe.png)
    2. Add `-forcesteamloader` in the **Arguments** section of the **F4SE** executable
    ![MO2 -forcesteamloader](../assets/images/MO2-GOG-Steamloader.png)