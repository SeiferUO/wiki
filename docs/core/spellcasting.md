# Spellcasting

Casting speed, mana, fizzles, spell damage, resisting, reflecting, buffs, healing and travel.

!!! note
    Numbers marked *default* come from in-game balance controllers and can be changed by staff.
    Spell interruption (Protection, Focus, Casting Focus) is on the [Combat Formulas](../combat/formulas.md#spell-interruption-fizzle-protection) page.
    PvP rules are explained on the [Weapons](weapons.md#pvp-or-pvm) page.

## Range and movement

- Spell range is **11 tiles** for players and most creatures.
- 1-slot Unchained pets have a range of **7 tiles** in PvP.
- Monsters standing on a **boat** cast from **13 tiles**.
- You **can't move while casting** most spells. A few effects let you move while casting.

## Casting time

```
cast delay = 0.5 s + 0.25 s per circle above the first
```

| Circle | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 |
|---|---|---|---|---|---|---|---|---|
| Delay | 0.5 s | 0.75 s | 1.0 s | 1.25 s | 1.5 s | 1.75 s | 2.0 s | 2.25 s |

### Faster casting (PvM only)

| Source | Faster by |
|---|---|
| Casting from a **wand** | 50% |
| Spell bonus: Cooldown | 50% |
| Casting Speed property (spellbook, jewelry, crook) + Cast Speed runes | max **50%** combined |
| Quick Spell | 15% |
| Magic food (Quickspell) | 15% |

- **Total max: 75% faster.** The shortest cast is 0.25 s *(default)*.
- **In PvP every spell uses its base delay.** Teleport always does.
- You **can't move while casting**, except when casting from a wand.

### Recovery between spells

**0.75 s** after each spell.
In PvM, Casting Recovery (spellbook, jewelry, crook, runes) shortens it by up to **25%**.

## Mana cost

| Circle | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 |
|---|---|---|---|---|---|---|---|---|
| Mana | 4 | 6 | 9 | 11 | 14 | 20 | 40 | 50 |

- Summon Creature costs 35.
- **Wands** cost 2 mana per circle above the first (1st circle is free).
- **Lower Mana Cost** comes from items, PvM properties (spellbook, armor, clothing, jewelry, crook), Doom mastery and runes. It's capped at **40%**.
  PvM-only sources don't count in PvP.
- Monsters cast for free.

## Reagents and scrolls

- **Lower Reagent Cost** (PvM): spellbook, armor, clothing, jewelry, crook, Fortune mastery and runes. Up to **100%** chance to cast without reagents.
- **Scrolls first:** when you cast from your book and have a matching scroll in your backpack or mage satchel, the scroll is used instead of reagents.
  You can turn this off with the account option *ScrollsPrio*.
- Scrolls and wands never use reagents. Casting in a duel pit is free.
- Casting damage or summon spells wears down non-blessed spellbooks.

## Fizzling

- **100+ Magery never fizzles a Magery spell.** The same goes for 100+ Necromancy and Necromancy spells.
- Wands never fizzle.
- Below 100, the chance depends on the circle. Scrolls count as **two circles lower**.

| Circle | Skill for 0% | Skill for 100% |
|---|---|---|
| 1 | — | 3.6 |
| 2 | — | 17.9 |
| 3 | 3.6 | 32.1 |
| 4 | 17.9 | 46.4 |
| 5 | 32.1 | 60.7 |
| 6 | 46.4 | 75.0 |
| 7 | 60.7 | 89.3 |
| 8 | 75.0 | 103.6 |

## Spell damage

### 1. Base damage *(default)*

| Spell | Damage | | Spell | Damage |
|---|---|---|---|---|
| Magic Arrow | 4–7 | | Energy Bolt | 24–41 |
| Harm | 1–15 | | Explosion | 23–44 |
| Fireball | 10–16 | | Chain Lightning | 27–48 |
| Lightning | 12–20 | | Flame Strike | 27–48 |
| Mind Blast | 12–15 | | Meteor Swarm | 27–48 |

Necromancy spells have their own table. See [Necromancy](../magic/necromancy.md).

### 2. Skill scaling

```
Magery factor  = 1 + (Magery − 100) × 0.35%
Eval Int factor = 1 + (Evaluating Intelligence − 100) × 0.45%
damage = base × Magery factor × Eval Int factor
```

At 120/120: ×1.07 × ×1.09 = **×1.17**. At 100/100 damage is unchanged.

- **Evaluating Intelligence counts as 100 max in PvP.**
- **Necromancy** uses Necromancy in place of Magery, and **Spirit Speak + Eval Int added together** in place of Eval Int alone.

### 3. PvM bonus damage (player vs monster)

Every bonus below is added together and applied at once. **The total is capped at +500%.**

| Source | Bonus |
|---|---|
| **Baseline** | **+125%** on every spell against monsters |
| **Pure mage, no followers out** | +10% per circle for circles 1–3, **+25% per circle** for circles 4–8 (Flame Strike = +175%). Necromancy: +2.5% per point of required skill, max +225% |
| **Casting from a scroll** (50+ Inscription) | +2% per 10 Inscription, max +50% |
| **Spell Damage** property (armor, clothing, jewelry, crook) | +1% per point |
| **Spell-specific spellbook property** (Magic Arrow, Harm, Fireball, Lightning, Mind Blast, Energy Bolt, Explosion, Flame Strike) | +1% per point, max +100% |
| **Spell Damage Increase runes** | +1% per point |
| **Surge** | Focus/10 % chance (+ Surging property and runes) for **+30%** |
| **Tracking** | up to +20% at 120, +20% more on the creature you're tracking |
| **Slayer spellbook** | +20% against the matching type |
| **Boss Damage runes** | +1% per point against bosses |
| **Mage Killer runes** | +1% per point against spellcasting monsters |
| **Creature-type runes** | +1% per point against that type |
| **Grimoire spell scrolls** | +1% per scroll point, max 100 points (0.5% if you have 75+ Animal Taming) |
| **Wand + Item Identification** | 3% per 10 Item ID chance (max 40%) to echo: +100%, then 50% chance of another +50% |
| **Spell curse on monster** | + the curse amount |
| **Magic food (Surging)** | 35% chance for +25% |
| **Arcane Feast** | +10% |
| **Ankh necklace (Friendship)** | +10% near party or guild members |
| **Cartography** | up to +30% against Chest Guardians |
| **Guild boss buff** | +5% per level against bosses |
| **Rune Beetle pet** | +5% + 2.5% per stage (max +25%) |
| **Arcane Resonance pet mastery** | 5% / 7.5% / 10% per pet (max +60%) |
| **Masteries, Wizard stances, Druid stances, Doom sets** | see [Masteries](../masteries/index.md) and [Grimoire](../magic/grimoire.md) |

!!! tip "Spell Leech"
    Spell Leech (spellbook, clothing, runes, max 30%) is a % chance to heal yourself for the spell's mana cost.

### 4. Discordance and debuffs

- A **discorded** monster takes more spell damage and deals less (see [Discordance](instruments.md#discordance)).
- Greater paragons and danger-zone monsters take **30% less** spell damage.
- Monsters inside houses take no damage.

### 5. Resisting

If the target resists, the spell does **25% less damage**. This applies to monsters, and to players hit by other players.

```
resist chance = max(Resist / 5,  Resist − ((caster skill − 20) / 5 + circle × 5)) / 2
```

- In PvP, a target with 100+ Magic Resist gets **+10–15%** against 4th circle and higher.
- Against **monster** spells, players also add Magic Resist × 0.1%. Warriors (real weapon in hand) add their mastery bonus.

### Monster spells against players

Instead of the 25% resist, your defenses against creature spells add together:

| Source | Reduction |
|---|---|
| **Magic Resist** | 0.15% per point (15% at 100, 18% at 120) |
| **Heavy armor** | armor-based reduction |
| **Repeated hits (non-tamers, non-summoners)** | **+5% per spell hit** taken (max 25%), resets after 2 minutes without spell damage |
| Phoenix armor set | against fire spells |
| Fira / Doom / Oblivion masteries | see [Masteries](../masteries/index.md) |
| Runic curse on you | 15% **more** damage |

- All these reductions together are capped at **90%**.
- Monster **Explosion** is capped at **40** and monster **Mind Blast** at **25** against players.
- **Mind Blast** cast by a player on a player does +1 damage per medium armor piece and +2 per plate piece the target wears (6 pieces max).

### Pets casting in PvP

Pet spells against players are scaled by control slots: ×0.5 for 1 slot, ×0.75 for 2, full for 3+. They're also capped by spell and by a PvP maximum *(default)*.

### Pet and summon spell bonuses (PvM)

When your pet or summon casts on a monster, these add together:

| Source | Bonus |
|---|---|
| Pet **Intelligence** | more Int, more spell damage |
| **Follower Spell Damage** (runes, Shepherd's Crook) | capped *(default)* |
| **Herding** (and your crook's bonus) | +Herding ÷ 8 % plus the crook bonus, see [Shepherd's Crook & Herding](../pets/herding.md) |
| **Follower Boss Damage** (runes, crook) | against boss-sized monsters, capped *(default)* |
| Guild prestige buff *Pet Spell Damage* | +5% per level (Unchained pets) |
| Domination control points (Guild Militia) | creature or summon spell damage |
| Gravelord Crown / Spring Fae Bonnet | +5% per tier to matching summons |
| Fira mastery | bonus to pet Magic Arrow, Fireball, Explosion and Flame Strike |
| Mystic pets below stage 2 | +25% |
| Melting Spells relic | +25% for its charges, and consumes burning |
| Spell Venom relic | poisons the target (by the pet's Poisoning) |

## Magic Reflection

**Against monster spells**, players get a passive reflect chance:

```
reflect = Inscription × 0.1% + Magic Resist × 0.1% + Magic Reflection (armor, jewelry, runes) + Undine set + Macing codex
```

**Max 30%.** Bulwark mastery adds a separate reflect roll for mages.

The **Magic Reflect** spell absorbs (circle + 1) points per reflected spell until it runs out.

## Buffs and curses

**Bless, Strength, Agility, Cunning, Curse, Weaken, Clumsy, Feeblemind**:

```
amount   = 1 + Magery / 10           (11 at 100, 13 at 120)
duration = Magery × 1.2 s × (1 + Inscription / 200)
```

- Against players, Magery counts as 100 for duration. Above 100 it adds up to +10%.
- Inscription adds up to **+60%** duration at 120.
- In PvM, **Warding Resonance** (armor, clothing, runes) extends buff duration.
- A new buff replaces an old one only if it's stronger. A buff cast on a cursed target cancels part of the curse instead.

## Healing

These change how much your healing spells and abilities restore:

| Source | Effect |
|---|---|
| Ankh necklace (Cleric) | +15% |
| Cleric armor set (PvM) | set bonus |
| Magic food (Enhanced Healing), PvM | +10% |
| Cleric stance (Wizard) | +30% on pets, +20% on players |
| Holy mastery | scales with level |
| Summon Heal (spellbook), on summons | +1% per point |
| Target is a golem | half |
| Target is Berserked (PvM) | half |
| You are heal-cursed | half in PvM, −25% in PvP |

!!! warning "Paladins"
    Members of the Paladins guild take **15 damage** when they heal a criminal or murderer, except in contested regions.

## Summons

Summon duration scales with your casting skill:

```
duration × (1 + (skill − 100) / 200)
```

**Summon Surge** (spellbook property and runes) gives your summons a chance to surge when they hit monsters.
A surge heals 25% of their HP over 5 ticks and gives a +1 damage scalar (max 30).
Melee summons also get Quicksilver for 5 s. Casters get 5 empowered spells.

## Travel

You **can't recall or gate** when you are:

- a criminal,
- in combat,
- overloaded.

