# Installation Guide – Rabbit Labyrinth Fusion NPC

## 1. Copy Files

```bash
cp npc/rabbit_labyrinth_fusion.txt   /path/to/server/npc/custom/
cp db/item_db_rabbit.yml             /path/to/server/db/re/   # or pre-re
# OR
cp db/item_db_rabbit.txt             /path/to/server/db/
cp items/item_info_rabbit.lua        /path/to/client/System/  # optional
```

## 2. Register the NPC

In `npc/scripts_custom.conf` (or equivalent):

```conf
npc: npc/custom/rabbit_labyrinth_fusion.txt
```

Optional set-bonus script:

```conf
npc: npc/custom/../scripts/rabbit_set_bonus.txt
```

## 3. Add Custom Items

Merge the YAML (preferred) or .txt entries into your item database.  
New item IDs used (change if they conflict):

| ID    | Name                  |
|-------|-----------------------|
| 19600 | Rabbit Top Hat        |
| 19601 | Twin Rabbit Headgear  |
| 19602 | Eclipse Corsair       |
| 19603 | Ghost Bunny Band      |
| 19604 | Rabbit Lucky Charm    |

## 4. Place the NPC

Edit the first line of the script:

```
prt_maze03,170,170,4	script	Labyrinth Fusionist	4_F_RABBIT,{
```

Recommended map: **prt_maze03** (Labyrinth Forest F3 – Eclipse’s home).

Alternative nearby maps if you prefer outside the maze:
- `prt_fild02`
- `prt_maze01` / `prt_maze02`

## 5. Client Side (optional)

Add the descriptions from `items/item_info_rabbit.lua` to your itemInfo file and update GRF / patch clients so the new headgears display correctly.

## 6. Test

1. `@reloadscript`
2. Warp to `prt_maze03 170 170`
3. Talk to the NPC and try a simple craft (e.g. Rabbit Top Hat).

## Troubleshooting

| Issue                     | Fix                                      |
|---------------------------|------------------------------------------|
| NPC missing               | Check coordinates + reloadscript         |
| Unknown item              | Confirm item IDs loaded in item_db       |
| Client shows “Unknown”    | Update itemInfo.lua + client patch       |
| Wrong material IDs        | Verify Four Leaf Clover, Corsair, etc.   |

## Uninstall

Remove the NPC line from scripts_custom.conf and delete/comment the custom items.
