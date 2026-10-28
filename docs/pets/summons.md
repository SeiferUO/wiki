# Enhanced Summons

Summoned creatures on the shard are **Enhanced Summons**. Each summon spell levels up as you use it and unlocks its own ability tree.

Related pages: [Summoner Rituals](../magic/rituals.md) for the Summoner Lantern, and [Creatures](../core/creatures.md#summons) for dispelling and followers.

## The summons

| Summon | Spell |
|---|---|
| Fire Elemental | Summon Fire Elemental |
| Water Elemental | Summon Water Elemental |
| Earth Elemental | Summon Earth Elemental |
| Air Elemental | Summon Air Elemental |
| Daemon | Summon Daemon |
| Energy Vortex | Energy Vortex |
| Blade Spirits | Blade Spirits |
| Summoned Creature | Summon Creature |
| Animated Dead | [Animate Dead](../magic/necromancy.md#animate-dead) |

## Basics

- A summon lasts **10 minutes**. Each corpse your Summoner Lantern drains adds **30 seconds**. Summon Duration runes and some abilities add more. Hover over the summon to see its time left.
- Summons are hard to dispel (difficulty 155). Spirit Speak makes them even harder.
- In PvP, summon stats are scaled down and their skills count as 100 max.
- How strong a summon is depends on you when you cast it: see [How summons scale](#how-summons-scale).

## How summons scale

A summon's strength is set **when you cast it**, from your skills and bonuses at that moment.

### Stats and damage

Every bonus below adds up into one multiplier. It raises the summon's **Str, Dex, Int, HP and damage** all together.

| Source | Bonus | Max |
|---|---|---|
| **Spirit Speak** | +1% per 4.5 skill | +25% (at 112.5) |
| **Arcane scrolls** for that spell | +0.25% per point | +25% (at 100 points) |
| **Summon level** (Summon Mastery tome) | +2.5% per level | +25% (level 10) |
| **Mastery**, while the matching mastery is activated | grows with mastery level | about +30% |
| **Spellbook summon property** for that summon (e.g. *Fire Elemental*) | +1% per point | +50% |

A summon with everything maxed has about **2.5× its base stats and damage**.

Each summon uses its own mastery:

| Summon | Mastery |
|---|---|
| Fire Elemental | Fira |
| Water Elemental | Holy |
| Earth Elemental | Earth |
| Air Elemental | Aero |
| Daemon | Doom |
| Energy Vortex | Energy |
| Blade Spirits | Berserk |
| Animated Dead | Death |
| Summoned Creature | your activated mastery (it also sets its form) |

### Skills

- **Magic Resist** = your Spirit Speak.
- **Wrestling, Tactics and Anatomy** = your Evaluating Intelligence.
- Summons that cast copy your **Magery, Eval Int and Meditation**.
- **Unlimited Knowledge** (ability 2) adds +8 to +15 to all of these.

### Armor

- Every **10 arcane scroll points** add +1 armor and +1% poison resistance.
- **Bulwark Stance** (ability 5) adds +7 to +15 armor, Magic Resist and poison resistance.

### Spiritbond

While fighting, a summon **grows stronger** every 15 seconds:

- +1% damage per tick (+2% against champion spawn creatures), and a little more if you're within 6 tiles.
- Up to **+30%** damage. Hover over the summon to see its Spiritbond.
- It slowly fades when the summon is out of combat.
- It doesn't grow against monsters with more than 75,000 HP or monsters that can't move.

### Control slots

| Summon | Slots |
|---|---|
| Blade Spirits | 1 (0 with **Efficiency**) |
| Fire, Water, Earth, Air Elemental, Energy Vortex, Summoned Creature | 2 |
| Daemon | 4 |
| Animated Dead | depends on the corpse |

## Leveling a summon

Keep a **Summon Mastery** tome in your backpack. While a summon is out, monsters you kill give that summon type XP.

- Each summon type has **10 levels**.
- Level 1 needs 50,000 XP. Each level after that needs 100,000 more.
- Lower levels earn XP much faster (×25 at the start, ×1 at max).
- **Each level gives 4 Ability Points (AP)**, so 40 AP at max level.

### Two point pools

| Pool | Max | Used to |
|---|---|---|
| **Ability Points (AP)** | 40 | **unlock** abilities |
| **Mastery Scroll points** (that spell's arcane scroll points) | 100 | **upgrade** unlocked abilities (3 levels each) |

- Unlocking costs 3 AP for abilities 1–3, 6 for 4–6, 8 for 7, 10 for 8 and 10, and 12 for 9. That's 67 AP for everything, so you **can't unlock them all**.
- Upgrading an ability costs its base cost × the new level. The base cost is 2 for abilities 1–3, 3 for 4–6, 4 for 7–9 and 5 for ability 10.
- Changes apply the **next** time you summon.

## Ability trees

Each row shows the unlock effect, then the upgrades for levels 1/2/3.

### Fire Elemental

| Ability | Effect | Upgrades |
|---|---|---|
| Stygian Breath | Volley of fireballs at one foe | +1/+2/+3 fireballs |
| Unlimited Knowledge | +8 skill caps | +10/12/15 |
| Molten Touch | Hits can burn the target | +1 strike per level |
| Unconditional Bond | When it dies, you regain 8% mana | 10/12/15% |
| Bulwark Stance | +7 physical/poison resist | 10/12/15 |
| Mirror | 10% chance to reflect damaging spells | 15/20/25% |
| Magical Potency | Learns Magery, Eval Int and Meditation | +5/10/15% Int |
| Ignitus Breath | Melee hits spray fire in a 1-tile cone | range 2/3, +15% damage at level 3 |
| Pyrebound | Loses 1% HP every 15 s, gains +10% damage | −2/3/4%, +15/20/25% |
| Nitro | Area blast within 3 tiles | +10/20/30% range and damage |

### Water Elemental

| Ability | Effect | Upgrades |
|---|---|---|
| Splash! | Hits up to 3 targets | 4/5/6 targets |
| Unlimited Knowledge | +8 skill caps | +10/12/15 |
| Arcane Resonance | +20% spell damage | 25/30/35% |
| Genesis | May regenerate 10% HP over 5 s when hit | 14/16/20% |
| Bulwark Stance | +7 physical/poison resist | 10/12/15 |
| Elusive Form | 10% chance to absorb 20% of incoming damage | 15/20/25% |
| Last Breath | On death, another summon heals 5% of its max HP | 7/10/13% |
| Hydro Blast | Armor-ignoring blast | 2/3/4 blasts |
| Toxic Water | Gains the Poisoning skill | +5/10/20 |
| High Tides | Damaging tide around it | +10/20/30% |

### Earth Elemental

| Ability | Effect | Upgrades |
|---|---|---|
| Crushing Blow | Extra damage to its target | +25/50/75% |
| Unlimited Knowledge | +8 skill caps | +10/12/15 |
| Force of Nature | +7% physical damage | 10/12/15% |
| Granite Shield | Invulnerable to spells and melee for 3 s | 5/7/10 s |
| Bulwark Stance | +7 physical/poison resist | 10/12/15 |
| Stonebreaker | +20% damage to frozen or paralyzed foes | 30/40/50% |
| Genesis | Out of combat, regains 2% HP every 5 s | 4/6/8% |
| Earth-Linked | After 5 s standing still, absorbs 15% physical damage | 20/25/30% |
| Massacre | Big hit that scales with the target's remaining HP | +15/25/35% |
| Seismic Clap | Wide frontal cleave | +15% per level |

### Air Elemental

| Ability | Effect | Upgrades |
|---|---|---|
| Double Strike | Can land several strikes at once | +10/15/20% per strike |
| Unlimited Knowledge | +8 skill caps | +10/12/15 |
| Hindering Strike | 10% chance to hinder | 15/20/25% |
| Sorcerer's Gambit | +35% spell damage, +20% damage taken | 15/12/9% taken |
| Bulwark Stance | +7 physical/poison resist | 10/12/15 |
| Tempest | Chain lightning, 2 strikes | 3/4/5 strikes |
| Mirror | 10% chance to absorb and reflect spells | 15/20/25% |
| Cyclone | 10% chance for melee to hit 3 more targets | +5/7/10% |
| Eye of the Storm | Lightning spells heal it and spread damage | +30/40/50% healing |
| Stampede | 6 s of extra attack speed, cast speed and damage | 8/10/12 s |

### Daemon

| Ability | Effect | Upgrades |
|---|---|---|
| Growing Anger | +1% damage per 30 s alive (max 30%) | 2/3/4% |
| Unlimited Knowledge | +8 skill caps | +10/12/15 |
| Molten Touch | Spells have 5% chance to restore 1% HP | 8/10/12%, 2/3/4% HP |
| Unconditional Bond | When it dies, you regain 7% mana | 10/15/25% |
| Bulwark Stance | +7 physical/poison resist | 10/12/15 |
| Infernal Strike | Flurry of burning strikes | +1 strike per level |
| Balrog Tongue | Blasts every enemy in a line | +10/20/30% |
| Infernal Shield | 10% chance to reflect spells, stronger | 15/20/25% |
| Inferno | Damage ripples up to 3 tiles | +10/20/30% |
| Hellfire | Summons Ignitus to burn everything around it | +10/20/30%, 4/5/6 tiles |

### Energy Vortex

| Ability | Effect | Upgrades |
|---|---|---|
| Ethereal Sap | Damage has 5% chance to restore 1% HP | 8/10/12%, 2/3/4% HP |
| Unlimited Knowledge | +8 skill caps | +10/12/15 |
| Eldritch Touch | 10% chance for damage to bounce to another target | more targets, 35/45/55% damage |
| Unconditional Bond | When it dies, you regain 8% mana | 10/12/15% |
| Bulwark Stance | +7 physical/poison resist | 10/12/15 |
| Wither | Withering frost on nearby enemies | +10/20/30% |
| Reflective Stance | +15% chance to reflect spells | 20/25/30% |
| Quicksilver | Big attack-speed boost for 5 s | 7/9/12 s |
| Channeling Pact | Loses 30% damage, **you gain +15% spell damage** | −25/20/15%, +20/25/30% |
| Surge | Shoves and damages everything in its path | range 2/3/3, +10/20/30% |

### Blade Spirits

| Ability | Effect | Upgrades |
|---|---|---|
| Double Trouble | May strike twice | +10/20/30% damage |
| Unlimited Knowledge | +8 skill caps | +10/12/15 |
| Toxicity | Learns Poisoning | 100/105/110 skill |
| Unconditional Bond | When it dies, you regain 5% mana | 7/10/12% |
| Bulwark Stance | +7 physical/poison resist | 10/12/15 |
| Velocity | Gets faster the longer it lives | +5/10/15% |
| Death Pact | +25% damage dealt and taken | −3% per level |
| Dancing Blades | Chance for a bouncing blade | +15/20/25% damage |
| Hemorrhage | 15% chance to bleed for 100% extra damage over 10 s | 20/25/30% |
| Efficiency | Costs **no control slots**, but −30% stats and only 1 at a time | −25/20/15% |

### Summoned Creature

| Ability | Effect | Upgrades |
|---|---|---|
| Genesis | Chance to heal 3% when injured | 5/7/10% |
| Unlimited Knowledge | +8 skill caps | +10/12/15 |
| Neverending Story | **+5 minutes** summon duration | 7/9/12 min |
| Last Breath | On death, another summon heals 5% of its max HP | 7/10/13% |
| Bulwark Stance | +7 physical/poison resist | 10/12/15 |
| Force of Nature | +10% spell or melee damage | 15/20/25% |
| Mirror | +15% chance to reflect spells | 20/25/30% |
| Survivalism | +8% max HP | 10/12/14% |
| Arcane Empowerment | Main ability +15% stronger | 20/25/30% |
| Growing Fury | +1% damage per 30 s alive (max 30%) | 2/3/4% |

### Animated Dead

| Ability | Effect | Upgrades |
|---|---|---|
| Vengeful Spirit | Loses 1% HP every 15 s, gains +10% damage | −2/3/4%, +15/20/25% |
| Unlimited Knowledge | +8 skill caps | +10/12/15 |
| Already Diseased | +7 poison/disease resist | 10/12/15 |
| Last Breath | +5% melee damage below 25% HP | 10/12/15% |
| Bulwark Stance | +7 physical/magic resist | — |
| Unconditional Bond | When it dies, you regain 8% mana | 10/12/15% |
| Mirror | +15% chance to reflect spells | 20/25/30% |
| Survivalism | +5% max HP | 7/10/12% |
| Arcane Empowerment | Main ability +15% stronger | 20/25/30% |
| Eldritch Stance | Learns Magery | +5/10/15% spell damage |

## Combat bonuses for summoners

- Each summon you have out can **surge** (Summon Surge on spellbooks and runes). A surge heals 25% over 5 ticks, adds +1 to its damage scalar (max 30) and gives Quicksilver or 5 empowered spells.
- **Summon Heal** (spellbook, runes) gives your summons a chance to heal for 35% of the damage they deal.
- Summons more than 12 tiles from you deal less damage: −5% per extra tile, max −90%.
