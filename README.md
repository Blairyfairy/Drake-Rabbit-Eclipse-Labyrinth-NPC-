# Rabbit Labyrinth Fusion NPC

**Custom rAthena / Hercules NPC pack** for Ragnarok Online private servers.

A mysterious fusion craftsman hidden deep inside the **Labyrinth Forest** (`prt_maze03`).  
He weaves together **rabbit** essence (Eclipse mini-boss, Bunny Band, Four Leaf Clover, Rainbow Carrot…), **Drake / ghost-property** power, and **pirate** relics into exclusive rabbit-themed gear:

- **Rabbit Top Hat** (enhanced Bunny Top Hat style)
- **Twin Rabbit Headgear**
- **Eclipse Corsair** (rabbit + pirate fusion hat)
- **Ghost Bunny Band**
- Smaller rabbit accessories and costume pieces

Fair trade-offs using rabbit / Eclipse materials, Drake-related items, and pirate drops.

---

## Theme Fusion

| Theme          | Source                          | Used For                          |
|----------------|---------------------------------|-----------------------------------|
| Rabbit         | Eclipse mini-boss, Lunatics, Bunny Band quest materials | Core rabbit gear & luck bonuses  |
| Eclipse        | Mini-boss in Labyrinth Forest   | Special “Eclipse” worded trades & card |
| Drake / Ghost  | Drake MVP (Sunken Ship), Ghost property items | Ghost-infused rabbit gear, size-ignore style bonuses |
| Pirate         | Corsair hat, Drake drops, Sunken Ship relics | Pirate-rabbit hybrid headgears   |

The NPC stands at the crossroads of the Labyrinth, offering fusion crafts that feel thematic and balanced.

---

## Features

- Multiple crafting / fusion menus
- Reasonably fair material costs (no extreme rarity gates)
- Uses real Ant Hell–style “hard but obtainable” drops from Eclipse + Drake
- Exclusive custom headgears with useful mid-game bonuses
- Optional set bonuses when wearing multiple rabbit pieces
- Fully documented installation & balance notes

---

## Quick Start

1. Copy `npc/rabbit_labyrinth_fusion.txt` into your `npc/custom/` folder.
2. Merge the item definitions from `/db`.
3. Place the NPC inside Labyrinth Forest (`prt_maze03`).
4. `@reloadscript` and test.

Full guide → [docs/INSTALLATION.md](docs/INSTALLATION.md)

---

## Folder Structure

```
rabbit-labyrinth-npc/
├── README.md
├── LICENSE
├── docs/
│   ├── INSTALLATION.md
│   ├── BALANCE.md
│   ├── QUEST_FLOW.md
│   └── CUSTOM_ITEMS.md
├── npc/
│   └── rabbit_labyrinth_fusion.txt
├── db/
│   ├── item_db_rabbit.yml
│   └── item_db_rabbit.txt
├── items/
│   └── item_info_rabbit.lua
└── scripts/
    └── rabbit_set_bonus.txt
```

---

## Recommended Location

**Labyrinth Forest – Floor 3** (`prt_maze03`)

Suggested coordinates (adjust to your map):
```
prt_maze03,170,170,4
```
(near Eclipse’s usual spawn area so the theme feels natural)

Sprite suggestions:
- `4_F_RABBIT` / custom rabbit-eared NPC
- `4_M_SAGE_C` with rabbit ears
- Any mysterious / alchemist / pirate-rabbit hybrid look

---

## Core Crafts (Examples)

| Result                     | Main Materials                                      | Zeny     |
|----------------------------|-----------------------------------------------------|----------|
| Rabbit Top Hat             | Bunny Band + 3× Four Leaf Clover + Feather x50     | 500k    |
| Twin Rabbit Headgear       | 2× Bunny Band + Eclipse Card (or materials)         | 1.5M    |
| Eclipse Corsair            | Corsair + Eclipse materials + Drake-related item    | 3M      |
| Ghost Bunny Band           | Bunny Band + Ghost property item / Ghostring mat   | 2M      |
| Full Rabbit Set Bonus      | Wear 3+ rabbit pieces                               | —       |

Exact recipes are configurable and documented in `/docs/BALANCE.md`.

---

## Requirements

- rAthena or Hercules
- Editable item database
- Basic knowledge of custom NPCs & headgear sprites (optional)

---

## Credits

- Inspired by official Bunny Band / Bunny Top Hat, Eclipse mini-boss, Drake the Pirate MVP, and the Labyrinth Forest.
- Designed for fair mid-game progression and fun thematic fusion.

**Hop into the Labyrinth and craft your legend!** 🐰🎩👻🏴‍☠️
