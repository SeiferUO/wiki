# Scavenging (Begging)

On this shard Begging is **Scavenging**: carving monster corpses finds extra loot.

## How it works

1. Use the skill to open the Scavenging window and pick what to look for. You need at least **3 options** and can pick up to 6.
2. **Carve** a monster corpse. Each carve makes one scavenging attempt.

### Success chance

| Creature tier | Difficulty |
|---|---|
| Below Easy | 29.1 |
| Easy | 40 |
| Medium | 50 |
| Hard | 60 |
| Elite | 75 |
| Legendary | 80 |
| Abomination | 100 |
| Mini-boss | 105 |
| Expeditions, Dungeon boss | 110 |
| Champion | 115 |
| Harrower | 120 |

```
difficulty = tier difficulty − 10 − (Begging − 100) / 2
chance = (Begging − difficulty + 25) / 50
```

**At 120 Begging every attempt succeeds.**

### How much you get

- One item from a random enabled basic option.
- **+1 extra item** from Abomination-tier monsters, **+2** from Mini-bosses and stronger.
- High-skill options each give their own extra roll.

## Options

| Option | Needs | What you get |
|---|---|---|
| Gold | — | max HP / 30 × (1 + 2.5% per 10 Begging), 5–150 gold. Champion minions give less |
| Gems | — | one random gem |
| Bandages | — | 5–10 bandages |
| Potions | — | a random potion. Greater versions at 100+ Begging against Medium-tier and stronger |
| Reagents | — | 5–50 magery or necro reagents, based on monster HP |
| Scrolls | — | an attack scroll. Stronger monsters drop higher circles (Flame Strike from Champions) |
| Petals | 100 | petals, or 5% chance for garden seeds |
| Food | 100 | food |
| Resources | 100 | crafting resources by skill |
| Enchanting | 105 | imbuing materials |
| Special items | 110 | special items |
| Quest items | 115 | quest items |

!!! tip "Scavenger satchel"
    With a Scavenger satchel equipped and 100+ Begging, scavenged items go straight into the satchel.

Begging also adds **+1% damage per 5 points with slashing weapons** (max +20%). See [Combat Formulas](../combat/formulas.md#melee-damage).
