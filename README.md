[WIP]

# NOTE

The setting to **reuse game icons is required** for this pack to function:

<img width="364" height="145" alt="image" src="https://github.com/user-attachments/assets/babef52d-c5ab-40d3-9881-925959b32d0e" />

# UI-Remake


A close to 1 to 1 remake of the skills UI. This is made in an attempt to create a copy of the game's UI that allows for custom positions, while also reducing clutter from buffs that don't really need to be taking up space in the UI during combat. Only Boons and Conditions will be present.

There are similar packs to this one, however this tries to stay consistent with the game's artstyle instead of using ugly or generic visuals like bars for everything. Many of the default UI elements have been recreated or redrawn for higher quality visuals.

# Examples

Examples of the default layout, a copy of the base UI:

<img width="796" height="205" alt="image" src="https://github.com/user-attachments/assets/ce298fe3-f79b-49d6-9740-c17af602354f" />

<img width="801" height="213" alt="image" src="https://github.com/user-attachments/assets/c5a9d5f9-cb21-4274-8002-aeaa92f92aa3" />

<img width="822" height="164" alt="image" src="https://github.com/user-attachments/assets/471f237c-2720-449d-9501-d31a4ad11dce" />

<img width="789" height="235" alt="image" src="https://github.com/user-attachments/assets/7aed450a-a886-407e-aff0-a3821d9bc4b5" />

<img width="777" height="222" alt="image" src="https://github.com/user-attachments/assets/144beb72-accf-4707-b40c-d1fbc123692c" />


# Custom Layouts

Examples of what can be achieved by moving elements around, potentially improving **controller support**:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/eca4b5a2-9136-4c8d-b44b-879be7db4d4d" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/172a4442-eb67-4936-be41-86bb35c795c5" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/9d095402-ee93-476c-9790-80f1103acd6b" />


## Disclaimer

Because this is an overlay, these skills are not actual buttons. They will not be clickable in gameplay nor will they display tooltips. It is recommended you **hide** the skills UI and enable "Use Show ally names key bind" under **Dynamic HUD** in order to have a button you can hold to edit your skills or switch builds.

**This is currently conisdered a BETA release, as some features are currently not replicable with the available Reffect tools. Notably:**
- **Herald Upkeep energy pips are completely non-functional**. It is not recommended to use this pack while playing Herald. Other Revenant specs are OK. This is the only one that's currently a hard **unplayable**. **(Needs Reffect update)**
- The endurance bar is represented as a separate orb at the moment, as radial wipes are currently not possible, making the radial endurance bar as it is displayed in the game is not possible. **(Needs Reffect update)**
- Similarly, skills on cooldown will not have a radial black reveal, and instead will just be darkened out. However, all other skill state animations are implemented (casting, no resources, charge skills, etc.). **(Needs Reffect update)**

### Ranger Issues

The ranger UI is particularly intricate and due to Reffect missing active pet filters, so some compromises have been made. Pet F2 skill IDs are used to check your active pet to display portraits. Because of this, whenever the F2 skill is modified, these pet checks cannot be performed. However, most of those issues have been circumvented somehow, so I would still consider it **playable just fine**. These issues are:

- There's a couple of pets that share the same F2 skills, so the portrait will be the same (Mostly Hall of Monument pets).
- The "Guard / Avoid Combat" button is not available. This also applies to Mechanist. (You can still use F3 to recall your pet or toggle your default UI visibility to click this button).
- In Beastmode, because the pet is not available to check for skills, portratis cannot be displayed. Additionally, Soulbeast's profession UI changes layout when merged / unmerged. This is not possible at the moment and thus Soulbeast will use the merged layout since you're mostly meant to stay in Beastmode.
- On Untamed, when your pet is unleashed, it also cannot check skills. However, a glowing Unleashed Pet portrait will replace your pet's portrait when active, improving Unleashed state readability.
<img width="762" height="217" alt="image" src="https://github.com/user-attachments/assets/9eb9b727-08c2-4273-a66d-be6c635e9a72" />
<img width="823" height="244" alt="image" src="https://github.com/user-attachments/assets/108f16f6-3748-4935-8c0c-614d480d4451" />

- Galeshot's feather generation timer bar is not available. **(Needs Reffect update)**
  
### Other minor issues
- Troubadour's instrument duration bar caps at 5 seconds. **(Needs Reffect update)**
- Luminary's shroud duration also caps at 5 seconds. **(Needs Reffect update)**

# How to use

Download "Venny Clean UI.zip" into your reffect root folder and extract. It should add the necessary files to the icons and packs subfolders. An additional Settings file is provided for style that's also recommended to download. More details below.

<img width="602" height="108" alt="image" src="https://github.com/user-attachments/assets/425ed5c1-993e-4219-b88b-19a325fd6d55" />

If you have GW2 open, restart it to let Reffect reloadd the pack.

Once the pack is installed, you'll have to **set the interface size that matches your current in-game interface size choice by Right clicking "Interface Normal" > Resize**:

<img width="640" height="275" alt="image" src="https://github.com/user-attachments/assets/94487424-91f8-4341-8d01-68e51d88080c" />
<img width="859" height="88" alt="image" src="https://github.com/user-attachments/assets/0b0dfe85-6ddc-4216-ac14-31a44af21a75" />

As listed, the sizes you should use are:

- Small: 90%
- Normal: 100% (Default, don't resize)
- Large: 110%
- Larger: 120%


By default, all the interfaces have the original layout. If you want to customize it, it's recommended you **duplicate** the group (by right-clicking). That way, you can keep the original as a reference while editing.
Most elements are grouped logically in a hierarchy. 

Weapon and utility hotbars are shared. Same for health and endurance orbs. The element that will take the most time customizing will be the profession UI / Skills section, since this one differs from class to class. 

Navigate the hierarchy to find the element or group you wanna move and place it wherever you want it to display. Reminder that positions are inherited, so if you move a parent, all children will move with it, keeping their own positions as offsets.

# Settings

A settings file is provided to style buffs to look as close to ingame as possible, with pretty stack markers and white duration bars instead of the default neon green. This is optional but highly recommended. It's only separate for users who may have customized their settings for other packs already.

<img width="123" height="55" alt="image" src="https://github.com/user-attachments/assets/9d546406-b656-45fd-9723-4d0209d8a5ee" />
