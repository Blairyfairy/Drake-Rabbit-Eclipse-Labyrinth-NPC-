# Balance & Design Notes – Rabbit Labyrinth Fusion

## Design Goals

1. Fair mid-game crafts that feel rewarding without being pay-to-win.
2. Use real obtainable materials from Eclipse (Labyrinth) and Drake (Sunken Ship).
3. Fuse three themes cleanly: Rabbit + Eclipse + Drake/Pirate/Ghost.
4. Give useful but not overpowered bonuses (AGI, LUK, small flee, size-related, etc.).

---

## Suggested Recipes (Default)

### 1. Rabbit Top Hat (Upper)
- 1× Bunny Band (2214)
- 3× Four Leaf Clover
- 50× Feather
- 500,000 zeny  
**Bonus idea:** AGI +4, chance of Increase AGI on being hit (stronger than official Bunny Top Hat)

### 2. Twin Rabbit Headgear (Upper or Mid)
- 2× Bunny Band
- 1× Eclipse Card **or** 5× Four Leaf Clover + 1× Rainbow Carrot
- 1× Cute Ribbon
- 1,500,000 zeny  
**Bonus idea:** LUK +5, FLEE +5, small chance to dodge

### 3. Eclipse Corsair (Upper – Pirate + Rabbit fusion)
- 1× Corsair (Drake drop)
- 1× Eclipse Card **or** equivalent materials (Rainbow Carrot ×3 + Four Leaf Clover ×5)
- 1× Pirate-related item (e.g. any Drake weapon or 1× Amethyst)
- 3,000,000 zeny  
**Bonus idea:** AGI +3, LUK +3, small resistance to Undead / Ghost, or size-related bonus inspired by Drake Card

### 4. Ghost Bunny Band (Upper)
- 1× Bunny Band
- 1× Ghost property item (Fabric, Ghost Bandana, or Ghostring-related)
- 1× Four Leaf Clover
- 2,000,000 zeny  
**Bonus idea:** Ghost property armor or small magic reflect / SP recovery

### 5. Rabbit Lucky Charm (Accessory)
- 2× Four Leaf Clover
- 1× Rainbow Carrot
- 10× Feather
- 300,000 zeny  
**Bonus idea:** LUK +4 or +5% item drop rate (very mild)

---

## Material Sources (Fairness Check)

| Material              | Source                          | Rarity          |
|-----------------------|---------------------------------|-----------------|
| Bunny Band            | Official quest / market         | Common          |
| Four Leaf Clover      | Many maps + Eclipse             | Uncommon        |
| Feather               | Early flying monsters           | Very common     |
| Rainbow Carrot        | Eclipse                         | Uncommon        |
| Cute Ribbon           | Eclipse                         | Uncommon        |
| Eclipse Card          | Eclipse (0.01%)                 | Rare (optional path) |
| Corsair               | Drake MVP                       | Uncommon–Rare   |
| Ghost mats            | Ghostring / Payon dungeon       | Uncommon        |

Players who farm Labyrinth + Sunken Ship can craft everything reasonably.

---

## Rate Scaling Suggestions

| Server Rate     | Zeny Multiplier | Notes                     |
|-----------------|-----------------|---------------------------|
| 1×–5×           | 1.0×            | Keep as written           |
| 10×–50×         | 0.4–0.7×        | Reduce zeny               |
| 100×+           | 0.2× or remove  | Focus on materials only   |

Always keep at least one thematic material (clover / carrot / Corsair) so the Labyrinth & Drake farms stay relevant.

---

## Anti-Abuse

- All crafts use `countitem` + `delitem`.
- Optional daily craft limit can be added via character variable.
- Custom items should be set as tradeable or bound according to your server rules.
