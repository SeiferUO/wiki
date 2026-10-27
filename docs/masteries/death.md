# Death Mastery

A soul-harvesting mastery that feeds on death and builds **rage**. You disease enemies, collect soul orbs from corpses and unleash rage-fueled bursts.

General mastery rules (leveling, orbs, Arcane Dust) are on the [Masteries](index.md) page.

!!! note
    Numbers marked *default* come from the Mastery Balance controller and can be changed by staff.

## Active ability: Agonizing Disease

Triggers in combat like every mastery ability (warriors on weapon hits).

```
damage = (Spirit Speak + Necromancy) / 5 + ability damage
```

The target is then **diseased**, taking the same damage again every 1.5 seconds:

- **Ticks:** 1 + level / 2 (max 10).
- Disease ticks do **half damage** unless the target is below 60% HP.

Ability damage includes **+45 per mastery level**.

## Rage

Rage builds from **0 to 100**.

| You gain 1 rage when... | Role |
|---|---|
| you hit a monster for more than 15 base damage | Warrior |
| you take more than 15 damage (outside PvP) | Warrior or mage |
| you cast a damaging spell on a monster | Mage |

### What rage does

| Role | Effect |
|---|---|
| **Warrior** | **+0.25% weapon damage per rage** (max +25%). Needs Arcane Dust. Doesn't work with a Shepherd's Crook |
| **Mage** | **+0.25% spell damage per rage** (max +20%). At **100 rage** your next spell **surges** for +10% plus up to +20% more with level, and rage resets |

### Killing blows

When you land a killing blow on a monster, the overkill damage jumps to **one other monster within 6 tiles** (it can't kill it).

## Orbs of Damnation

Monsters you kill can drop an orb nearby. **Walk over it** to use it.

- **Drop chance:** 5% + a bonus for the monster's HP + up to 20% from level. Max 50%.
- Orbs last **30–60 seconds** (longer at higher level).

| Orb | Effect |
|---|---|
| **Health** (warriors) | Restores 10–20 HP + up to 30 more with level |
| **Mana** (mages) | Restores 10–20 mana + up to 30 more with level |
| **Damage** | Your next attack or spell deals **+5% to +50%** bonus damage (scales with level) |
| **Extended** (rare, dark purple) | **+5% to +20%** damage on every attack and spell for 30–60 seconds |

An orb has a **5% + up to 15%** chance (by level) to be Extended. Otherwise, warriors get health or damage orbs (50/50). Mages get mana orbs 60% of the time and damage orbs the rest.

## Role bonuses

| Role | Passives |
|---|---|
| **Warrior** | Damage grows with rage. Max rage unleashes power. Killing blows spread to the next foe. Weapon damage scales with level |
| **Tamer** | Pets deal up to **+15% damage** to monsters below 66% HP. Pets build rage (+0.2% damage per rage, max 15%). At 100 rage they burst for twice their max damage. Slain monsters may drop soul orbs |
| **Mage** | Soul orbs. Rage boosts spells and surges at 100. Spell damage +0.5% per level (max 15%) |

Summons get stronger with Death level: +1 per level, max +30.
