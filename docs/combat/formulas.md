# Combat Formulas

How hit chance, melee damage and spell interruption are calculated.

!!! note
    Numbers marked *default* come from in-game balance controllers and can be changed by staff.

## Hit chance

```
chance = (attack skill + 50) / ((defense skill + 50) × 2)
chance × (1 + Hit Chance Increase %)
```

- **Attack skill** is your weapon's skill (Swords, Macing, Fencing, Archery, Wrestling…).
  The Battle Lute uses **Musicianship**.
- **Defense skill** is the defender's weapon skill the same way.
- **Bards:** if you have at least two of Musicianship, Peacemaking, Provocation and Discordance at 10+,
  the average of those skills (max 100) is used instead whenever it is higher.
- **Hit Chance Increase counts double against monsters.**
- PvM runes: *Hit Chance* raises your chance against monsters; *Evasion* lowers the chance to be hit (outside PvP).
- Monsters use Wrestling when it is higher than their weapon skill, and stronger monsters get a flat accuracy bonus.
  Legendary monsters gain +5% accuracy per nearby attacker.

## Melee damage

Base damage is the weapon's damage roll. Two-handed weapons in PvM roll toward the high end of their range.
The bonuses below are then added together and applied to the roll.

| Source | Bonus |
|---|---|
| **Tactics** | 0 = −50%, 50 = no change, 100 = +50%, 120 = +70%. Counts as 100 max in PvP. |
| **Anatomy** | +1% per 5 points, plus +10% at 100 or more (120 Anatomy = +34%) |
| **Strength** | +1% per 5 Strength |
| **Lumberjacking** (axes) | +1% per 5 points, max +20% (half for one-handed axes) |
| **Mining** (bashing weapons) | +1% per 5 points, max +20% (half for one-handed) |
| **Fletching** (ranged weapons) | +1% per 5 points, max +20% (half for one-handed) |
| **Begging** (slashing weapons) | +1% per 5 points, max +20% |
| **Weapon quality** | Mastercrafted +30%, Exceptional +20%, Superior +10%, Low −10%, Decrepit −20%, Ruined −30% (max +20% in PvP) |

Damage is then **halved when the target is a player**, and creature damage is always halved.

### Battle Lute

The [Battle Lute](../bard/battle-lute.md) replaces the skill bonuses:
Provocation works like Tactics, Discordance like Anatomy and Peacemaking like Strength, plus quality.
In PvP each bard skill counts as 100 max.

## Spell interruption (fizzle protection)

When you take damage while casting, three separate rolls can save your spell.
The spell is only interrupted if **all three fail**.

| Roll | Formula | Max |
|---|---|---|
| **Protection** spell | (Evaluating Intelligence + Meditation + Inscription) / 4, Inscription counts as 120 max (100 in PvP) | 75% |
| **Focus** (PvM only) | Focus × 0.6 + Aero mastery (5–20% *default*) + item Focus (armor + clothing + runes, max 50% *default*) | 75% |
| **Casting Focus** | Casting Focus item property + fish pie (max 12%) + Inscription / 20 | 18% |

Best possible protection:

- **PvM:** about **95%**
- **PvP:** about **80%** (no Focus roll)

Always uninterruptible: **wands**, and **first-circle Magery on Felucca**.
