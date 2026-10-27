# Necromancy Spells

The shard's necromancy is a custom PvM spell school with 14 spells, its own damage table and a mastery tree.

!!! warning "PvM only"
    Necromancy spells only work against monsters (buffs work on you, friendly players and your pets).
    In PvP, the Necromancy skill still adds up to **+10% spell damage** to your other spells (+1% per 10 points).

!!! note
    Numbers marked *default* come from the Necromancy Spell Damage controller and can be changed by staff.

## How necro damage scales

Necromancy uses its own skills in place of Magery and Evaluating Intelligence:

```
Necromancy factor  = 1 + (Necromancy − 100) × 0.35%
Spirit Speak factor = 1 + (Spirit Speak − 100) × 0.35%
Eval Int factor     = 1 + (Eval Int − 100) × 0.45%

damage = base × Necromancy factor × (Spirit Speak factor + Eval Int factor)
```

Because Spirit Speak and Eval Int are **added together**, a necromancer with 100 in all three deals **double** the base damage.

All the PvM spell bonuses from [Spellcasting](../core/spellcasting.md#3-pvm-bonus-damage-player-vs-monster) apply on top, including the +125% baseline.
A pure caster with no followers gets **+2.5% per point of the spell's required skill** (max +225%).

### Casting

- Casting time is fixed per spell (the "Cast" column). Faster-cast items don't shorten it.
- Mana cost is fixed per spell.
- **100+ Necromancy never fizzles.** Below that, you need the required skill, and 100% success comes at required skill + 40.
- Scrolls use the required skill as both minimum and maximum.

## Spell list *(default)*

| Spell | Skill | Mana | Cast | Base damage | Type |
|---|---|---|---|---|---|
| [Animate Dead](#animate-dead) | 30 | 25 | — | — | Summon |
| [Bone Armor](#bone-armor) | 40 | 20 | — | — | Self shield |
| [Mind Rot](#mind-rot) | 40 | 10 | 4 s | 8–18 per tick | Channel |
| [Evil Omen](#evil-omen) | 50 | 15 | — | — | Buff |
| [Siphon Blood](#siphon-blood) | 50 | 12 | 3 s | 8–15 | Area + heal |
| [Pain Spike](#pain-spike) | 60 | 15 | 3 s | 15–30 | Single target |
| [Insect Swarm](#insect-swarm) | 60 | 15 | 6 s | 8–18 per tick | Damage over time |
| [Iron Maiden](#iron-maiden) | 70 | 20 | 8 s | — | Buff |
| [Exorcism](#exorcism) | 70 | 20 | 8 s | — | Heal |
| [Poison Strike](#poison-strike) | 70 | 20 | 4 s | 20–40 | Single target + poison |
| [Bone Cleave](#bone-cleave) | 75 | 25 | 5 s | 25–50 | Cone |
| [Corpse Explosion](#corpse-explosion) | 80 | 25 | 5 s | see spell | Area |
| [Wither](#wither) | 85 | 30 | 8 s | 25–50 | Area around you |
| [Vampiric Embrace](#vampiric-embrace) | 90 | 35 | 10 s | 20–40 | Single target + heal |

## Damage spells

### Pain Spike

A single hit that grows stronger as the target gets weaker.

```
damage × (1.5 − target's HP %)
```

×1.5 against a nearly dead monster, ×0.5 against one at full health.

### Vampiric Embrace

- Above 50% HP it's a plain damage spell.
- **Below 50% HP** it heals you for 50% + Spirit Speak / 400 of the damage dealt (80% at 120). **Max 35 HP** per cast.

### Poison Strike

Hits the target. Then:

- **If the target isn't poisoned**, it's poisoned based on your **Poisoning** skill: Lesser below 40, Regular 40+, Greater 60+, Deadly 80+, Lethal 100+.
- **If it's already poisoned**, the poison **spreads** to nearby monsters that aren't poisoned.
  Radius 2 + Spirit Speak / 40 (max 5). Up to 1 + Spirit Speak / 25 extra targets (max 5).

### Bone Cleave

A 60° cone in the direction you target.

- Range: 3 + Spirit Speak / 40 tiles (max 6).
- Targets: 3 + Spirit Speak / 33 (max 6).
- **−10% damage per tile** away from you (min 50%).

### Wither

Hits monsters around you, closest first.

- Range and max targets: 3 + Spirit Speak / 33 (6 at 100).
- **−15% damage per tile** away from you (min 10%). Best used point-blank.

### Siphon Blood

Damages monsters around a targeted spot and heals you.

- Radius: 2 + Spirit Speak / 40 (max 5). Hits as many monsters as the radius.
- Heal: total damage / (10 − radius) + Necromancy / 20.

### Corpse Explosion

Target a corpse, or yourself to pick the closest one. It detonates and hits monsters around it.

- Damage: **20 + Necromancy / 5** (44 at 120), less the further a monster is from the corpse.
- Radius: 3 + Spirit Speak / 50.
- A corpse can only be exploded once every 10 s.

## Damage over time

### Mind Rot

Channels damage every second for **10 ticks**.

- **You must stand still**, keep line of sight and stay within 12 tiles, or it breaks.
- Mana per tick: 12 − Spirit Speak / 20 (min 3).
- Each tick does 5% less than the last (min 50%).
- Casting it again replaces your current Mind Rot.

### Insect Swarm

Damage every second.

- Ticks: 5 + Spirit Speak / 20 (max 10).
- Each tick does 8% less than the one before.
- **Recasting on a swarmed target** deals one full burst of damage and starts a fresh swarm.

## Buffs and shields

### Bone Armor

A damage shield on yourself.

```
shield = min(125, 25 + (Spirit Speak + Necromancy) / 2) × (1 + Inscription / 400)
```

At 120/120/120: 125 × 1.3 = **162 HP**. Duration: 20 + Spirit Speak / 3 seconds (60 s at 120).

### Evil Omen

Buffs **you and all your pets within 18 tiles**.

- Bonus damage: **10% + Necromancy / 5 %** (34% at 120).
- Each hit has a 25% chance to hurt the attacker for 50% of the bonus damage.
- Duration: (30 + Spirit Speak / 2) × (1 + Inscription / 400) seconds.

### Iron Maiden

Cast on yourself, a friendly player or a pet. When a monster hits them, part of the damage is reflected back at the monster.

- Reflect: **30% + Necromancy / 4 %**.
- Duration: (20 + (Spirit Speak − target's Magic Resist) / 5) × (1 + Inscription / 400) seconds.

## Corpse spells

### Exorcism

Consume a corpse (or target yourself for the closest one within 8 tiles) to heal.

- Heal: **8% of the creature's max HP × (1 + Spirit Speak / 300)**. Min 5, max 40.
- ×1.5 when you're below 50% HP (still max 40).
- Your pets within 15 tiles are healed for **twice** that (max 80).
- Carved corpses can't be used.

### Animate Dead

Raise a monster corpse (or the closest one, if you target yourself) as a temporary minion.

- Duration: **4 × Necromancy + 2 × Spirit Speak** seconds.
- It takes 2 control slots, or more if you have free slots (up to 3 while mounted with no followers).
- Carved corpses, player corpses and pet corpses can't be animated.

## Necromancy mastery

Killing monsters gives Necromancy XP. XP earns mastery points to spend on upgrades.

```
XP for the n-th point = 800 × n + 2 × (n − 1)²
```

| Upgrade | Per tier | Max tier | Cost of tier 1 |
|---|---|---|---|
| Pain Spike Power | +10% damage | 5 | 2 |
| Mind Rot Channeling | +1 tick, −1 mana per tick | 3 | 1 |
| Corpse Explosion Radius | +1 tile | 3 | 2 |
| Poison Strike Spread | +1 spread target, 20% chance for a stronger poison | 5 | 1 |
| Siphon Blood Power | +5% healing | 5 | 1 |
| Insect Swarm Duration | +1 tick | 3 | 1 |
| Wither Power | +10% damage | 3 | 3 |
| Bone Cleave Targets | +1 target | 5 | 2 |
| Vampiric Embrace Power | +5% lifesteal | 3 | 3 |
| Iron Maiden Reflection | +5% reflect | 3 | 2 |
| Evil Omen Power | +5% damage, −2.5% self-damage chance | 3 | 3 |
| Exorcism Healing | +5% healing | 3 | 2 |

Each tier costs 1 point more than the one before. Resetting your points costs **100 gold per point spent**.
