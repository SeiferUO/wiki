# Weapons & Melee

Everything that happens when you swing a weapon: speed, hit chance, damage, armor, parry and durability.

!!! note
    Numbers marked *default* come from in-game balance controllers and can be changed by staff.
    For the short version of hit chance and damage scaling, see [Combat Formulas](../combat/formulas.md).

## PvP or PvM?

Many numbers on this page are different in PvP. You count as being **in PvP** when any of these is true:

- You are in a duel pit or deathmatch arena.
- You are in a MOBA match.
- You are fighting a Duelist NPC.
- You (or your pet) are actively fighting another player.

Fighting a staff member never counts as PvP. Everything else is **PvM**.

## Weapon damage and speed

Each weapon's base damage range and speed are set by staff in the Weapon Damage controller. They can be different for PvP and PvM.
Check a weapon in game to see its current values. Higher speed means faster swings.

## Swing speed

```
delay (seconds) = 15000 / ((speed stat + 100) × weapon speed)
```

The **speed stat** depends on what you're holding and where you are:

| Situation | Speed stat |
|---|---|
| Normal weapons | (Stamina + Dexterity) / 2 |
| Mage staves, PvM | (Mana + Intelligence) / 2 |
| Mage staves, PvP | Mana |
| [Battle Lute](../bard/battle-lute.md) | its own bard stat |

**Example:** 100 Stamina, 100 Dexterity and a weapon with speed 50: 15000 / (200 × 50) = **1.5 s**.

### PvM speed bonuses

In PvM, these bonuses add together and shorten the delay:

| Source | Bonus |
|---|---|
| Aero mastery | scales with mastery level |
| Quicksilver | +15% |
| Savagery | +15% |
| Divine Fury (Chivalry) | spell bonus |
| Magic food (Attack Speed) | +7.5% |
| Warrior Feast | +10% |
| Artifact weapon speed | +5% per point |
| Attack Speed item property + Weapon Speed runes | max 50% combined |
| Lunar armor set | set bonus |
| Druid stances | Crab/Worm when active; Peacock 5% + 1% per Nature level (max 25%) |
| Weapon codexes (Swords, Macing, Fencing, Archery) | see [Weapon Codex](../codex/weapon-codex.md) |
| Slowed | −15% |

- **Total bonus is capped at 60%.**
- **Fastest possible swing in PvM: 0.6 s.**
- **Fastest possible swing in PvP: 1.25 s** *(default)*. PvM bonuses don't apply in PvP.

### Creature swing speed

Monsters and pets use 35% Dexterity + 65% Stamina as their speed stat.

| Modifier | Effect |
|---|---|
| Quicksilver | +25% |
| Berserk (Berserker codex) | +15% |
| Aero mastery (owner) | up to +15% for pets and summons |
| Slowed | −15% |
| Casting debuffs / Disoriented | slower |

Fastest swing: **0.85 s** for pets in PvM, **1.0 s** for pets in PvP *(default)*, **1.0 s** for monsters.

## Hit chance

The basic formula is on the [Combat Formulas](../combat/formulas.md#hit-chance) page. These extra rules apply on top of it.

### Player attacking a monster (PvM)

All these bonuses add together, are **capped at +75%**, and then multiply your hit chance:

| Source | Bonus |
|---|---|
| Focus skill | 0% at 0, up to **+20% at 120** |
| Weapon Accuracy property (weapon, clothing, jewelry) | +1% per point |
| Artifact weapon accuracy | +10% per point |
| Consecrate Weapon (Chivalry) | spell bonus |
| Magic food (Concentration) | +15% |
| Aero mastery | scales with level |
| Artisan mastery, player-crafted weapon | +0.1% per point of the crafting skill (Fletching for bows, Carpentry for staves, Blacksmithing for the rest) + mastery level |
| Sphere players with 100+ Tactics | +25% |
| Bard aura (Peacemaking) | party bonus |
| Tiger stance (Druid) | stance bonus |
| Weapon codexes | see [Weapon Codex](../codex/weapon-codex.md) |

- **Miss streak:** if your total bonus is under 15%, each miss in a row adds +5% to your next swing. A hit resets it.
- **Mage staves:** +0.1% per point of Focus and Meditation (PvM only).
- Hit Chance Increase on your weapon (Accurate to Supremely: +2% to +10%) **counts double against monsters**.

### Monster attacking a player (PvM)

Your defensive bonuses add together, are **capped at 75%**, and lower the monster's chance to hit you:

| Source | Bonus |
|---|---|
| Evasion armor property | −1% per point |
| Evasion spell enhancement | spell bonus |
| Monster is blinded | −25% |
| You are evading | −25% |
| Archery/Fencing/Macing codex footwork | see [Weapon Codex](../codex/weapon-codex.md) |

Monsters get a flat accuracy bonus from their [difficulty tier](creatures.md#difficulty-tiers).
Legendary monsters gain **+5% per attacker within 12 tiles**. Hard-tier or stronger monsters get **+25% against pets**.

### Always hit / always miss

- **Always hit:** Stealth attacks, concentrating monsters attacking a player, Legendary monsters attacking pets.
- **Always miss:** a blind player. Players also always miss monsters that are evading (invasions).

**Final chance is always between 10% and 100%.**

## Damage

### 1. Base roll

You roll the weapon's damage range.

- **Two-handed weapons in PvM** roll toward the high end of the range (square-root distribution).
- Magic weapons add a flat bonus: Ruin +1, Might +3, Force +5, Power +7, Vanquishing +9.

### 2. Skill and stat scaling

Tactics, Anatomy, Strength, crafting skills and weapon quality are applied next.
See the full table in [Combat Formulas](../combat/formulas.md#melee-damage).

Damage is then **halved if the target is a player**. Creature damage is always halved.

### 3. Armor

See [Armor](#armor) below.

### 4. PvM bonus damage

When a player hits a monster with a weapon, every bonus below is added together and applied to the damage left after armor.
**The total is capped at +500%.**

| Source | Bonus |
|---|---|
| **Weapon skills** | +1% per 10 total points of Swords + Macing + Fencing + Archery (max +20%) |
| **Tracking skill** | up to +20% at 120 Tracking. Another +35% at 120 against a creature you are tracking |
| **Slayer** | +20% against the matching creature type |
| **Weapon Damage** property (weapon, armor, clothing, jewelry, runes) | +1% per point, max **75%** combined |
| **Critical hit** | Critical Damage property + Critical Chance runes = % chance (max 30%) for **+25%** (more with Critical Damage runes, max +30%) |
| **Boss damage** property + runes | +1% per point, max 50% (Mini-boss tier and above) |
| **Mage Killer** property + runes | +1% per point, max 50% against spellcasting monsters |
| **Creature-type runes** (Undead, Arachnid, Daemonic, Draconic, Elemental, Giant, Vermin, Infidel) | max 25% each |
| **Armor Penetration** runes | chance (max 30%) to add half the monster's armor as extra damage |
| **Backstab runes** | bonus when hitting a monster from behind |
| **Knives from behind** | +20% |
| **Stealth attack** | (Hiding + Stealth) × 0.75–1.0 %, doubled if the target is tracked, +20% from behind, + Shadow mastery and Rogue set bonus |
| **Savagery** | 15% damage while active. Trigger chance from weapon, armor, clothing, runes and Ankh necklace (max 10%) |
| **Bulwark mastery** | +3.5% per aggressor (max +35%) |
| **Berserker codex** | +1% per 2% HP missing (max +30%) |
| **Maniac** | +30%, but each hit costs you 2–5 HP |
| **Enemy of One** (Chivalry) | bonus against the chosen creature type |
| **Holy curse** | +10% + Holy mastery level |
| **Lyrical mastery** | +10% + level against peaced or provoked monsters |
| **Shadow mastery** | bonus against isolated monsters |
| **Hiryu mount** | +15% + 2% per stage (max +30%) |
| **Cartography** | up to +30% against Chest Guardians (25+ Cartography) |
| **Ankh necklace (Friendship)** | +10% with a party or guild member nearby |
| **Guild boss buff** | +5% per buff level against bosses |
| **Danger zones** | region bonus, max +50% |
| **Artisan mastery** (player-crafted weapon) | bonus from the matching crafting skill + mastery level |
| **Artifact clothing** | Hunter's Headdress (bows) or Spirit of Totem (axes): +5% per tier |
| **Doom armor sets** | Nightmare, Daemon Bone (2% proc per piece) and Bloodstained (heals) |
| **Masteries** (Energy, Oblivion, Death, Earth, Druid stances) | see [Masteries](../masteries/index.md) |
| **Weapon codexes** | see [Weapon Codex](../codex/weapon-codex.md) |

!!! tip "Life leech"
    The Weapon Lifeleech property (plus runes) is a % chance, max 30%, to heal for part of the damage dealt.
    Slower weapons can heal more per hit. Ranged weapons heal 25% as much.

### 5. Final caps

| Situation | Damage |
|---|---|
| Minimum weapon hit | 2–5 |
| Player vs player | max **55** per hit |
| Monster vs player | max **35** per hit |
| Pet vs player | max **15** per hit *(default)* |

### Followers lower your weapon damage

When you have more than **3 control slots** of pets out *(default)*, every extra slot lowers your weapon damage by **15%** *(default)*.
This does not apply while you hold a Shepherd's Crook.

## Armor

Your armor rating (AR) lowers incoming melee damage by a random amount between **0.45% and 0.75% per AR point**.

| | Max AR |
|---|---|
| Players | set by staff |
| Creatures | 150 |

- PvM armor bonuses (virtual armor) are removed in PvP.
- **Mage staves ignore creature armor.** The monster's **Magic Resistance** lowers staff damage by 2.5% per 10 points instead *(default)*.
- Monsters with Parry have a Parry/100 chance to block 20–25% of a hit.

### Which armor piece gets hit

| Slot | Chance |
|---|---|
| Chest | 35% |
| Legs | 22% |
| Head | 15% |
| Arms | 14% |
| Gloves | 7% |
| Neck | 7% |

## Parrying

- **With a shield:** Parry × 0.2% + shield AR × 0.25% (max 20%), plus a failed-parry streak, up to **65%**. A successful parry blocks **65%** of the hit.
- **With a two-handed weapon** (against monsters): (Parry − 50)%, blocking 25% (15% with a bow).

See [Parrying & Shields](../combat/parrying.md) for the full rules, shield AR, Shield Taunt and casting with a shield.

## Durability

Each hit has a **2% chance** *(default)* to cost your weapon 1 durability point, at most once per minute *(default)*.

- **Arms Lore** gives a chance to skip the loss: 2% per 10 points (20% at 100).
- Danger-zone fortification adds up to 15% more.
- Below 10% durability you get a warning.
- With the **StoreBeforeDestroy** account option on, a weapon at 1 durability is moved to your backpack before it breaks.

Magic properties on non-artifact weapons can also slowly fade with use: 0.25% chance per hit *(default)*.

## Hit spell properties

Against monsters, weapon properties can cast a free spell on hit. The number is the % chance per hit:

**Hit Magic Arrow, Hit Harm, Hit Fireball, Hit Lightning, Hit Curse, Hit Explosion.**

**Area Damage** (Felucca only) has a % chance to hit every monster around the target.

## Chivalry in PvP

Every 10 points of Chivalry add **+1% weapon damage against players** (max +10%).
This does not apply to fists or mage staves.
