# Druidic Mastery

The **Nature** mastery. Druids shapeshift into creatures, and the weapon you hold decides which ones. Each form has a **switch buff**, a **passive** while you're in that form, and a **special ability** (archery forms get special ammo instead).

General mastery rules (leveling, orbs, Arcane Dust) are on the [Masteries](index.md) page. All values below scale with your **Nature level** (max 30).

## Shapeshifting

1. Activate Nature mastery. The **stance window** opens (it also opens at login). You can reopen it with `[stance`.
2. Click a form to shapeshift. Which forms you see depends on what you hold:

    | You hold | Forms |
    |---|---|
    | A melee weapon | Tiger, Ram, Ophidian, Crab, Terathan, Peacock |
    | A bow or crossbow | Purger, Worm, Bug |
    | A wizard staff or spellbook | Ophidian Mage, Drakeling, Gargoyle |

3. While shapeshifted you move at **mounted speed** on foot. If you're mounted, you're dismounted. You get your mount back when you return to human form.
4. Pick **Human** (or `[druid 0`) to return to normal.

**Shortcuts:** `[druid 1`–`[druid 6` shapeshifts into the form in that slot. `[druidability` uses your special ability. The **Options** button opens the Druidic Stance Compendium, which describes every form.

### Rules

- Shapeshifting needs at least **1 Arcane Dust**.
- **Cooldown** between form changes: **60 s − 0.25 s per Nature level** (52.5 s at 30). Returning to human form has no cooldown.
- You can't shapeshift while in PvP combat, in duel pits, while casting, while polymorphed or in a costume, or while holding a Shepherd's Crook or a runebook.
- Your form ends when you:
    - die,
    - equip a weapon for a different set of forms, or a Shepherd's Crook,
    - get hit by a **Dismount** attack,
    - commit a criminal act while not mounted.
- Regions with no mounts turn off the speed bonus.

### Switch buff

Every time you shapeshift, you get that form's **switch buff**:

```
buff     = 5% + 2.5% per Nature level   (max 30%, reached at level 10)
duration = 30 s + 2 s per Nature level  (90 s at level 30)
```

- **Casting speed** and **spell damage** buffs are half as strong and last half as long.
- With a **spellbook** instead of a staff, mage switch buffs are **1.5×** stronger.
- Some forms have an instant effect instead (cure, heal, mana).

### Special ability

Damage you deal to monsters fills your **special gauge**:

```
gauge = 1,500 − 50 per Nature level   (min 250, reached at level 25)
```

- When it's full, click the ability button in the stance window, or say `[druidability` (costs 5 Arcane Dust).
- The ability has a **15 s cooldown** and empties the gauge.
- Specials only hit monsters and don't work in PvP.
- Archery forms don't have a special. They use [special ammo](#archery-forms) instead.
- The **Nature** [mage staff effect](../magic/mage-staves.md) refills your gauge and resets both cooldowns while you're shapeshifted.

## Melee forms

| Form | Switch buff | Passive | Special ability |
|---|---|---|---|
| **Tiger** | Accuracy vs monsters | +5% damage, +0.5% per level (max 25%) | **Massacre:** your next hit strikes 3 more times, for 100%, 75% and 56% of its damage |
| **Ram** | Melee damage | 10% damage resistance vs monsters, +0.5% per level (max 20%) | **Charge** |
| **Ophidian** | Critical chance (crits deal +35%) | 15% chance to resist poison, +3% per level (max 45%) | **Whirlwind** |
| **Crab** | Attack speed | +10 HP regeneration, +1 per level (PvM) | **Shell:** a shield that absorbs 100 + 25 per level damage (max 250) |
| **Terathan** | Cures your poison | 5% chance to poison, +0.5% per level (max 20%) | **Venom strike** |
| **Peacock** | Heals 15% of your max HP, +0.5% per level (max 30%) | +5% swing speed, +1% per level (max 25%) | **Lightning storm** |

- **Charge (Ram):** rush a monster **3–14 tiles** away. You hit everything in your path and the target for your weapon's damage. The target is knocked back 3 tiles and frozen for 2 s, and monsters within 2 tiles of where you land are hit too.
- **Whirlwind (Ophidian):** 5 pulses around you. Each pulse hits up to 5 monsters within 6 tiles for 50% weapon damage.
- **Venom strike (Terathan):** your next hit poisons the target: Greater, Deadly at 110 Poisoning, Lethal at 120. If it's already poisoned, the hit deals double damage instead.
- **Terathan poison** (passive) depends on the average of your Tactics and Poisoning: Lesser, Regular at 65+, Greater at 85+, Deadly at 100.
- **Lightning storm (Peacock, Ophidian Mage):** strikes your target for your weapon's damage, then calls 25 bolts over 5 seconds within 5 tiles. Each monster can be hit once.

## Archery forms

- Each switch gives you **5 special ammo** for that form. The stance window shows how many you have.
- Each bow hit has a **10% chance (+1% per level, max 40%)** to give back 1 ammo.
- Your special ammo is used up on hits against monsters.
- Returning to human form clears your ammo.

| Form | Switch buff | Passive | Special ammo |
|---|---|---|---|
| **Purger** | Damage: +5%, +0.5% per level (max 25%) | 5% chance to ignore armor (adds half the monster's armor as damage), +0.5% per level (max 20%) | **Piercing:** adds the monster's full armor as damage |
| **Worm** | Attack speed | 10% damage resistance vs monsters, +0.5% per level (max 20%) | **Bleeding:** damage over time |
| **Bug** | Cures your poison | 15% chance to resist poison, +3% per level (max 45%) | **Acid spray:** a 6-tile cone for 50% of your hit's damage, with a 25% chance to poison (Regular; Greater at 105 Poisoning, Deadly at 110, Lethal at 120) |

## Mage forms

Hold a **wizard staff** or a **spellbook**. Spellbook users get stronger switch buffs.

| Form | Switch buff | Passive | Special ability |
|---|---|---|---|
| **Ophidian Mage** | Restores mana: 5 pulses of 5 + level / 10 mana (8 pulses of 1.5× with a spellbook) | 10% damage resistance vs monsters, +0.5% per level (max 20%) | **Lightning storm** (see above) |
| **Drakeling** | Spell damage | Spells can set monsters **burning**: 7.5% chance, +0.25% per level (max 30%) | **Fire breath** |
| **Gargoyle** | Casting speed | Spells can **surge** for +30% damage: 7.5% chance, +0.25% per level (max 30%) | **Fireball barrage** |

- **Fire breath (Drakeling):** a cone of fire with range 3 + level / 4 (max 8). Every monster in it takes your weapon's damage +1% per level, and the breath leaves fire on the ground. You're frozen for 2.5 s while breathing.
- **Fireball barrage (Gargoyle):** 3 to 5 + level / 5 fireballs at one monster within 12 tiles. Each deals 50% weapon damage +2% per level and leaves fire fields around the target.
- Staff hits have their own burn and surge chances (see [Mage Staves](../magic/mage-staves.md)).

## Tamer role

With a Shepherd's Crook (or empty hands), Nature is a pet-support mastery:

- **Veterinary is stronger** on your pets: +0.5% per level, max +15%.
- Bandaging a pet heals a further 10% + 0.5% per level.
- Pets can **surge**: on a hit, a pet can restore 12% (up to 19.5% with level) of its HP, mana and stamina, for all your pets within 12 tiles.
- Holding a crook while shapeshifted ends your form, so you can't get the mounted speed for free.
