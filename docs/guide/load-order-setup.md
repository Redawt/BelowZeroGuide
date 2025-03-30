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
Some plugins depend on other plugins, or need to overwrite changes from other plugins (="winning conflicts").
That is why sorting your load order is important, otherwise features from mods will break, or you will encounter issues like crashes, fps issues and bugs. 

This section provides information on how to sort your load order regarding FROST and the mods featured in this guide, but also for mods which are not featured in this guide. We do not recommend to use LOOT or any other automatic load order sorting tool, as they tend to sort mods wrong (especially FROST mods).

!!! info "Mods without plugins"
    Not all mods have an esm/esp/esl plugin. Certain mods that are part of the guide, like Buffout 4, don't have a plugin.

---
## How to sort your mods in your mod manager
The scope of the guide does not include detailed instructions about how to use your mod manager.
There are other resources online for that.
This is only a rough overview.
If you are already familiar with how to do this, skip this subsection.

??? abstract "Expand me if you need to know more." 


    === "MO2"

        ![MO2 Panes](/assets/images/mo2-panes.png)
        If you want more details, read [this MO2 guide :simple-github:](https://github.com/sower-j/modding-guides/blob/main/images/mo2-panes.png)

        <div class="grid cards" markdown>

        -   :material-dock-right:{ .lg .middle } __Left Pane__

            ---

            The left pane contains the mods and mod separators you've installed.

            Sort the separators and the mods inside them in the same order as they have been featured in this guide.

            To sort them, you can simply drag & drop the mods and separators around.

        -   :material-dock-left:{ .lg .middle } __Right Pane__

            ---
            
            The right pane has a "plugins" section. It contains the esm/esp/esl plugins from the mods from this guide.

            They reflect the content of your `loadorder.txt` and `plugins.txt` files, which tell the game how to load your plugins.

            To sort them, you can simply drag&drop the plugins around in the list.

        </div>


        
    === "Vortex"
        
        I am not using Vortex, and I don't recommend using it. 
        If you followed this guide and decided to use Vortex, and don't know how to sort your load order in it, you should have decided to use MO2 instead (bummer).

        I can not offer you much help. There are videos like [this  video from Gopher :fontawesome-brands-youtube:{ .youtube }](https://www.youtube.com/watch?v=BRo8I32ASSw) that talk about the topic, and the [**Nexusmods Discord :simple-discord:**](https://discord.gg/nexusmods) where you might be able to find additional help and resources.

---
--8<-- "docs/mods/loadorder/loadorder-structure.md"


---
## Example Load Order
This load order contains most mods from this guide.
Your load order should look similar.
Make sure to follow the sorting rules from above, and to use the Automatic Load Order checker from below.

??? abstract "Expand me if you want to see the example load order" 
    --8<-- "docs/mods/loadorder/loadorder-example.md"

---
--8<-- "docs/mods/loadorder/loadorder-checker.md"

---
<small>
:material-information-box:
**Note:** If you sorted your load order, you can move on to the next section.
</small>