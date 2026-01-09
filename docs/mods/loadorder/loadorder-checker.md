## Automatic Load Order Checker

The Automatic Load Order Checker can detect if you

* use mods that are incompatible with FROST
* use mods that are outdated or broken
* forgot to install a required mod from this guide
* sorted your mods correctly

Copy and paste the content of your **loadorder.txt** into this text field, and press the button.
Make sure that you copy all the content of your load order into the text field.

!!! tip
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

--8<-- "docs/javascripts/loadorder-checker.js"

</script>
