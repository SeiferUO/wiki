# Mage Staves

A **mage staff** (the **Tribal Staff**) is a one-handed caster weapon. It fires magic bolts that scale with your mind instead of your muscles, restores mana and builds up the **wizard staff gauge** that releases your mastery's staff effect.

## Basics

- **Weapon skill:** **Mysticism**. It sets your hit chance and gains with each shot.
- **Damage** scales with Evaluating Intelligence, Intelligence and Focus (below).
- Holding a staff counts as a **mage** weapon for [masteries](../masteries/index.md#roles).
- You can **cast spells** while holding a staff, outside PvP combat.
- Staves are crafted with **Carpentry**. They roll spellbook properties (see [Gear Properties](../items/gear-properties.md#spellbooks-and-mage-staves) and [Enchanting & Crafting](../items/enchanting-crafting.md#mage-staves)).

## Firing

- **Stand still to fire.** After moving you wait 0.35 s + (120 − Intelligence) ms before the next shot.
- Each shot costs **mana**, with a different cost in PvM and PvP *(set by staff)*. No mana, no shot.
- Staff can turn off staff attacks against players.
- In a WOTA match staff shots cost no mana.
- **Swing speed** uses your mana and Intelligence instead of stamina and Dexterity. See [Weapons & Melee](../core/weapons.md#swing-speed).
- **Hit chance (PvM):** +0.1% per point of Focus and of Meditation.

## Damage

Starting from the staff's base damage *(set by staff)*:

| Modifier | Change |
|---|---|
| Evaluating Intelligence | +(Eval Int − 50)%: −50% at 0, +50% at 100, +70% at 120 |
| Intelligence | +Int ÷ 5 % |
| Focus | +Focus ÷ 5 %, plus **+10%** at 100+ Focus |
| Quality | Ruined −30%, Decrepit −20%, Low −10%, Superior +10%, Exceptional +20%, Mastercrafted +30% (max +20% in PvP), the same as other weapons |

**Against monsters:**

- Staves **ignore armor**. Instead, the target's **Magic Resistance** lowers the damage by 2.5% per 10 points *(set by staff)*.
- **Wizard staff mastery bonus:** more damage by your active mastery's level *(set by staff)*.
- **Magic Resistance debuffs** on the monster add up to +35%. **Runic Curse** adds +20%.
- **Druidic** stances: Ophidian adds its spell damage bonus. Drake has a chance to set the target burning, and Daemon a chance to surge for +30% (each 7.5% + 0.5% per Nature level, max 30%).
- **Burster** stance: chance to chain a hit to another nearby monster. See [Wizard](../masteries/wizard.md#mage-stances).

**Against players:** the target's Magic Resistance lowers the damage by 2.5% per 10 points *(set by staff)*.

## Mana on hit

Each staff hit on a monster has a **Eval Int ÷ 8 %** chance (15% at 120) to restore mana:

| Source | Mana |
|---|---|
| Base | 5 |
| Exceptional / Mastercrafted | +5 / +8 |
| Wood: Oak / Ash / Yew / Heartwood / Bloodwood / Frostwood | +5 / +6 / +7 / +8 / +9 / +10 |
| Damage level (loot staves): Ruin / Might / Force / Power / Vanquishing | +2 / +4 / +6 / +8 / +10 |

## Wizard staff gauge

- Each staff hit adds **+5 charge**, up to **100**. Hits in PvP don't charge it.
- At **100**, your next hit on a monster releases your **mastery's staff effect**. That costs **3 Arcane Dust**, empties the gauge and adds a charge to your [mastery gauge](../masteries/wizard.md#mastery-gauge) (up to 5 from staff hits).
- Equipping a staff opens the wizard trigger window.

"Hit damage" below means the damage of the staff hit that set off the effect.

| Mastery | Staff effect |
|---|---|
| **Fira** | Ignites the target. If it's already burning, deals extra damage equal to the hit. Leaves a fire patch |
| **Bulwark**, **Earth**, **Artisan** | *Protected* for 10 s: immune to monster special-ability damage |
| **Aero** | **Quickspell** for 10 s: 15% faster casting |
| **Blood** | Heals you 15% + 1.5% per Blood level of your max HP, and makes the target bleed for the hit damage over 3 ticks |
| **Doom** | **Runic Curse** on the target for 15 s (+20% staff damage, see [Masteries](../masteries/index.md#doom-delayed-burst)) |
| **Lyrical** | Uses your best bard skill. **Peacemaking:** pacifies for 5 s plus a level bonus (2 s on Legendary monsters). **Discordance:** up to 30% weaker. **Provocation:** provokes it onto the nearest monster (not Legendary) |
| **Poison** | Poisons the target. 15% + 1% per Poison level chance for **Lethal** poison. With high Poisoning it also poisons creatures around it: 100 → Regular, 3 tiles; 110 → Greater, 4 tiles; 120 → Deadly, 5 tiles |
| **Shadow** | Shadow fog around the target, which is **blinded** for 5 s |
| **Holy** | Deals 2× the hit damage (3× to undead). Heals and cures up to 3 nearby players, friends first, for 10% + 1% per Holy level of your max HP |
| **Fortune** | Random damage between Fortune level ÷ 2 and 100 + level (max 150). A **jackpot** (rolling 7 or 77, a "blackjack", or a luck roll: 2.5% + Hunter's Luck + Fortune level, max 35%) deals **7×** the hit damage |
| **Death** | 3 ticks of 100% / 75% / 50% of the hit damage, **doubled** if the target is below 35% HP |
| **Nature** | Shapeshifted: resets your druidic abilities. Otherwise: heals all your pets 25% of their max HP |
| **Energy** | Freezes the target for 3 s and arcs to up to 5 monsters within 6 tiles, splitting the hit damage. Each can be frozen too (level ÷ 60, max 50%). Uses Energy charges; higher levels keep up to 75% |
| **Berserk** | Deals the hit damage plus up to +75%, the lower your HP. Below 30% HP, heals you for 40% of that damage |
| **Oblivion** | Outside PvP: restores 10% + up to 20% by level (max 30%) of your max mana, 3 times, every 2 s |
