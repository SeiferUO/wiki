# Treasure Maps & Dungeon Chests

## Treasure maps

### Levels

Treasure maps go from **level 0 to 8**. Each level needs more Cartography to decode and more Lockpicking to dig up.

| Level | Cartography to decode | Lockpicking to dig | Base guardians |
|---|---|---|---|
| 0 (Youth) | — | 5 | 2 |
| 1 | — | 5 | 3 |
| 2 | 41 | 45 | 3 |
| 3 | 51 | 65 | 4 |
| 4 | 61 | 75 | 4 |
| 5 | 70 | 95 | 5 |
| 6 | 70 | 105 | 5 |
| 7 | 110 | 110 | 2 |
| 8 | 120 | 120 | 2 |

### Decoding

- Double-click the map to decode it. The skill check runs from (requirement − 10) to (requirement + 30).
- Once decoded, the map shows where the chest is buried.
- Unfinished maps reset to a new location after 30 days.

### Digging

Use a **shovel or pickaxe** on the spot. How close you need to be depends on your **Mining**:

| Mining | Dig radius |
|---|---|
| below 51 | 1 tile |
| 51+ | 2 tiles |
| 81+ | 3 tiles |
| 100+ | 4 tiles |

Digging takes a few seconds and stops if you move or use a skill or spell.

### Guardians

Digging up the chest spawns **Chest Guardians** from the map's level pool:

```
guardians = base (table above) + Lockpicking / 30      (max 12)
```

Higher Lockpicking gives more guardians **and** better loot.
You must **kill every guardian** before you can open the chest.

!!! tip "Cartography"
    With 25+ Cartography you deal up to **+30% weapon and spell damage** to Chest Guardians (+3% per 10 points).

### The chest

- Chests are **locked** (lock difficulty = the lockpicking requirement) and usually **trapped**. Disarm with Remove Trap before you pick the lock.
- The chest disappears after **1 hour**.

#### Loot

| | Amount |
|---|---|
| Gold | **250 × level** (Fortune mastery adds 15 × level × Fortune level) |
| Magic items | **one per map level**, stronger at higher levels |
| Rare and special loot | chance grows with level (+2.5% per level, +1% per Fortune level) |

Other possible loot includes spell scrolls, mastery orbs, mage items, pet relics, runic components, crafting resources, imbuing materials, rare cloth, reagents, artifact materials and artifact clothing.
When an Unchained raffle is running, there's also a 5% × level chance for a raffle token.

## Sequence trap chests (dungeon chests)

Dungeons spawn **sequence-locked treasure chests**. Each one lasts **3 hours**.

| Chest | Loot focus |
|---|---|
| Wizard's | mage gear |
| Warrior's | weapons and armor |
| Artisan's | crafting rewards |
| Explorer's | exploration rewards |

### 1. Disarm the trap (button sequence)

Use the chest to open its trap panel. A hidden **5-button sequence** has to be pressed in the right order.

- A correct button stays pressed.
- **A wrong button resets the whole sequence** and raises the **Danger Level** by 5–20%. Every 10 Remove Trap above 50 lowers that by 1% (min 5%).
- At **100% danger** the trap **explodes**:
    - you take 25–50 + 10 × trap level damage (trap level 3–5),
    - the chest unlocks, but **enraged guardians** spawn,
    - much of the loot is **destroyed**.

### 2. Pick the lock

You need at least **50 Lockpicking** (and the trap must be disarmed first).

Each attempt has a chance to wake **guardians**. Higher Lockpicking means less chance:

| Lockpicking | Guardian chance |
|---|---|
| 0 | 100% |
| 50 | 75% |
| 75 | 50% |
| 100 | 35% |
| 110 | 25% |
| 120 | 17.5% |

Guardian count and strength grow with your Lockpicking. They arrive in waves. Kill them all before you can open the chest.

### 3. Loot

Loot quality scales with **Lockpicking + Remove Trap** (out of 240), your **Luck** and **Hunter's Luck**.

Opening a dungeon chest also counts for the **Treasure Hunt** [weekly task](../quests/daily-weekly.md#weekly-tasks).
