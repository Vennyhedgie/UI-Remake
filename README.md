# UI-Remake

[WIP]

A close to 1 to 1 remake of the skills UI. This is made in an attempt to create a copy of the game's UI that allows for custom positions, while also reducing clutter from buffs that don't really need to be taking up space in the UI during combat. Only Boons and Conditions will be present.

There are similar packs to this one, however this tries to stay consistent with the game's artstyle instead of using ugly or generic visuals like bars for everything. Many of the default UI elements have been recreated or redrawn for higher quality visuals.

# Examples

Examples of the default layout, a copy of the base UI:

<img width="796" height="205" alt="image" src="https://github.com/user-attachments/assets/ce298fe3-f79b-49d6-9740-c17af602354f" />

<img width="801" height="213" alt="image" src="https://github.com/user-attachments/assets/c5a9d5f9-cb21-4274-8002-aeaa92f92aa3" />

<img width="822" height="164" alt="image" src="https://github.com/user-attachments/assets/471f237c-2720-449d-9501-d31a4ad11dce" />

<img width="789" height="235" alt="image" src="https://github.com/user-attachments/assets/7aed450a-a886-407e-aff0-a3821d9bc4b5" />

<img width="777" height="222" alt="image" src="https://github.com/user-attachments/assets/144beb72-accf-4707-b40c-d1fbc123692c" />



Examples of what can be achieved by moving elements around:

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/eca4b5a2-9136-4c8d-b44b-879be7db4d4d" />

<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/172a4442-eb67-4936-be41-86bb35c795c5" />

## Disclaimer

Because this is an overlay, these skills are not actual buttons. They will not be clickable in gameplay nor will they display tooltips. It is recommended you **hide** the skills UI and enable "Use Show ally names key bind" under **Dynamic HUD** in order to have a button you can hold to edit your skills or switch builds.

**This is currently conisdered a BETA release, as some features are currently not replicable with the available Reffect tools. Notably:**
- **Herald Upkeep skills are completely non-functional**. It is not recommended to use this while playing Herald. This is the only one that's currently a hard **unplayable**. **(Needs Reffect update)**
- Parts of the pack will still be visible when in down state or defeated. **(Needs Reffect update)**
- The endurance bar is represented as a separate orb at the moment, as radial wipes are currently not possible, making the radial endurance bar as it is displayed in the game is not possible. **(Needs Reffect update)**
- Similarly, skills on cooldown will not have a radial black reveal, and instead will just be darkened out. However, all other skill state animations are implemented (casting, no resources, charge skills, etc.). **(Needs Reffect update)**
- Ranger pet portraits. There is currently no filter for pet selections, thus portraits are displayed by tracking F2 skill ids. There's a couple of pets that share these skills, so the portrait will be inacurate (Black moa and Ravens for example). Also, only about 40% of the portraits have been added. There's like 100 different pets, still working on adding these but it's tedious, please bear with me!
- The "Guard / Avoid Combat" button is not available.
- In Beastmode, because the pet is not available to check for skills, portratis cannot be displayed. Additionally, Soulbeast's profession UI changes layout when merged / unmerged. This is not possible at the moment and thus will use the merged layout since you're mostly meant to stay in Beastmode. 
- Galeshot's feather generation timer bar is not available. **(Needs Reffect update)**
- Troubadour's instrument duration bar caps at 5 seconds. **(Needs Reffect update)**
- Luminary's shroud duration also caps at 5 seconds. **(Needs Reffect update)**

# How to use

Once the pack is installed, you'll have to select the interface size that matches your current in-game interface size choice:

<img width="312" height="174" alt="image" src="https://github.com/user-attachments/assets/78449a9d-3a96-4963-905f-2ff45d11b56b" />

By default, all the interfaces have the original layout. If you want to customize it, it's recommended you **duplicate** the group (by right-clicking). That way, you can keep the original as a reference while editing.
Most elements are grouped logically in a hierarchy. The big exception that will take the most time editing is the profession UI / Skills, since this one differs from class to class, they had to be unique to each one.
