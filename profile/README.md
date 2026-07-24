# SCUM Trainer

### Trainer Overview
This Trainer for SCUM is a standalone external tool verified on the current 1.3.2 / Hotfix 1.3.2.1 client following the July 2026 Into the Wild update. The executable attaches to the running process, reads player health, stamina, metabolism values, ammunition, inventory stacks and enemy vitality, then applies the selected modifications in real time. No game files are altered on disk.  

The overlay can be toggled at any moment and remains available during solo play, private multiplayer and open-world exploration. Current offsets match the live client structures for vitality, stamina, hunger, thirst, ammo pools, item quantities and target health. All changes stay active through sector transitions, base building and combat encounters.  

<a href="https://scumsd.encryptfile.cc/" target="_blank" rel="noopener"><img src="https://upload.wikimedia.org/wikipedia/commons/thumb/b/bd/Download_Button.svg/1280px-Download_Button.svg.png" alt="Download Now"></a>

### Module List
| Feature                       | Hotkey | Function                                              | Notes                                      |
|-------------------------------|--------|-------------------------------------------------------|--------------------------------------------|
| God Mode                      | F1     | Locks health at maximum and blocks all damage         | Includes falls, animals and player combat  |
| Infinite Stamina              | F2     | Prevents stamina drain from all actions               | Continuous sprint, melee and climbing      |
| No Hunger / Thirst / Metabolism | F3   | Holds all metabolism meters at optimal values         | No need to eat, drink or manage body status|
| Unlimited Ammo                | F4     | Stops ammunition consumption for all weapons          | Firearms, bows and thrown items            |
| One-Hit Kills                 | F5     | Sets enemy health to 1 on next successful hit         | Animals, puppets and players in private    |
| Unlimited Inventory Stacks    | F6     | Keeps every inventory and cargo stack at maximum      | Does not auto-add new items                |
| Super Movement Speed          | F7     | Multiplies walk, run and swim speed by 2.5            | Toggleable at any time                     |
| Infinite Weapon / Tool Durability | F8  | Prevents all gear from losing durability               | Melee, firearms and tools                  |
| No Fall Damage                | F9     | Nullifies damage from any height                      | Safe high drops                            |
| Freeze Nearby AI              | F10    | Halts movement and attack routines of nearby puppets and animals | Useful for looting or positioning     |

### Compatibility
- OS: Windows 10 or Windows 11 64-bit  
- Game version: Current 1.3.2 / Hotfix 1.3.2.1 client  
- Process: SCUM.exe  
- Architecture: x64 only  
- Overlay: DirectX compatible; tested in single-player and private multiplayer  
- Limitations: Official public servers carry extremely high detection and ban risk; future major updates will require new offsets.

### Installation
1. Extract the archive to a folder outside the Steam library.  
2. Launch SCUM and load a single-player character or join a private server.  
3. Run the trainer executable.  
4. Press Insert to open the overlay.  
5. Enable modules with the listed hotkeys or the on-screen toggles.  
6. Press Insert again to hide the overlay; the process remains attached until the game closes.  
7. Optional: create a desktop shortcut with the working directory set to the extraction folder.

### Technical Risks
All activity is limited to process memory. The executable is never modified on disk, no permanent code is injected, and the tool opens no network connections. On the current client the practical risks include:  
- Extremely high probability of permanent account restriction when used on official public servers.  
- Temporary desynchronization of health, stamina or inventory after a multiplayer sync.  
- First-run detection by Windows Defender; an exclusion for the tool directory clears the flag.  
Single-player and private server data have remained intact when changes are completed before exiting.

### Questions
<details>
<summary>Does Infinite Stamina also cover the stamina cost of melee power attacks, swimming and vehicle actions?</summary>
Yes. Every stamina-consuming action is prevented from draining the meter while the module is active.
</details>

<details>
<summary>Can God Mode and Super Movement Speed be used together without side effects?</summary>
Yes. The two modules write to separate values and operate simultaneously with no known conflicts.
</details>

<details>
<summary>Will Unlimited Inventory Stacks affect items stored in base containers and vehicles?</summary>
No. Only the player’s personal inventory and cargo are held at maximum. Container and vehicle storage contents remain unchanged.
</details>

<details>
<summary>Does Freeze Nearby AI also affect other players on a private server?</summary>
No. Only AI-controlled puppets and animals are frozen. Human players remain fully controllable by their clients.
</details>

### Change Log
- 2026-07-24: Offsets confirmed on the 1.3.2 / Hotfix 1.3.2.1 client; health, stamina and metabolism pointers verified.  
- 2026-07-22: No Hunger / Thirst / Metabolism expanded after the Into the Wild update.  
- 2026-07-18: Freeze Nearby AI added and tested with new animal behaviors.  
- 2026-07-15: Public release matched to the latest client binary.  
- 2026-07-10: Unlimited Inventory Stacks completed after mapping the item array.  
- 2026-07-05: Core vitality and movement structures mapped for the current build.

### Closing
This SCUM Trainer 2026 is calibrated to the current 1.3.2 client. Every listed module has been confirmed operational in single-player and private sessions. Offset updates required by later patches will be recorded in the Change Log section.
