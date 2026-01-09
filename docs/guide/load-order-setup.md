# Load Order
<small>
:material-information-box:
This section tells you how to sort your mods correctly.
</small>

---
## Sorting is important

After you've installed the mods from the previous sections, you now need to sort your load order.
The load order is a list that tells the game in which order it should load esp/esm/esl plugins.
Those plugins contain changes to vanilla game objects (like quests, items) or add new objects.

Some plugins depend on other plugins, or need to overwrite elements from other plugins (="winning conflicts").
Plugins that are further "up" in your load order can get overwritten by other plugins that are "further down" in your load order.
That's why the base game plugins, like Fallout4.esm, are at the top of your load order.

That is why sorting your load order is important, otherwise features from mods will break, or you will encounter issues like crashes, fps issues and bugs. 


This section provides information on how to sort your load order regarding FROST and the mods featured in this guide, but also for mods which are not featured in this guide. We do not recommend to use LOOT or any other automatic load order sorting tool, as they tend to sort mods wrong (especially FROST mods).

!!! info "Mods without plugins"
    Not all mods have an esm/esp/esl plugin. Certain mods that are part of the guide, like **Buffout 4**, don't have a plugin.

---
## How to sort your mods in your mod manager
Expand the section below to learn how to sort your load order in MO2 and Vortex.

??? abstract "Expand me if you need to know more." 


    === "MO2"

        ![MO2 Panes](../assets/images/mo2-panes.png)

        <div class="grid cards" markdown>

        -   :material-dock-right:{ .lg .middle } __Left Pane__

            ---

            The left pane contains the mods and mod separators you've installed.

            Sort the separators and the mods inside them in the same order as they have been featured in this guide.

            To sort them, you can simply drag & drop the mods and separators around.

            Make sure that the list is displayed by "priority" (it's the default) in the UI. Otherwise you might not be able to move the mods around.

        -   :material-dock-left:{ .lg .middle } __Right Pane__

            ---
            
            The right pane has a "plugins" section. It contains the esm/esp/esl plugins from the mods from this guide.

            They reflect the content of your `loadorder.txt` and `plugins.txt` files, which tell the game how to load your plugins.

            To sort them, you can simply drag&drop the plugins around in the list.

            Make sure that the list is displayed by "priority" (it's the default) in the UI! Otherwise you might not be able to move the mods around.

        </div>

        !!! abstract "Drag & Drop Example"

            Here is an example on how you can drag & drop plugins around in MO2:

            ![mo2 profiles menu](../assets/images/mo2_sort_loadorder_loop.gif "mo2 load order sorting gif")

        If you want even more details, read [this MO2 guide :simple-github:](https://github.com/sower-j/modding-guides/blob/main/images/mo2-panes.png).

        
    === "Vortex"

        This [video from Nexusmods :fontawesome-brands-youtube:{ .youtube }](https://www.youtube.com/watch?v=ZBE_PcI3qUU) explains how to sort your load order in Vortex. 
        
        We recommend to use the method(s) explained in [this part of the video :fontawesome-brands-youtube:{ .youtube }](https://youtu.be/ZBE_PcI3qUU?si=Z1b-D6Mn4HrBs9YR&t=120). Do not use Vortex' automatic mod sorting feature, it will sort some mods featured in this guide completely wrong and break your game.

        As you might notice in the video (and its comment section), sorting your load order with Vortex is a tedious and annoying process. It's one of the reasons why we don't recommend to use Vortex.

---
--8<-- "docs/mods/loadorder/loadorder-structure.md"


---
## Example Load Order
This load order contains most mods from this guide.
Your load order should look similar.
Make sure to follow the sorting rules from above, and to use the Automatic Load Order checker from below.


???+ abstract "Example Load Order"
    --8<-- "docs/mods/loadorder/loadorder-example.md"
     

---
--8<-- "docs/mods/loadorder/loadorder-checker.md"

---
<small>
:material-information-box:
**Note:** If you sorted your load order, you can move on to the next section.
</small>