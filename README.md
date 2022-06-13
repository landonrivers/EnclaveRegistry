# EnclaveRegistry
Registry Files for Enclave PC (2003) - Different branches allow for modding in different ways

## How to use this repo?

Clone this repo to your `registry` folder in your Enclave/Sbz1 directory. Do git checkout on one of the branches in order to swap the way your registry is configured. Every time you make a change to the registry, you must restart enclave.exe to see these changes.

The Master branch has no changes made to it. There is a separate `vanilla` branch as well which also has no changes. It is not advised to merge any of the branches to your master branch.

! ! ! Please keep in mind, when you make a save file, the save file will 
  1. use whatever registry you currently have active, and 
  2. cache that registry.  

You cannot change back a save file once its registry has been affected.

## Encoding:
For **Notepad++**, use **ANSI encoding**  
For **Visual Studio Code**, use **Western (Windows 1252)** encoding.  
The `StringTable` files may work better with UTF-16-LE encoding in some cases. Honestly I haven't gotten a handle on it yet.

**Failure to do so** will potentially overwrite the unicode block character %xA7 (varchar) with a section character (§), and will result in a strange characters showing in game. This will be apparent when you go to commit a change and it shows you as having changed the unicode character.

## Branches (Configurations):  

### 1. newcharacters

This is the branch which has been shared as a standalone mod on the steam guide and in the youtube video description.
**What This Does:**
- This mod creates two entirely new characters, Zale and Mordessa for the player to use. This does not replace any current characters. This also adds in Mordessa's Staff and Zale's Staff of the Earth Spirit for purchase in the store. This also gives access for the Druid, Wizard, Lich, and Sorceress to use these new weapons as well!
- This also gets rid of the line `special:quittomenu` which triggers when beating either of the campaigns. This allows the new staves to be used by the Druid, Wizard, Lich, and Sorceress specifically when the game is beaten through making the ending cutscene the 'challenge' to complete. `special:quittomenu` prevented the cutscene from properly completing, and also didn't allow 'Light Final' or 'Dark Final' to show on the map.

**How to Unlock Zale and Mordessa:**
- Unlock Zale by completing the Light campaign. This also unlocks the Staff of the Earth Spirit (Cost 5000) and gives this weapon to the Druid and Wizard as well.
- Unlock Mordessa by completing the Dark campaign. This also unlocks Mordessa's Staff (Cost 4000) and gives this weapon to the Lich and Sorceress as well.

**Notes:**
- Zale and Mordessa are not entirely overpowered. They share the same HP as a regular character, though they have heightened weapon abilities.
- The Staff of the Earth Spirit and Mordessa's Staff are unchanged from how they were originally entered in the registry. Mordessa's Staff is weaker, therefore it has the lower price.

### 2. weapons-for-all

**What This Does:**
- This mod adds every default character (no Zale or Mordessa) to every level in each campaign. Furthermore, it alters the inventory of every character so they are able to equip every item from the start.
- The starting levels for Light and Dark now allow you to choose your character and weapons.
- There are some oddities that come with this, for instance the Sorceress does not have a proper reload animation for the crossbow.

### 3. vanilla

**What This Does:**
- This is simply a clean version of the registry as it comes from Steam. No changes made to it.
