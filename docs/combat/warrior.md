# Warrior Guide

Everything a melee or archery character needs in one place: what each skill gives you, how you hit, how you take less damage, how you heal and how you progress. Each section links to the page with the full rules.

Playing a spellcaster instead? See the [Mage Guide](../magic/mage-guide.md).

## What your skills do

| Skill | At 100 | At 120 | More |
|---|---|---|---|
| **Swords / Macing / Fencing / Archery** | Your attack skill for hit chance. 100 base unlocks that weapon's [codex](../codex/weapon-codex.md) | Higher hit chance | [Hit chance](#hit-chance) |
| **Tactics** | **+50%** weapon damage | **+70%** weapon damage (counts as 100 in PvP) | [Combat Formulas](formulas.md#melee-damage) |
| **Anatomy** | **+30%** weapon damage, bigger bandage heals | **+34%** weapon damage | [Combat Formulas](formulas.md#melee-damage) |
| **Healing** | Bandages always land, cure poison, resurrect (with Anatomy) | Bigger bandage heals | [Healing](#healing) |
| **Forensic Evaluation** | **+10 to +13** HP per bandage, **double** carving resources | **+12 to +16** HP per bandage, **2.2×** carving resources | [Healing](#healing) |
| **Focus** | **+17%** hit chance against monsters | **+20%** hit chance against monsters | [Weapons](../core/weapons.md#hit-chance), [Player](../core/player.md#regeneration) |
| **Parrying** | **20%** block chance with a shield, before shield and streak bonuses | **24%**, up to about **59%** with bonuses | [Parrying & Shields](parrying.md) |
| **Arms Lore** | **20%** chance to skip durability loss, **21%** to stop a magic property fading | **24%** and **25%** | [Weapons](../core/weapons.md#durability) |
| **Chivalry** | PvM heals and buffs powered by Virtue Marks | Longer buffs | [Chivalry](../magic/chivalry.md) |
| **Lumberjacking / Mining / Fletching / Scavenging** | **+30%** damage with axes / bashing / ranged / slashing weapons in PvM (+20% in PvP) | **+34%** in PvM (+20% in PvP) | [Combat Formulas](formulas.md#melee-damage) |

One-handed axes, maces and bows get half the Lumberjacking, Mining or Fletching bonus.

Focus also speeds up your stamina regen and raises your Virtue Mark gain chance.

## Hit chance

Against an enemy with the **same skill as you**, your base chance is **50%**. Everything else raises it from there.

| Example (120 skill vs a 120-skill monster) | Hit chance |
|---|---|
| No bonuses | 50% |
| Supremely Accurate weapon (+10%, doubled against monsters) | 60% |
| Supremely Accurate + 120 Focus | **about 70%** |

- Other bonuses: Weapon Accuracy items, Consecrate Weapon, Concentration food, codex passives and more. Your PvM accuracy bonuses add up to **+75%** max. The full list is on [Weapons](../core/weapons.md#player-attacking-a-monster-pvm).
- **Miss streak:** with less than 15% total accuracy bonus, each miss in a row gives +5% on your next swing. This mainly helps new characters.
- Stronger monsters have higher skill and a flat accuracy bonus. Legendary monsters gain **+5% accuracy for each player** near them.

## Taking less damage

Several layers stand between a monster and your hit points.

### 1. Don't get hit

Evasion armor, the Archery, Fencing and Macing codex footwork talents, blinding the monster (Holy Light) and evading all lower a monster's chance to hit you. They add together up to **75%**. See [Weapons](../core/weapons.md#monster-attacking-a-player-pvm).

### 2. Block it

With a shield, a successful parry blocks **65%** of a weapon hit. Two-handed weapons can parry monsters too. See [Parrying & Shields](parrying.md).

### 3. Armor

Every point of armor rating (AR) removes **0.45% to 0.75%** of a melee hit.

| Your AR | Damage removed |
|---|---|
| 40 | 18% to 30% |
| 66 | 30% to 50% |
| 100 | 45% to 75% |

Your AR is shown on your status bar. Plate armor and a good shield are what get you there. See [Armor](../core/weapons.md#armor).

### 4. Damage reduction

Percent reductions from these sources add together, up to **50%** of what's left:

- **Dispel Evil** (Chivalry)
- Physical Resistance buffs and **magic food**
- **Slayer-type protection** on armor, clothing and [PvM runes](../items/ankhs-runes.md) (Undead, Daemonic, Draconic and so on) against that monster type
- **Guild** protection buffs
- **Bard** protection and taunt, and **Shield Taunt** against the monsters you taunted
- Some Druid stances

### 5. Hard limits

- A single monster melee hit on you is capped at **35 damage**. Bigger numbers come from spells and special abilities.
- **Burst protection:** when monsters hit you for more than 25 damage within 1.5 seconds, the extra is reduced by up to 60%. See [Player](../core/player.md#burst-protection).

!!! tip "Fighting bosses"
    Big hits from bosses are usually **special abilities**, not melee. Parrying a monster's special ability lowers its damage by 20–35%.
    See [Creatures](../core/creatures.md#monster-abilities).

## Healing

### Bandages

| | |
|---|---|
| **Heal per bandage** | min = Anatomy/5 + Forensics/10 + Healing/5 + 3 |
| | max = Anatomy/5 + Forensics/7.5 + Healing/2 + 10 |
| **Success chance** | (Healing + 10)%, so always at 90+ Healing |
| **Self-bandage time (PvM)** | 3.5 s at 120 Dexterity, +0.6 s per 10 Dexterity below that (min 2.5 s) |
| **Cure poison** | needs 60 Healing and 60 Anatomy |

At **120 Healing, Anatomy and Forensics** a bandage heals **63 to 110 HP**. Without Forensics it's 51 to 94.

In PvM, damage never makes your bandages slip.

### Other healing

- **Chivalry:** Close Wounds, Exalted Sacrifice, Noble Sacrifice, Cleanse by Fire and Remove Curse. See [Chivalry](../magic/chivalry.md).
- **Potions** and [food](../core/food.md).

## Getting stronger

| System | What it gives | Page |
|---|---|---|
| **Weapon Codex** | Talents and active abilities for your weapon type, earned by killing monsters | [Weapon Codex](../codex/weapon-codex.md) |
| **Chivalry mastery** | Cheaper spells, faster Virtue Mark gain, longer and stronger buffs | [Chivalry](../magic/chivalry.md) |
| **Masteries** | Extra power from Aero, Artisan and others | [Masteries](../masteries/index.md) |
| **Ankhs & PvM Runes** | Hit chance, evasion, damage and protection against monster types | [Ankhs & PvM Runes](../items/ankhs-runes.md) |
| **Gear** | Accuracy, evasion, Slayer-type protection and more | [Gear Properties](../items/gear-properties.md) |

!!! note "Codex XP"
    Codex XP only counts while you have **no pets or summons** out and are using that weapon type.
    New codexes level faster: see [Weapon Codex](../codex/weapon-codex.md#points).
