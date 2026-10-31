# Mage Guide

Everything a spellcaster needs in one place: what each skill gives you, how to hit hard, how to keep your mana up, how to survive and how you progress. Each section links to the page with the full rules.

Playing a melee or archery character instead? See the [Warrior Guide](../combat/warrior.md).

## What your skills do

| Skill | At 100 | At 120 | More |
|---|---|---|---|
| **Magery** | Magery spells **never fizzle**. Buffs and curses give **±11** | **×1.07** spell damage, buffs and curses give **±13** | [Spellcasting](../core/spellcasting.md) |
| **Evaluating Intelligence** | Normal spell damage | **×1.20** spell damage in PvM (+1% per point above 100). Counts as 100 in PvP | [Spell damage](../core/spellcasting.md#2-skill-scaling) |
| **Meditation** | Always succeeds. Takes **6 s** off the 7 s mana regen base | Takes **7.2 s** off (100 max in PvP) | [Mana regen](../core/player.md#mana) |
| **Focus** | Takes **5.75 s** off mana regen, **10%** Surge chance, **60%** chance to keep a spell when hit (PvM) | Takes **6.9 s** off mana regen, **12%** Surge chance, **72%** chance to keep a spell when hit | [Spell interruption](../combat/formulas.md#spell-interruption-fizzle-protection) |
| **Inscription** | **+50%** buff duration, **+20%** damage when casting from scrolls, **10%** reflect against monster spells | **+60%** buff duration, **+24%** scroll damage, **12%** reflect | [Spellcasting](../core/spellcasting.md) |
| **Resisting Spells** | Monster spells deal **15% less**, **10%** reflect against monster spells | **18% less**, **12%** reflect | [Resisting](../core/spellcasting.md#5-resisting) |
| **Taste Identification** | Faster mana regen, cancels part of the armor penalty | Cancels the armor penalty fully | [Mana regen](../core/player.md#mana) |
| **Wrestling** | Your defense skill against weapons when you hold a spellbook or nothing | same | [Hit chance](../combat/formulas.md#hit-chance) |
| **Necromancy + Spirit Speak** | The Necromancy school. Spirit Speak also adds to necro damage | Stronger necro spells | [Necromancy](../magic/necromancy.md) |
| **Mysticism** | Weapon skill for [mage staves](mage-staves.md) | Higher staff hit chance | [Mage Staves](mage-staves.md) |
| **Item Identification** | Wand echo chance (up to 30%) | up to 36% | [PvM bonus damage](../core/spellcasting.md#3-pvm-bonus-damage-player-vs-monster) |
| **Tracking** | PvM spell damage | **+20%**, more on the creature you track | [Tracking](../skills/tracking.md) |

Inscription and Resisting Spells add together for reflect, up to **30%** with gear.

## Dealing damage

Against monsters, every spell gets a **+125%** baseline bonus. On top of that:

| Bonus | Amount |
|---|---|
| **Pure mage, no followers out** | +25% per circle from 4th circle up (Flame Strike **+175%**) |
| **Arcane scrolls** | +1% per point for that spell, up to +100% |
| **Spell Damage** gear and runes | +1% per point |
| **Spell-specific spellbook property** | +1% per point for that spell (up to +50% on a spellbook or staff) |
| **Surge** | Focus/10 % chance for +30% |
| **Casting from scrolls** | up to +50% with Inscription |

All PvM bonuses together cap at **+500%**. The full list is on [Spellcasting](../core/spellcasting.md#3-pvm-bonus-damage-player-vs-monster).

!!! tip "What counts as a pure mage"
    100 Magery (or Necromancy), 100 Evaluating Intelligence, and 150 combined Focus, Meditation, Spirit Speak and Mysticism, with no pets or summons out.
    Pure mages also get [Spell Promotion](spell-promotion.md) and the strongest [Wizard stances](../masteries/wizard.md). Characters with 75+ Animal Taming get half the arcane scroll bonus.

### Casting faster

- In PvM, wands, Cooldown, Casting Speed gear and runes, Quick Spell and Quickspell food add up to **75% faster** casting.
- Casting Recovery shortens the pause between spells by up to **25%**.
- In PvP, every spell uses its base cast time.

See [Casting time](../core/spellcasting.md#casting-time).

## Keeping your mana up

| Source | Effect |
|---|---|
| **Meditation, Focus, Taste Identification** | Each makes mana regen much faster, and Meditation and Focus keep improving up to 120. Two of them at 100 already gets you near the fastest regen (0.25 s per point) |
| **Actively meditating** | 35% faster regen |
| **Lower Mana Cost** gear | up to **40%** cheaper spells |
| [Spell Promotion](spell-promotion.md) | Casting the promoted spell refunds **35%** of its mana |
| **Spell Leech** | chance to heal for the spell's mana cost |
| [Eldritch Orb](eldritch-orb.md) | chance for a spell to cost **no mana** |
| [Mage staves](mage-staves.md) | staff hits restore mana |

!!! warning "Armor"
    Armor that isn't meditable slows your mana regen, and you can't actively meditate in it.
    **Taste Identification** cancels the regen penalty, fully at 120. See [Mana](../core/player.md#mana).

## Staying alive

### Against spells

Monster spells against you are reduced by these, added together up to **90%**:

- **Resisting Spells:** 0.15% per point (18% at 120)
- **Heavy armor**
- **Repeated hits:** +5% for each spell that hits you (max 25%). It resets after 2 minutes without spell damage. Not for tamers or summoners
- Some armor sets and masteries

Monster **Explosion** is capped at 40 damage against players and **Mind Blast** at 25.

**Reflect:** Inscription, Resisting Spells and Magic Reflection gear give a passive chance to bounce monster spells back, up to **30%**. See [Magic Reflection](../core/spellcasting.md#magic-reflection).

### Against weapons

- Monsters hit you based on their skill against your **Wrestling** (or the skill of what you're holding). Low Wrestling means monsters hit you more.
- Armor rating still lowers melee damage. See the [Warrior Guide](../combat/warrior.md#taking-less-damage) for armor, evasion and burst protection.
- **Protection** and **Focus** keep your spells from being interrupted when you're hit, up to about **95%** in PvM. See [Spell interruption](../combat/formulas.md#spell-interruption-fizzle-protection).

### Healing

- **Greater Heal** and **Heal**, boosted by the healing bonuses on [Spellcasting](../core/spellcasting.md#healing).
- **Spell Leech** gear and runes.
- Bandages and potions work for mages too.

## Getting stronger

| System | What it gives | Page |
|---|---|---|
| **Arcane scrolls** | +1% damage per point for one spell (max 100 points each). Summon scrolls make that summon stronger | [Enhanced Summons](../pets/summons.md) |
| **Grimoire** | Upgrades for individual Magery spells, earned by killing monsters | [Grimoire](grimoire.md) |
| **Spell Promotion** | Mana refunds, charges and bonus effects for casting your rotation | [Spell Promotion](spell-promotion.md) |
| **Wizard mastery** | Mastery gauge, staff gauge and mage stances | [Wizard](../masteries/wizard.md) |
| **Mage staves** | A caster weapon that fires magic bolts and restores mana | [Mage Staves](mage-staves.md) |
| **Eldritch Orb** | Free spells in your off hand | [Eldritch Orb](eldritch-orb.md) |
| **Summons** | Upgraded summoned creatures | [Enhanced Summons](../pets/summons.md) |
| **Ankhs & PvM Runes** | Spell damage, casting speed, mana regen and more | [Ankhs & PvM Runes](../items/ankhs-runes.md) |
| **Gear** | Spellbook properties, Lower Mana Cost, Spell Damage and more | [Gear Properties](../items/gear-properties.md) |

You can check your arcane scroll progress from the **Compendium**. Arcane scrolls drop from monsters, champion spawns and rare loot.
