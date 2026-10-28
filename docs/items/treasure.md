# Treasure Maps & Dungeon Chests

Kinds of buried, hidden or dropped treasure:

| | Where | Found with |
|---|---|---|
| [Treasure maps](#treasure-maps) | Buried on land | A decoded treasure map and a shovel |
| [Dungeon chests](#dungeon-chests) | Hidden in dungeons | Walking near them |
| [Waterstained chests](#waterstained-chests) | Out at sea | A waterstained map and a boat |
| [Paragon chests](#paragon-chests) | Dropped by paragon monsters | Lockpicking |
| [Rusty chests](#rusty-chests) | Fished up from the sea | A rusty key |

## Treasure maps

### Levels

Treasure maps go from **level 0 to 7**. Each level needs more Cartography to decode and more Lockpicking to dig up.

| Level | Cartography to decode | Lockpicking to dig | Base guardians |
|---|---|---|---|
| 0 (Youth) | — | 5 | 2 |
| 1 | — | 5 | 3 |
| 2 | 41 | 45 | 3 |
| 3 | 51 | 65 | 4 |
| 4 | 61 | 75 | 4 |
| 5 | 70 | 95 | 5 |
| 6 | 70 | 105 | 5 |
| 7 | — | 110 | see [level 7](#level-6-and-7-maps) |

- **Level 0** maps can only be used by young players.
- Level 1–5 maps drop from monsters, bosses, quests and other loot. Level 6 and 7 come from [Carlos](#level-6-and-7-maps).

### Decoding

- Double-click the map to decode it. The skill check runs from (requirement − 10) to (requirement + 30).
- Once decoded, the map shows where the chest is buried.
- Unfinished maps reset to a new location after 30 days.

### Digging

Use a **shovel or pickaxe** on the spot. You need the map's Lockpicking requirement to dig. How close you need to be depends on your **Mining**:

| Mining | Dig radius |
|---|---|
| below 51 | 1 tile |
| 51+ | 2 tiles |
| 81+ | 3 tiles |
| 100+ | 4 tiles |

Digging takes a few seconds and stops if you move or use a skill or spell. The map is used up when the chest comes out.

### Guardians

Digging up the chest spawns **Chest Guardians** from the map's level pool:

```
guardians = base (table above) + Lockpicking / 30      (max 12)
```

You must **kill every guardian** before you can open the chest.

!!! tip "Cartography"
    With **25+ Cartography** you deal **+30% weapon and spell damage** to Chest Guardians.

### The chest

- The chest is **locked** at the map's Lockpicking requirement. Pick the lock, then kill the guardians to open it.
- It isn't trapped.
- The chest disappears after **1 hour**.

#### Loot

| | Amount |
|---|---|
| Gold | **250 × level** (Fortune mastery adds 15 × level × Fortune level) |
| Magic items | **level + 1** items (max 6), stronger at higher levels |
| Spell scrolls | one per level |
| Reagents | 1 to level stacks of 40–60, each with artifact materials |
| Resources | always one stack |
| Rare and special loot | 2.5% per level (+1% per Fortune level); two items at level 4+ |
| Hunter's Luck | each point is a +1% chance for an extra special item |

Other loot, with a chance that grows with the level: enhancement scrolls, mastery orbs, mage items, imbuing materials, rare cloth, bounty scrolls, high-end runic components, Item Bless Deeds, song sheets, orb fragments (level 1–2), pet relics (level 4+) and [PvM runes](ankhs-runes.md#where-runes-drop).
When an Unchained raffle is running, there's also a 5% × level chance for a raffle token.

### Level 6 and 7 maps

**Carlos**, the treasure map trader, turns your extra maps into **level 6** maps and sells the **Codex of Echoes** that leads to a **level 7** chest. See [Level 6 & 7 Treasure Maps](carlos-maps.md).

## Dungeon chests

Dungeons hide **sequence-locked treasure chests**. A chest is invisible until a player comes within **5 tiles**, and it lasts **3 hours**. You need **50 Lockpicking** to work on one.

### 1. Disarm the trap (button sequence)

Use the chest to open its trap panel. A hidden **5-button sequence** has to be pressed in the right order.

- A correct button stays pressed.
- **A wrong button resets the whole sequence** and raises the **Danger Level** by 5–20%. Every 10 Remove Trap above 50 lowers that by 1% (min 5%).
- At **100% danger** the trap **explodes**:
    - you take 25–50 + 10 × trap level damage (trap level 3–5),
    - the trap is gone, but **enraged guardians** spawn (twice as many, up to 8),
    - **70% of the loot is destroyed**.

### 2. Pick the lock

Once the trap is disarmed, use the chest again with **lockpicks** in your backpack.
When you pick the lock, the guardians may wake. The higher your Lockpicking, the lower the chance:

| Lockpicking | Guardian chance |
|---|---|
| 0 | 100% |
| 50 | 75% |
| 75 | 50% |
| 100 | 35% |
| 110 | 25% |
| 120 | 17.5% |

- Guardian count is about 1 + Lockpicking / 20 (up to 6). They get stronger at 40, 80 and 120 Lockpicking.
- They arrive in waves. Kill them all before you can open the chest.

### 3. Loot

Loot scales with three things:

- **Lockpicking + Remove Trap** (out of 240)
- **Hunter's Luck** from all your gear and runes
- **Fortune** mastery (up to ×1.5)

| | Amount |
|---|---|
| Gold | 300 + your Lockpicking + Remove Trap, scaled up (max 5,000) |
| Magic items | 2–6, stronger with more skill and Hunter's Luck |
| Reagents, spell scrolls, resources, gems | a few of each, more with a higher loot scale |
| Resources | better types at 120, 160, 200 and 240 combined skill |
| Special item | chance from Hunter's Luck and skill (max 65%) |

- Bonus rare item (chance from skill and Hunter's Luck, max 50%): a treasure map, rare cloth, a runic component, a spell hue deed, a mage item, a mastery orb, an **artifact weapon**, a resource map or a waterstained map.
- At **200+ combined skill**: an enhancement scroll and an imbuing material every time, plus a raffle token chance during the Unchained raffle.
- [PvM rune](ankhs-runes.md#where-runes-drop): up to 5%.

Opening a dungeon chest also counts for the **Treasure Hunt** [weekly task](../quests/daily-weekly.md#weekly-tasks).

## Waterstained chests

**Waterstained treasure maps** come from fishing (hotspots and fishing resource maps), boss Void Skulls, dungeon bosses and dungeon chests. See [Boats](boats.md#waterstained-treasure-maps) for sailing.

- Maps are **level 1–5**. Double-click one in your backpack to reveal a chest somewhere **at sea**. The chest and the map last **2 hours**.
- When a player gets within **8 tiles**, the chest spawns **guardian waves**: one wave per map level, each wave stronger and smaller than the last (4, 3, 3, 2, then 1 creature).
- Kill every wave, then pick the lock. The chest is also **trapped**.

| Level | Lockpicking |
|---|---|
| 1 | 50 |
| 2 | 80 |
| 3 | 100 |
| 4 | 105 |
| 5 | 110 |

#### Loot

| | Amount |
|---|---|
| Gold | **1,000 × level** (Fortune adds 15 × level × Fortune level) |
| Magic items | **level + 2** items (max 7), stronger at higher levels |
| Resources | 1 to level stacks of 15–35 |
| Reagents | 2–3 + level stacks of 40–60 |
| Orb fragment | always |
| Enhancement scroll | 25% × level |
| Mastery item, mage item | 15% × level each |
| Special loot | 5% × level (+1% per Fortune level), rolled twice: once for special loot, once for a rare fishing net |
| Resource or treasure map | 7.5% × level (+1% per Fortune level) |
| Hunter's Luck | each point is a +1% chance for an extra special item |

Also possible: imbuing materials, high-end runic components, Item Bless Deeds, bounty scrolls, a rare hued item and [PvM runes](ankhs-runes.md#where-runes-drop) (3%, or 6% at level 4+).

Opening a waterstained chest gives Monthly Challenge points, Seafarer score and Treasure Hunter XP, and counts for the Treasure Hunt weekly task.

## Paragon chests

**Paragon** monsters can drop a **paragon chest** on their corpse. Chests are locked and **trapped** (they explode when opened). Pick the lock to fill them with loot.

| Chest | Lockpicking | Dropped by |
|---|---|---|
| **Lesser paragon chest** | 80 | Medium and Hard-tier paragons, and Wrong treasure maps |
| **Paragon chest** | 100 | Elite and Legendary-tier paragons (most of the time) |
| **Greater paragon chest** | 105 | Elite paragons (10%), Legendary paragons (20%) |
| **Legendary paragon chest** | 110 | Greater paragons (sometimes) and Mythic monsters |

A paragon has a **2.5%** chance to drop a chest, more for stronger ones: ×1.25 for Hard tier, ×1.5 for Elite, ×2 for Legendary and stronger. **Greater paragons** can drop any of the four.

### Paragon chest loot

| | Lesser | Regular | Greater | Legendary |
|---|---|---|---|---|
| Gold | 1,250–2,500 | 1,500–3,000 | 2,500–5,000 | 3,500–7,500 |
| Magic items | 3 | 4 | 5 | 6 |
| Magic spellbook | ✅ | ✅ | ✅ | ✅ |
| Resources, reagents | ✅ | ✅ | ✅ | ✅ |
| Enhancement scroll, orb fragment | ✅ | ✅ | ✅ | ✅ |
| Treasure map | 15% (level 1–3) | 25% (2–4) | 25% (3–5) | always (4–5) |
| Special loot | 15% | 25% | always | always |
| Mage item | 25% | 35% | 50% | — |
| Imbuing material | 25% | 50% | 75% | 2, always |
| Mastery item | 25% | 50% | 75% | always |
| [PvM rune](ankhs-runes.md#where-runes-drop) | 5% | 8% | 10% | 15% |
| [Doom armor](../bosses/doom.md#doom-armor-sets) piece | 2.5% | 5% | 7.5% | 10% |
| High-end runic component | 2.5% | 5% | 5% | 7.5% |
| Song sheet | 2.5% | 5% | 6% | — |
| Pet relic | — | — | 1% | 2.5% |
| Item Bless Deed | — | — | 2.5% | 10% |
| Rare-hued dungeon cloth | — | — | — | always |

Magic items and spellbooks are stronger in better chests.

## Rusty chests

**Rusty chests** and **rusty keys** are dredged up from the sea: rare fishing catches, [fishing hotspots](boats.md) and the fisher guildmaster.

- Rusty chests can't be lockpicked. Put the chest in your **backpack**, double-click a **rusty key** and target the chest. The key is used up.
- They're **trapped**, like paragon chests.
- Your **Hunter's Luck** makes their magic items stronger and adds gold.

| | Small rusty chest | Rusty chest |
|---|---|---|
| Gold | 1,250–3,000 | 2,000–4,000 |
| Magic items | 3–4 | 4–5, stronger |
| Magic spellbook, resources, reagents | ✅ | ✅ |
| Enhancement scroll, orb fragment | ✅ | ✅ |
| Treasure map | 20% (level 1–3) | 25% (level 2–5) |
| Special loot | 20% | 25% |
| Mage item | 30% | 42% |
| Imbuing material, mastery item | 37% each | 62% each |
| Cannonball crate | 30% | 40% (including greater and deadly crates) |
| Special fishing net | 25% | 25% |
| Wire | 15% (copper or iron) | 25% (copper, iron, silver or gold) |
| Nautical decoration | 10% | 15% |
| **Mossy armor** piece | 2.5% | 5% |
| [Doom armor](../bosses/doom.md#doom-armor-sets) piece | 3.7% | 6.2% |
| Song sheet, high-end runic component | 3.7% each | 5.5% each |
| Seaweed or Octopus Ink | 1% | 5% |
| **Ancient Fishing Pole** (500–1,000 uses) | 0.3% | 0.5% |
| Pet relic | — | 0.5% |
| Item Bless Deed | — | 1.2% |
