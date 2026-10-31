# Chivalry

Chivalry is a custom PvM support school. It runs on **Virtue Marks** instead of mana or tithing.

!!! warning "PvM only"
    Chivalry spells can't be cast in PvP. Out of combat with players, the Chivalry skill still gives
    **+1% weapon damage against players per 10 points** (max +10%). See [Weapons](../core/weapons.md#chivalry-in-pvp).

## Virtue Marks

Every spell costs Virtue Marks. Mana is never used.

- You start earning marks once you carry a **Paladin Tome** or have **100 base Chivalry**.
- You can hold **100 marks** (+10 per *Virtue Capacity* tier).
- Spells are **never interrupted** by damage.

### Earning marks

| Action | Chance | Amount |
|---|---|---|
| **Hitting a monster** with a weapon | 35% + Chivalry/20 % + Focus/20 % (max 95%) | 1, or 1–2 vs Hard+, 1–3 vs Legendary+ |
| **Killing a monster** | 10% (New/Easy), 25% Medium, 35% Hard, 50% Elite, 100% Legendary+ | same as above |
| **Parrying** with a shield | half the hit chance | 1 |

- Fists and mage staves don't earn marks.
- Each *Virtue Abundance* tier adds +1 per gain. The **Paladin Cloak** artifact adds +1.
- **Virtue Mark Bonus** runes raise the chance (max +50%).
- **Virtue Mark Efficiency** runes give a chance for a spell to cost nothing (max 50%).

Hitting monsters with a weapon is also how Chivalry skill gains happen.

## Power value

Healing spells scale with your Karma and Chivalry:

```
power = √(Karma + 20,000 + Chivalry × 100)
```

At 15,000 Karma and 100 Chivalry, power is about **212**.

## Spells

| Spell | Skill | Marks | Cast | Effect |
|---|---|---|---|---|
| [Close Wounds](#close-wounds) | 0 | 5 | 1.5 s | Heal |
| [Cleanse by Fire](#cleanse-by-fire) | 5 | 5 | 1.0 s | Cure poison |
| [Remove Curse](#remove-curse) | 5 | 15 | 1.5 s | Remove debuffs |
| [Vigor](#vigor) | 10 | 15 | 1.0 s | Stamina-loss immunity |
| [Exalted Sacrifice](#exalted-sacrifice) | 15 | 20 | 1.5 s | Big heal, costs HP |
| [Sacred Journey](#sacred-journey) | 15 | 25 | 1.5 s | Recall |
| [Karma Reflection](#karma-reflection) | 20 | 20 | 1.0 s | Magic reflect |
| [Divine Fury](#divine-fury) | 25 | 20 | 1.0 s | Swing speed buff |
| [Dispel Evil](#dispel-evil) | 35 | 25 | 1.0 s | Damage reduction |
| [Consecrate Weapon](#consecrate-weapon) | 45 | 25 | 1.0 s | Hit chance buff |
| [Enemy of One](#enemy-of-one) | 55 | 30 | 1.5 s | Damage vs one creature type |
| [Holy Light](#holy-light) | 55 | 25 | 1.5 s | Blind monsters |
| [Noble Sacrifice](#noble-sacrifice) | 65 | 30 | 2.0 s | Group heal and resurrect |

You can't cast on criminals, murderers or monsters (except where noted). 100% success comes at required skill + 50.

### Close Wounds

Heals a target within 2 tiles for **power / 6 + 0–2** (min 7, max 39). Doesn't work if the target is poisoned or mortally wounded.

### Cleanse by Fire

Cures the target's poison. You take fire damage equal to **10% of your max HP** (min 5).

### Remove Curse

Removes stat curses, negative buffs and poison from a target within 12 tiles.

### Vigor

You don't lose stamina for **5 + Chivalry / 5 seconds**.

### Exalted Sacrifice

Heals another player or pet within 12 tiles for **power / 5 + 10–25**. You lose 70% of the amount healed. You need more than 20% HP to cast it.

### Sacred Journey

Recall with a rune, runebook, boat key or house. The usual [travel rules](../core/spellcasting.md#travel) apply.

### Karma Reflection

A magic reflect that absorbs **circles equal to your Chivalry skill** (100 circles at 100). See [Magic Reflection](../core/spellcasting.md#magic-reflection).

### Divine Fury

| | Value |
|---|---|
| Swing speed | **+5% + Chivalry / 10 %** (+15% at 100) |
| Damage taken from monsters | **+40% − Chivalry / 6.5 %** (about +25% at 100, never below 0) |
| Duration | 10 + Chivalry / 5 seconds |

### Dispel Evil

You take less damage from monsters: **5% + 0.15% per Chivalry point** (20% at 100, 23% at 120).
This counts toward the 50% cap on [defenses against monsters](../core/creatures.md#your-defenses-against-monsters).
Duration: 10 + Chivalry / 7 seconds.

### Consecrate Weapon

Your PvM hit chance goes up by **5% + Chivalry / 10 %** (15% at 100) for 10 + Chivalry / 5 seconds.
You need a weapon in hand. This counts toward the [75% PvM accuracy cap](../core/weapons.md#player-attacking-a-monster-pvm).

### Enemy of One

The **first monster you hit** sets your enemy type (undead, daemon, dragon, spider, elemental, giant, vermin or humanoid).

- **+15% damage** against that type.
- **+100% damage taken** from every other type.

Duration: 10 + Chivalry / 5 seconds. Best used when a fight is all one kind of monster.

### Holy Light

Blinds every monster within 3 tiles of the target spot for **3 + Chivalry / 20 seconds**. Some monsters are only blinded for half as long.
Blinded monsters are **25% less likely to hit you**.

### Noble Sacrifice

Helps every innocent player and pet within 6 tiles:

- resurrects the dead,
- cures poison,
- heals for **power / 8 + 5–25**.

Afterwards your HP, mana and stamina **drop to 25%**.

## Paladin mastery

Killing monsters earns Paladin XP. XP earns mastery points:

```
XP for the n-th point = 800 × n + 2 × (n − 1)²
```

| Upgrade | Per tier | Max tier | Cost of tier 1 |
|---|---|---|---|
| Close Wounds Power | +5% healing | 5 | 1 |
| Exalted Sacrifice Power | +5% healing, −5% HP cost | 5 | 1 |
| Noble Sacrifice Power | +5% healing | 5 | 2 |
| Cleanse Efficiency | −2% HP cost | 5 | 1 |
| Vigor Duration | +5 s | 5 | 1 |
| Divine Fury Duration | +3 s | 5 | 1 |
| Divine Fury Speed | +2.5% swing speed | 5 | 2 |
| Divine Fury Power | +2.5% weapon damage to monsters | 3 | 3 |
| Divine Fury Resilience | −3% damage taken | 3 | 1 |
| Dispel Evil Duration | +3 s | 5 | 1 |
| Dispel Evil Protection | +2.5% damage reduction | 3 | 3 |
| Consecrate Duration | +3 s | 5 | 1 |
| Consecrate Accuracy | +3% hit chance | 3 | 2 |
| Enemy of One Duration | +3 s | 5 | 1 |
| Enemy of One Power | +5% damage | 3 | 3 |
| Enemy of One Defense | −15% vulnerability | 3 | 1 |
| Holy Light Range | +1 tile | 5 | 1 |
| Karma Reflection Power | +2 circles | 5 | 1 |
| Virtue Generation | +2.5% mark gain chance | 5 | 1 |
| Virtue Abundance | +1 mark per gain | 5 | 2 |
| Virtue Capacity | +10 max marks | 3 | 3 |
| Virtue Efficiency | −5% mark cost | 3 | 2 |

Each tier costs 1 point more than the one before. Resetting costs **100 gold per point spent**.
