## Automatic Load Order Checker

The Automatic Load Order Checker can detect if you

* use mods that are incompatible with FROST
* use mods that are outdated or broken
* forgot to install a required mod from this guide
* sorted your mods correctly

Copy and paste the content of your **loadorder.txt** into this text field, and press the button.
Make sure that you copy all the content of your load order into the text field.

!!! info
    The Automatic Load Order checker is especially useful if you add mods from outside of this guide or from the Additional Mods section.

??? info "How to find your loadorder.txt" 
    === "MO2"
        If you use **MO2**, you can find your **loadorder.txt** by:

        1. Clicking on the folder icon in MO2
        2. Selecting "Open profile folder"
        3. The Windows Explorer will open the folder which contains the **loadorder.txt**

        ![MO2 LO location](../assets/images/mo2_find_loadorder_file.png)

    === "Vortex"
        If you use **Vortex**, you can find your **loadorder.txt** here:

        ![Vortex LO location](../assets/images/vortex-load-order-find.png)

        Alternatively, you can find your **loadorder.txt** in `C:/Users/[YourUsername]/AppData/Local/Fallout4`

!!! warning "A Small Warning"
    The load order checker is not perfect, it won't find every problem, and in rare cases it sometimes complains when it should not.
    However, it works well enough and will definitely help you a lot if something is really wrong.
    If you need help, visit the [FROST Discord Server :simple-discord:](https://discord.com/invite/BaKsm7Fn4A).
    
    The load order checker is not smart enough to check if you use a mod that requires a patch for FROST.

### Put the content of your load order here!

<textarea id="loadordertxt" name="txtBody" rows="10" cols="100"></textarea>


[primary color]: ../setup/changing-the-colors.md#primary-color
[accent color]: ../setup/changing-the-colors.md#accent-color
[CheckLoadOrder]: javascript:checkLoadOrder()

[Check Load Order][CheckLoadOrder]{ .md-button .md-button--primary }


<div id="content"></div>

<script>

const required_plugins =  [
            "Unofficial Fallout 4 Patch.esp",
            "FROST.esp",
            "RedsFrostFixes.esp",
            "aFrostMod.esp",
            "FROST - UFO4P Patch.esp",
            "FCF_Main.esp",
            "FCF_Previsibines.esp"
        ];
const frost_core_plugins = [
            "FROST.esp",
            "RedsFrostFixes.esp",
            "aFrostMod.esp",
            "FROST - UFO4P Patch.esp"
  ];

const incompatible_plugins =  [
            "RoomBoundPortalFix_Q.esp",
            "WorkshopFramework.esm",
            "unofficial fallout 4 patch.esp",
            "ManufacturingExtended.esp",
            "SS2_DLCSettlerPatch.esp",
            "Modern Weapon Replacer - Glock 19x Ardent117 - 10mm Pistols.esp",
            "Modern Weapon Replacer - Glock 19x Ardent117 - Deliverer.esp",
            "Modern Weapon Replacer - Glock 19x Ardent117 - Gamma Guns.esp",
            "Modern Weapon Replacer - CombinedArmsEXPack - Mk12 - Handmade Rifles.esp",
            "Modern Weapon Replacer - CombinedArmsEXPack - Mk12 - Combat Rifles.esp",
            "Modern Weapon Replacer - CombinedArmsEXPack - Mk12 - Assault Rifles.esp",
            "ValdacilsItemSorting-00-ValsPicks-DLCVersion.esp",
            "ValdacilsItemSorting-00-ValsPicks-NoDLCVersion-VanillaWeight.esp",
            "ValdacilsItemSorting-00-ValsPicks-NoDLCVersion.esp",
            "ValdacilsItemSorting-00-ValsPicks-DLCVersion-VanillaWeight.esp",
            "LOST - AWKCR VIS-G Items and Weight.esp",
            "Companion Infinite Ammo.esm",
            "Energy Weapon Replacer - Wattz Laser Gun - Institute Guns.esp",
            "Energy Weapon Replacer - Wattz Laser Gun - Laser Guns.esp",
            "Energy Weapon Replacer - Wattz Laser Gun - Laser Muskets.esp",
            "Modern Weapon Replacer - AK74M - Handmade Rifles.esp",
            "Wanderer Description Fix.esp",
            "Alias - SuperMutants.esp",
            "Alias - Gunner.esp",
            "Alias - Brotherhood.esp",
            "Alias - Triggermen.esp",
            "Alias - Raiders.esp",
            "ImmersiveLegendaryMutations.esp",
            "LegendariesTheyCanUse.esp",
            "Stuff of Legend.esp",
            "Stuff of Legend - Far Harbor.esp",
            "ECO.esp",
            "Penetration Framework.esp",
            "Better Explosives Redux.esp",
            "ECO_INNRoverride.esp",
            "CALIBER-COMPLEX.esm",
            "WeaponsFramework.esm",
            "Armament.esp",
            "htcwHighLevelPerks.esp",
            "FAR.esp",
            "Conquest.esp",
            "MAIM Distributor.esp",
            "MAIM 2.esp",
            "MAIM 2 - Dismemberment Patch.esp",
            "MAIM 2 - EZ Keywords.esp",
            "MAIM 2 - Point Lookout.esp",
            "MAIM 2 - Russian Stimpak Patch.esp",
            "MAIM 2 - Stimpaks Help You Breathe Patch.esp",
            "MutilatedDeadBodies.esp",
            "AnotherLife.esp",
            "Machete Damage Boost .esp",
            "LongerDrugEffects.esp",
            "FastSwordsMeleeRebalance.esp",
            "RangedWeaponRebalance.esp",
            "SpectacleIslandBoat.esp",
            "HiPolyFacesCompanionPlugin.esl",
            "ArmoredRaiderLeveledList.esp",
            "CaN - Player Pony.esp",
            "FatherCompanion.esp",
            "No Perk Level Requirements ALL DLC 3.0.esp",
            "Perks76.esp",
            "vertunlockminutemenpilot.esp",
            "Settlement PreCombine Changes.esp",
            "SS2.esm",
            "PerkReset.esp",
            "AAF_Violate.esp",
            "AnimatedRadaway.esp",
            "Animated Drinking.esp",
            "MilitarisedMinutemen_PatchesAddon.esp",
            "NW_FROST_Extended.esp",
            "Legendary Apocalypse.esp",
            "ArmorClothingOverhaul.esp",
            "ACO_DLCw03.esp",
            "Better Armor.esp",
            "Militarized Minutemen - Craftable Outfits.esp",
            "ExpandedBallisticWeave.esp",
            "NoRailRoadBallisticWeave.esp",
            "Brotherhood Power Armor Overhaul.esp",
            "The Deadly Commonwealth Expansion.esp",
            "PiperCaitCurieDialogueOverhaul.esp",
            "Stm_DiamondCityExpansion.esp",
            "UniquePlayer.esp",
            "NewSanctuary.esp",
            "WelcometoGoodneighbor.esp",
            "Extended weapon mods.esp",
            "More Cooking 1_1.esp",
            "SimSettlements_Patch_Nukaworld.esl",
            "ProjectMojave.esm",
            "SKK476OpenWorld.esp",
            "Loads.esm",
            "NewCalibers.esp",
            "ArmorKeywords_Patch_INNR_UFO4P.esp",
            "ArmorKeywords.esm",
            "DLCUltraHighResolution.esm",
            "Armorsmith Extended.esp",
            "Weaponsmith Extended 2.esp",
            "Better Locational Damage.esp",
            "Fallout 4 NPC Scaling and Enemy Buff 1.0.esp",
            "BLD - Leveled Lists - DLC.esp",
            "Crafting Mastery.esp",
            "Better Locational Damage - DLC_Automatron.esp",
            "Better Locational Damage - DLC_WWorkshop.esp",
            "Better Locational Damage - DLC_Nuka_World.esp",
            "Better Locational Damage - DLC_Far_Harbor.esp",
            "Loads of Ammo - Leveled Lists.esp",
            "Killable Children.esp",
            "Gas Mask ArmorKeywords.esp",
            "Gas Mask NPC.esp",
            "RaiderOverhaul.esp",
            "WeightlessMods.esp",
            "Better Locational Damage - Ghoul Edition.esp",
            "Better Locational Damage.esp",
            "UnbogusNPCScaling.esp",
            "UnbogusFallout.esp",
            "MK_Agony.esp",
            "Better Perks.esp",
            "WeightlessSpecialAmmo.esp",
            "TacticalTablet_Pip-BoyFlashlight.esp",
            "Agony_IAF_Patch.esp",
            "Z_Horizon.esp",
            "Z_Architect_EnhancedSettlements.esp",
            "Z_Architect_EnhancedSettlements_DLC.esp",
            "Z_Architect_Extras.esp",
            "Z_Architect_HomePlate.esp",
            "Z_CameraAddon.esp",
            "Z_Extras.esp",
            "Z_Horizon_DEFUI.esp",
            "Z_Horizon_DEFUI_MenusOnly.esp",
            "Z_Horizon_Desolation.esp",
            "Z_Horizon_Mode_Scavenger.esp",
            "Z_Horizon_Optional_ShortNaming.esp",
            "Z_Horizon_StrictCarryWeight.esp",
            "Z_Horizon_Timescale.esp",
            "Z_Horizon_WeaponPack01.esp",
            "Z_SettlementLimits.esp",
            "Z_Horizon_DLC_Automatron.esp",
            "Z_Horizon_DLC_FarHarbor.esp",
            "Z_Horizon_DLC_Nuka.esp",
            "Z_Horizon_DLC_Workshop01.esp",
            "Z_Horizon_DLC_Workshop02.esp",
            "Z_Horizon_DLC_Workshop03.esp",
            "Wasteland Heroines Replacer All in One_2.0.esp",
            "PRP.esp",
            "PPF.esm",
            "DamnApocalypse_CORE.esm",
            "America Rising - A Tale of the Enclave.esp",
            "DarkerNights.esp",
            "SimSettlements.esm",
            "SS2Extended.esp",
            "LegendaryModification.esp",
            "Companion Infinite Ammo.esp",
            "StartMeUp.esp",
            "LootableVertibirds.esp",
            "HeightstestNukaWorld.esp",
            "Heightstest.esp",
            "AnimChemRedux.esp",
            "DiamondCityAutoClose.esp",
            "W.A.T.Minutemen.esp",
            "More Armor Slots - All Dlc.esp",
            "More Armor Slots.esp",
            "BetterModDescriptions.esp",
            "BetterModDescriptionsLite.esp",
            "DeadlierDeathclaws.esp",
            "CommonwealthChooksAndBunnies.esp",
            "True Legendary Enemies.esp",
            "CommonwealthCritters.esp",
            "CommonwealthCritters - Both DLC.esp",
            "CommonwealthCritters - Far Harbor.esp",
            "CommonwealthCritters - Nuka World.esp",
            "WorldwideGhoulsV400.esl",
            "WorldwideGhoulsV400.esp",
            "Give Me That Bottle.esp",
            "moreuniques.esp",
            "lovingcait.esp",
            "lovingpiper.esp",
            "busty grrl.esp",
            "lovingcurie.esp",
            "automatron protectrons expanded.esp",
            "angler.esp",
            "the deadly commonwealth expansion.esp",
            "buffed minutemen.esp",
            "ConcealedArmor.esm",
            "Pip-Boy Flashlight.esp",
            "Live Dismemberment - Brutal.esp",
            "Live Dismemberment - Insane-o.esp",
            "Live Dismemberment - Liebermode.esp",
            "Live Dismemberment - Mental.esp",
            "Live Dismemberment - Mind-Blowing.esp",
            "Live Dismemberment - POSTAL.esp",
            "Live Dismemberment - Regular.esp",
            "BetterCompanions.esp",
            "AWKCR - Mod Power Armor Engine Glitch Fix.esp",
            "Campsite-AWKCR.esp",
            "WestTekTacticalOptics-AWKCR.esp",
            "AutomatronUnlocked.esp",
            "Scavver's Toolbox.esp",
            "MojaveImports.esp",
            "VendorItemSteal.esp",
            "MegaExplosions_x1.5.esp",
            "nuka_world_vb_height_fix.esp",
            "UD_AlternateFarming_for_FROST.esp",
            "IV_Frost_Fungus_Farming.esp",
            "Jacq-FROST-CK-base.esp",
            "Jacq-FROST-NoMods.esp",
            "Jacq-FROST.esp",
            "Cleaner Railroad HQ Environment.esp",
            "DITC - Cooking Outputs Improved.esp",
            "ChildrenofGoodneighbor.esp",
            "Performance Enhancing Drugs.esp",
            "Immersive Alcoholic Drinks.esp",
            "MaleCait.esp",
            "Publick Occurrences Expanded.esp",
            "AnimatedIngestibles.esp",
            "SimHomestead.esp",
            "No Bloody Mess.esp",
            "SSNPC - Minutemen.esp",
            "RaiderFaceVariety_2.0.esp",
            "EK - MojaveImports.esp",
            "LoreFriendlySurvivalChems.esp"
        ];

const bad_plugins =  [
            "FrostFallUIPatch.esp",
            "FunctionalTank.esl",
            "M8r_Item_Tags_Vanilla.esp",
            "FROST-More Armor Slots.esp",
            "FROST - Backpack agility fix.esp",
            "FROST - Blight Brew Fix.esp",
            "Frost - NewGame.esp",
            "RRTV_FROST_EleanorRestored.esp",
            "FROST - Fungal Purge Patch.esp",
            "FROST - Fungal Purge Patch Chemist Edition.esp",
            "FrostMasksAndHelmets.esp",
            "FROST_NPCs-No-Ammo-Use.esp",
            "FROST_SimplifiedSorting_NPCs-No-Ammo-Use.esp",
            "Moneyswap.esp",
            "FROST - Fungal Purge fix.esp",
            "Frost Water Patch.esp",
            "shep 4thdoor.esp",
            "FrostACOBetterArmors.esp",
            "xx_FrostAndAgony.esp",
            "Ozzy.esp",
            "FROST Alliance Fix.esp",
            "CannibalWithSanity.esp",
            "Frost Buggs Bunny.esp",
            "Craftable Liquor Original.esp",
            "FrostACOBetterArmors.esp",
            "Frosty Cazador.esp",
            "FrostFungalStew.esp",
            "Frost Fatigues 2.0.esp",
            "Federation Hostile.esp",
            "Friendly Alliance Hostle Federation.esp",
            "Friendly Cannibals Hostile Federation.esp",
            "Friendly Remnants.esp",
            "Friendly Themis Hostile Federation.esp",
            "FROST Fusion Core Rebalance.esp",
            "Chill Weapon Weights.esp",
            "Frost Hunter.esp",
            "Power Helmet Rad Patch.esp",
            "FrostLoneWandererWithSettlements.esp",
            "FrostIsAgony.esp",
            "FrostWarning.esp",
            "Water Filter Not Junk.esp",
            "Frost Weaver.esp",
            "FungalPurgeEdit.esp",
            "Gas Mask FROST.esp",
            "FROST-MoreVoices.esp.3.esp",
            "FROST - KrebsAK Patch.esp",
            "Frost Wastland guide replacer name changes.esp",
            "ZygsFrostStart.esp",
            "Grhk_FROST_VIS-G_GMTBottle_Patch_v1.3.esp",
            "FROSTfix.esp",
            "frostdiamondremoval.esp",
            "FROST_WorkshopPatch.esp",
            "FROSTIntPR.esp",
            "FROSTIntPR_MoreDoors.esp",
            "FROSTIntPR_NW.esp",
            "FROSTIntPR_UIL.esp",
            "FROSTExtPR.esp",
            "FROSTExtPR_NW.esp",
            "FROSTExtPR_UEL.esp",
            "FROST NW Previs Patch.esp",
            "Frost-AWKCR Patch.esp",
            "Frost Construction.esp",
            "LD-Frost - Brutal.esp",
            "LD-Frost - Liebermode.esp",
            "LD-Frost - Regular.esp",
            "FROST Portable Instant Workbench.esp",
            "NPCLimitedAmmo - Automatron.esp",
            "NPCLimitedAmmo.esp",
            "FROST Tomato Wheat.esp",
            "Grhk_FROST_Weightless_Ammo.esp",
            "MK_Agony_VIS patch Non survival.esp",
            "xxFrost_Dogmeat.esp",
            "FCF_PrevisibinesDoors.esp",
            "FCF_PrevisibinesNW.esp",
            "FCF_PrevisibinesNW_UEL.esp",
            "FCF_PrevisibinesNW_UIL.esp",
            "Freeze.esp",
            "FROST Feral Fix.esp",
            "FrostNukaWorld.esp",
            "FROSTmoreDoors.esp",
            "ArgonnFROSTSanityTweakPatch.esp",
            "Frost PipTab.esp",
            "Z_LevelUp_HealingRemoval.esp",
            "FROSTHuntingRifleToSVT40.esp",
            "FROSTCombatRifleToRU556.esp",
            "FROST_Opal_patch.esp"

        ];

const not_recommended_plugins =  [
            "Better Manufacturing.esp",
            "ValdacilsItemSorting-Mods.esp",
            "BetterItemSorting.esp",
            "Regening Life Giver.esp",
            "True Damage.esp",
            "MiscellaneousPerksPack.esp",
            "SKKHeadshotAnyActor.esl",
            "CaN.esm",
            "RealisticHunting.esp",
            "More Antibiotic Loot.esp",
            "More Power Armour Mods.esp",
            "More Power Armour Mods - Automatron.esp",
            "Alex_Stripper_Pole_2.esp",
            "Scrap Everything - Ultimate Edition.esp",
            "Famished.esp",
            "CombinedArmsNV.esp",
            "Damage Threshold.esm",
            "Mycophagy.esp",
            "FO4_AnimationsByLeito.esp",
            "Mutated Lust.esp",
            "SavageCabbage_Animations.esp",
            "LivingParasiteArmor.esp",
            "Atomic Lust.esp",
            "Marmo1233 - PowerArmorAirdrop.esp",
            "AAF_CreaturePack01.esp",
            "AAF_CreaturePack02DLC.esp",
            "TraumaOverrideHarness.esp",
            "AnimalLoverWastelandSeducer.esp",
            "LegendaryDropBugfix.esl",
            "TortureDevices.esm",
            "WashOutThatCum.esl",
            "AnimeRace_Nanako.esp",
            "Fleshsmith.esp",
            "SettlementAttacksBeyondFH.esp",
            "SettlementAttacksBeyondNW.esp",
            "NoRecoilReset.esp",
            "Gauss Non-explosive Rounds.esp",
            "NPCLimitedAmmo - Automatron.esp",
            "fusioncore permanent.esp",
            "Locksmith.esp",
            "Locky Bastard.esp",
            "AmmoCrafting.esp",
            "ImmersiveVendors.esp",
            "[ARR] FallEvil - Mega Zombie Pack.esp",
            "[ARR] FallEvil - Zombie Dogs REVisited.esp",
            "[ARR] FallEvil - Palehead.esp",
            "FallEvil - Complete Edition.esp",
            "Orphans.esp",
            "SurvivalistFirstAid.esp",
            "Atomguard.esp",
            "Autumn Overhaul.esp",
            "MoreWildlife.esl",
            "EvilInstituteHD2K.esl",
            "Bashed Patch, 0.esp",
            "Simple Ballistic Weave Expansion.esp",
            "P.A.C. Ammo Factory.esp",
            "Professional Ammo Crafting.esp",
            "WeightlessMods.esp",
            "WeightlessJunk.esp",
            "WeightlessMods.esp",
            "WeightlessAid.esp",
            "NoMedicsNoAmmoWeight.esp",
            "SimpleProstitutes.esl",
            "No Essential Npcs.esp",
            "ExplosionKnockdown.esp",
            "TheMobileMechanic.esp",
            "fusioncore permanent.esp",
            "XP From Companion Kills.esp",
            "Consistent Power Armor Overhaul.esp",
            "Brotherhood Power Armor Overhaul.esp",
            "AnimatedIngestibles.esp",
            "AnimatedInjestibles_RobotFix.esp",
            "Minuteman Watchtowers.esp",
            "SimpleProstitutes",
            "Realistic Survival Damage.esp",
            "CraftingFramework.esp",
            "Buildable_PAFrames.esp",
            "WeightlessJunk.esp",
            "More Power Armour Mods SPA.esp",
            "MK_Agony.esp",
            "Feral Ghoul Bite Skills.esp",
            "SolarPower.esp",
            "Safe SSEx.esp",
            "SSEX.esp",
            "Water Purification Stations.esp",
            "CraftableAmmo.esp",
            "CraftableAmmo_plus.esp",
            "Insignificant Object Remover.esp",
            "YouAreSPECIAL.esm",
            "jags78_ExtendedAgony.esp",
            "MK_Agony_Unofficial_Patch.esp",
            "ExpandedQuickCleanJamaicaPlain.esp",
            "Agony_IAF_Patch.esp",
            "MK_Agony_non Survival.esp",
            "AdvancedNeeds2_Expansion_01_Ghoulified.esp",
            "AdvancedNeeds2_Expansion_02_Spoilage.esp",
            "AdvancedNeeds2_Expansion_05_Gasmasks.esp",
            "AdvancedNeeds2_Patch_Campsite.esp",
            "AdvancedNeeds2_Patch_DLC.esp",
            "Flashy_CommonwealthFishing.esp",
            "Flashy_CommonwealthFishingFarHarborAddon.esp",
            "AdvancedNeeds2.esp",
            "Facials.esp",
            "FROST_weather_no_headache.esp"
        ];

const fcf_check_plugins = [
            "FCF_Main.esp",
            "FCF_Previsibines.esp",
            "FCF_Previsibines-TheForest.esp",
            "FCF_Previsibines-JSRSRegions.esp",
            "FCF_Previsibines-TheMarshlands.esp",
            "FCF_Previsibines-ELFX.esp",
            "FCF_Previsibines-WinterRedone.esp",
            "FCF_Previsibines-WinterRedoneELFX.esp",
            "FCF_HotfixELFX.esp",
            "FCF_HotfixWR.esp",
            "FCF_Previsibines-MMHelipad.esp",
            "FCF_Previsibines-Oberland.esp",
            "FCF_Previsibines-Drawbridges.esp",
            "FCF_Previsibines-MFG.esp",
            "FCF_Hotfix.esp",
            "FCF_Previsibines-Hotfix.esp",
            "PLI_USAF_Satellite_Station_Olivia.esp",
            "PLI_USAF_Olivia FROSTified.esp",
            "PLIDHP_Previs.esp",
            "WCLINS_Previs.esp",
            "WCLINPP_Previs.esp",
            "WCLIRIL_Previs.esp",
            "WCLINRR_Previs.esp",
            "WCLIPET18F_Previs.esp",
            "WCLILGP_Previs.esp",
            "Vivid Waters.esp",
            "Synthesis.esp",
            "SatelliteWorldMap.esp",
            "FOLIP - Before Generation.esp"
        ];


  function removeAllHtmlChildNodes(parent){
    while (parent.firstChild) {
        parent.removeChild(parent.firstChild);
    }
  }
  var counter_checker = 0;

  function myPrint(output_list, title, message) {
      if(output_list.length == 0){
        return
      }
      var p = document.createElement("ul");
      let heading = document.createElement('h2');
      heading.innerHTML = title;
      let description = document.createElement('p');
      description.innerHTML = message;
      p.appendChild(heading)
      p.appendChild(description)
      output_list.forEach(plugin => {
          if (plugin != "" && plugin != null){
            let t = document.createElement("li")
            t.innerHTML = plugin;
            p.appendChild(t)
          }
        }
      )
      document.getElementById("content").appendChild(p);
      counter_checker++
  }


  function checkForCCmods(plugin_list){
    var result_list = [];
    plugin_list.forEach(plugin => {if (plugin.startsWith("cc")){result_list.push(plugin)}});
    return result_list;
  }

  function checkForMissingPlugins(plugin_list, check_list){
      var result_list = [];
      check_list.forEach(plugin => {if (!plugin_list.includes(plugin)){result_list.push(plugin)}});
      return result_list;
  }

  function checkForExistingPlugins(plugin_list, check_list){
      var result_list = [];
      check_list.forEach(plugin => {if (plugin_list.includes(plugin)){result_list.push(plugin)}});
      return result_list;
  }

  function checkFrostCore(plugin_list, check_list){
    var result_list = [];
    for(let i=1; i < check_list.length; i++){
      if (plugin_list.indexOf(check_list[i]) != plugin_list.indexOf(check_list[i-1])+1 ){
        result_list.push(check_list[i]);
      }
    }
    return result_list;
  }

  function checkFrostPluginOrderBefore(plugin_list){
    var result_list = [];
    for(let i = 0; i < plugin_list.indexOf("FROST.esp"); i++){
        let plugin = plugin_list[i];
        pluginS = plugin.toLowerCase()
        if (pluginS.includes("frost") || pluginS.includes("rff")){
          result_list.push(plugin)
        }
    }
    return result_list;
  }

  function checkFrostPluginOrderAfter(plugin_list){
    var result_list = [];
    //alert(plugin_list)
    //for(let i = plugin_list.indexOf("FROST.esp"); i < plugin_list.length-1; i++){
    let offset = plugin_list.indexOf("FROST - UFO4P Patch.esp");
    if (offset < 0){
      offset = plugin_list.indexOf("FROST.esp");
    }
    if (offset < 0){
      return [];
    }
    for(let i = offset; i < plugin_list.length-1; i++){
        let plugin = plugin_list[i];
        let pluginS = plugin.toLowerCase()
        //alert(plugin)
        const exception_list = ["IV_Misc_BoiledWaterBottles.esp", "IV_HC_Perk_Updated.esp","Cat Meat Recipe.esp","SatelliteWorldMap.esp", "PLI_USAF_Satellite_Station_Olivia.esp", "M8r Complex Sorter.esp", "ChillGhouls.esp", "VividWeatherDarkerNWindier.esp", "Nuclear weather.esp",
        "PollutedClimate.esp", "Calamity Weathers.esp", "Calamity Weathers - Far Harbor.esp", "Calamity Weathers - Nuka World.esp", "Calamity Weathers - Winter climate.esp", "PollutedClimate-Winter.esp", "Simple Winter Weather.esp"];
        if (!pluginS.includes("frost") && !pluginS.includes("rff") && !pluginS.includes("fcf") && exception_list.indexOf(plugin_list[i]) < 0){
          result_list.push(plugin)
        }
    }
    return result_list;
  }

    function checkPluginOrder(plugin_list, check_list){
      var result_list = [];
      for (let i = 0; i < check_list.length-1; i++){
          let plugin1 = check_list[i];
          let plugin2 = check_list[i+1];
          let pl1 = plugin_list.indexOf(plugin1);
          let pl2 = plugin_list.indexOf(plugin2);
          if (pl1 < 0 || pl2 < 0){
            continue
          }
          if (pl1 > pl2){
            result_list.push(plugin1);
          }
      }
      return result_list
  }

  function checkEndOfLO(plugin_list, check_list){
    var exist_list = checkForExistingPlugins(plugin_list, check_list)
    var result_list = []
    const sumbo =   plugin_list.length - exist_list.length
    for (let i = 0; i < check_list.length; i++){
          let plugin1 = check_list[i];
          let pl1 = plugin_list.indexOf(plugin1);
          if (pl1 < sumbo && pl1 >= 0){
            result_list.push(plugin1);
          }
      }
      return result_list
  }


  function checkLoadOrder(){
    counter_checker = 0;

    // Get the load order from the input field
    removeAllHtmlChildNodes(document.getElementById("content"))
    var load_order_text = document.getElementById('loadordertxt').value;
    var plugins = load_order_text.split('\n');

    // In case that the user inserted the content of his plugins.txt, we have to remove some characters at the start of the lines
    for (let i = 0; i < plugins.length; i++){
      plugins[i]  = plugins[i].replace("*", "");
      plugins[i]  = plugins[i].replace("<", "");
      plugins[i]  = plugins[i].replace(">", "");
      plugins[i]  = plugins[i].replace("\"", "");
      plugins[i]  = plugins[i].replace("\'", "");
      plugins[i]  = plugins[i].replace("/'", "");
      plugins[i]  = plugins[i].trim();
    }

    //Ignore all lines that are shorter then 5 characters
    plugins = plugins.filter(plugin => plugin.length > 4);

    //Check if this is a valid load order
    if (plugins.length <= 2){
      return;
    }

    // Get the information from the load order
    const found_cc_plugins = checkForCCmods(plugins);
    const found_missing_plugins = checkForMissingPlugins(plugins, required_plugins);
    const found_incompatible_plugins = checkForExistingPlugins(plugins, incompatible_plugins);
    const found_bad_plugins = checkForExistingPlugins(plugins, bad_plugins);
    const found_not_recommended_plugins = checkForExistingPlugins(plugins, not_recommended_plugins);
    const found_wrong_order_plugins =  checkPluginOrder(plugins, required_plugins);
    const found_wrong_order_before_frost_plugins = checkFrostPluginOrderBefore(plugins, required_plugins);
    const found_wrong_sorted_fcf_plugins = checkEndOfLO(plugins, fcf_check_plugins);
    const found_wrong_order_after_frost_plugins = checkFrostPluginOrderAfter(plugins);
    const found_wrongly_sorted_core_plugins = checkFrostCore(plugins, frost_core_plugins);

    const cc_description = "Creation Club Content is often incompatible with FROST, immersion-breaking or needs a patch. There are currently no patches for CC content for FROST. Please remove all CC mods, unless they add paint for Power Armor, Armors or Weapons.";
    myPrint(found_cc_plugins, "Creation Club Content", cc_description);
    const missing_description = "You are missing the following plugins. Please install them and put them into the right spot in your load order!";
    myPrint(found_missing_plugins, "Missing Plugins", missing_description);

    const core_sorted_wrong_description = "The following plugins are \"Main Files\" of FROST, and you did not sort them correctly (or even did not install them at all)! Take a look again at Sorting Rule 5 and the example load order!"
    myPrint(found_wrongly_sorted_core_plugins, "Frost Main Files" ,core_sorted_wrong_description)

    const incompatible_description = "You are using mods that are incompatible with FROST. Please remove them!";
    myPrint(found_incompatible_plugins, "Incompatible Plugins", incompatible_description);

    const problematic_description = "The following plugins are problematic/outdated and should also be removed";
    myPrint(found_bad_plugins, "Problematic Plugins", problematic_description);

    const not_recommended_description = "The following plugins are not-recommended to be used with FROST, as they either need a patch that is way to complicated to make, or they do or add things that are already present in FROST, or because they are outdated/not necessary anymore.";
    myPrint(found_not_recommended_plugins, "Not-Recommended Plugins", not_recommended_description);
    const wrong_order_description = "The following plugins are sorted wrong. Please check the Load Order section to make sure that they are sorted correctly!";
    myPrint(found_wrong_order_plugins, "Following Plugins are sorted wrong", wrong_order_description);
    const wrong_order_before_frost_description = "All FROST mods need to be loaded AFTER \"FROST - UFO4P Patch.esp\"! The following FROST mods are not loaded after \"FROST - UFO4P Patch.esp\":";
    myPrint(found_wrong_order_before_frost_plugins, "FROST Plugins are sorted wrong", wrong_order_before_frost_description);

    const wrong_order_after_frost_description = "You should load these frost unrelated mods before Frost.esp, unless you know what you are doing and know how to use xEdit. If you are unsure about this, go to the FROST Discord and ask there for clarification."
    myPrint(found_wrong_order_after_frost_plugins, "Normal Plugins are sorted wrong", wrong_order_after_frost_description);

    const fcf_lo_end_description = "Please load the following plugins at the END of your load order, and read the sorting rules from above again VERY carefully."
    myPrint(found_wrong_sorted_fcf_plugins, "Problems at the end of the load order.", fcf_lo_end_description);

    if (counter_checker == 0){
        myPrint([""], "No problems were found", "The checker couldn't find any problems. Keep in mind that the checker is not perfect, there could still be something wrong with your load order.");
    }
}
</script>

