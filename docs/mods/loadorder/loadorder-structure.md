## Load Order Structure
This load order structure applies to the mods featured in this guide, as well as all other mods that you can find online.

You need to sort your load order so that it resembles the order of mods as described in this subsection.


#### 1. Bethesda Files

All Bethesda main files: You can not change their order, they always need to be at the top of the plugins section in MO2 and Vortex.

- Fallout4.esm
- DLCRobot.esm
- DLCworkshop01.esm
- DLCCoast.esm
- DLCworkshop02.esm
- DLCworkshop03.esm
- DLCNukaWorld.esm


#### 2. Master files

Put all **.esm files** and **.esmflagged .esp files** here. 

- PANPC.esm
- HUDFramework.esm
- Unofficial Fallout 4 Patch.esp
- ...


#### 3. Frost Unrelated Mods I


Put all mods here that are unrelated to FROST and don't need a patch for FROST.
Weather should not be placed here though, they need to be loaded later if possible.

* GCM_DLC_Automatron.esl
* GCM_DLC_Far_Harbor.esl
* GCM.esp
* Immersive HUD.esp
* M8rDisablePipboyEffects.esp (this is an optional plugin from FallUI Inventory)
* ...


#### 4. Frost Unrelated Mods II


Put all mods here that need a patch for Frost. Load their frost patches at the section marked down below!. Mods that belong here are Lighting Mods, Weapon Mods, Armor Mods, Creature Mods, Mods that edit leveled lists, ...

* SCM.esp
* UltraInteriorLighting.esp
* UltraExteriorLighting.esp
* ...


#### 5. Frost Main Files

The following four plugins must be in this exact order! 

- FROST.esp
- RedsFrostFixes.esp
- aFrostMod.esp
- FROST - UFO4P Patch.esp


#### 6. Other Frost Mods

Put all other FROST standalone mods here.

* RedsFrostBlurRemoval.esp (Optional File)
* RedsFrostExplosionEffects.esp (Optional File)
* FROST - It Snowed.esp
* Frost-Snowy-Weathers.esp
* FROST - LootableCars.esp
  * FROST_LLCars_Intermediate.esp (Optional File)
  * FROST_LLCars_Realistic.esp (Optional File)
  * FROST_LLCars_Scarcity.esp (Optional File)
* FROST - AccessibleMedTekResearch.esp
* FROST - AccessibleFortStrong.esp
* FROST - AccessibleArcJet.esp
* FROST - AccessibleFortHagen.esp
* FROST - SuperMutantLocations.esp
* FROST - Hunkered Down.esp
* FROST - Hunkered Down-Settlements.esp
* FROST Downtown Workbenches.esp
* ...


#### 7. Frost Patches

Put all mods here that patch a certain mod for FROST.

* PANPC FROST Patch.esp
* RedsFrostCampsitePatch.esp
* RedsFrostSCM.esp
* ...

#### 8. Weather Mods

Weather mods need to be loaded here.
This guide doesn't feature weather mods, you can skip step 8. unless you are using a weather mod.

**Notes** 

- The Automatic Load Order checker below does not know which mods are weather mods, and therefore might complain. You can ignore the load order checker in such cases. Certain Weather mods are esm files and can't be loaded here. In that case they need to be loaded at the top of the load order (see rule 1), and require a patch for FROST that needs to be loaded here.
- NACX does not need a patch for FROST anymore and needs to be loaded at the top of the load order

#### 9. Frost Cell Fixes (FCF)

No other files should come after the FCF .esp files, except very special mods (see rule 10).
If you don't follow these rules, bad things will happen!
The FCF_Main.esp and FCF_Previsibines.esp must come first, and in the same order as below. After those two plugins all other FCF plugins must be loaded.

- FCF_Main.esp
- FCF_Previsibines.esp
- (Additional FCF files for patching certain mods)
- FCF_Hotfix.esp (only if there is a Hotfix for FCF)
- ...

#### 10. Exceptions to Rule 9


If you use the following plugins, they need to be loaded after FCF.
Keep in mind that this list is not complete. 
These mods either have speciallcell headers that can be safely loaded after FCF, or provide their own precombines/previs data which needs to overwrite FCF. 
If you use a sorting mod, make sure to let it generate a sorting plugin for your load order specifically, and load it after all other plugins.

- PLI_USAF_Satellite_Station_Olivia.esp
- PLI_USAF_Olivia FROSTified.esp
- Vivid Waters.esp
- Synthesis.esp
- SatelliteWorldMap.esp
- FOLIP - Before Generation.esp
- People Live In mods by Glitchfinder + their FCF patches
- We Can Live In by Glitchfinder + their FCF patches
- (Auto-Generated Item Sorting Mod plugin)
