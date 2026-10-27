# Unchained Pets

**Unchained pets** are the shard's leveling tamables. They grow through stages, learn relic abilities, unlock masteries and can be [bred](breeding.md).

For basic taming and control rules, see [Taming](../skills/taming.md). For every pet's slots, class and abilities, see the [Unchained Pet List](unchained-list.md).

## Lineages

Every Unchained pet belongs to one or more **lineages**: **Molten, Aero, Blood, Death, Mystic (Nova), Earth** or **Noxious**. The lineage decides which relics the pet can learn, what food it eats and how it breeds.

| Lineage | Favorite food |
|---|---|
| Molten | Meat |
| Aero | Fruits and vegetables |
| Blood | Meat |
| Death | Meat |
| Mystic | Grains and hay |
| Earth | Eggs |
| Noxious | Fruits and vegetables |

## Roles

Each species has a **role** that sets its starting stats and how it grows.

| Role | Starting Str / Dex / Int (× slots) | Gains per stage, per control slot |
|---|---|---|
| Tank | 115 / 35 / 35 | Str +12, Dex +6, Int +6 |
| Mage | 75 / 35 / 75 | Str +8, Dex +4, Int +12 |
| Bruiser | 95 / 35 / 55 | Str +12, Dex +4, Int +8 |
| Assassin | 95 / 50 / 40 | Str +8, Dex +8, Int +8 |
| Dragon | 100 / 35 / 50 | Str +10, Dex +4, Int +10 |

- Starting stats roll up to ±10 around those bases.
- A new pet starts with **100 HP per control slot**, 10 armor per slot, and 5–7 damage per slot (mages 3–5 per slot).
- Every stage also adds +1 min damage, +1–2 max damage, +1 armor and +2.5% poison resist.
- **Assassins** get shorter ability cooldowns.

## Stages

Pets gain XP from monsters they help kill. The max stage is **10**. After that, XP goes into [masteries](#masteries).

| Stage | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
|---|---|---|---|---|---|---|---|---|---|---|
| XP needed | 10,000 | 25,000 | 75,000 | 250,000 | 500,000 | 750,000 | 1,000,000 | 1,500,000 | 2,000,000 | 2,500,000 |

That's about **8.6 million XP** from a new pet to stage 10.

### Skill requirements

To **evolve** to the next stage, you need **Animal Taming and Animal Lore** at:

| Current stage | Skill needed |
|---|---|
| 0–5 | 50 + 10 × stage |
| 6–8 | 100 + 5 × (stage − 5) |
| 9+ | 120 |

The pet's **taming requirement** also rises as it grows: 50, 50, 60, 70, 80, 90, 100, 105, 110, 115 and 120 for stages 0 to 10.

### What a stage gives

| Stage | Bonus |
|---|---|
| 1 | The pet becomes **bonded** |
| 2 | +1 ability slot |
| 4 | +1 ability slot (2+ control-slot pets only) |
| every stage | stat gains (see [Roles](#roles)) |

### XP bonuses

XP per kill is capped at **3,500**. Bonuses:

- **+10%** if the pet has never been bred.
- **Hunger:** up to **+10%** at full hunger.
- **Tamer skill:** +0.25% per point above 100 in Animal Taming, Animal Lore and Herding (max **+15%** at 120 in all three).

**Vials of Pet XP** add XP directly.

## Relic abilities

Abilities come from **Creature Ability Relics**. Target your pet with a relic from your backpack to teach it.

- The relic's lineage must **match one of the pet's lineages**.
- A pet can hold **2 relics** at most, and needs a free ability slot (see [Stages](#what-a-stage-gives)).
- **Dragon relics** only work on dragons. A dragon can have only **one wave** and **one breath/barrage** ability, counting innate ones.
- Relics level **1 to 10**. A relic gains 1 XP each time it fires on a monster. The next level needs 200 × the current level.

### Relics by lineage

See [Meta Relics](relics.md) for what each relic does, its chance to fire and its damage.

| Lineage | Relics |
|---|---|
| Molten | Angry Fire, Engulf, Explosion, Fire Orb, Firecannon, Hell Burst, Inferno, Melting Spells, Meteors, Molten Fire, Raging Breath, Swarm |
| Aero | Chill, Crystalize, Frozen Touch, Lightning Force, Quicksilver, Sharp Thoughts, Splash, Tempest, Velocity, Water Spout |
| Blood | Blood Disease, Blood Frenzy, Blood Healing, Blood Rage, Bloody Talons, Expunge, Life Drain, Regeneration, Sacrifice, Savagery, Spell Leech |
| Death | Agonization, Baneful Strike, Blinding Strike, Death Touch, Disease, Doom, Fade, Witch Brew, Wither |
| Earth | Charge, Cleave, Colossal Blow, Concentration, Confusing Blow, Crushing Blow, Double Strike, Earth Shield, Genesis, Grasping Claw, Massacre, Repel, Taunt, Vigor |
| Mystic | Blast, Calming Touch, Clarity, Conductive Blast, Eldritch Shield, Empowerment, Mana Drain, Mystic Blast, Runic Curse, Teleport |
| Noxious | Intoxicate, Manticore Venom, Paralytic Venom, Poison Cloud, Poison Spit, Poison Strike, Root, Spell Venom, Targeted Weakness, Venomous Blood |
| Dragon only | Blood Barrage, Blood Wave, Earth Blast, Earth Wave, Eldritch Barrage, Glacial Wave, Magma Breath, Molten Barrage, Molten Wave, Shadow Breath, Shockwave, Snow Breath, Swamp Breath |

### Cooldowns

A relic's **base cooldown** is 50 seconds, 0.5 s shorter per relic level. Your pet then cuts it further with:

- **1 s per 100 Dex**,
- **1 s per control slot** (another 1 s per slot for Assassins and for Velocity),
- **0.5 s per stage**.

That reduction is capped at **9 seconds**. A pet with **more abilities than control slots** loses almost all of it.

Last, the **Ability Cooldown** mastery takes another 5/10/15% off what's left.

## Masteries

Once your pet reaches **stage 10**, its XP earns **mastery points**, up to **100** in total.

```
XP for mastery point n = (floor((n − 1) / 7.5) + 1) × 25,000
```

Each mastery has **3 tiers**. Tier 1 costs 1 point, tier 2 costs 2 more and tier 3 costs 3 more, so a maxed mastery takes **6 points**.

!!! note "Damage cap"
    Damage masteries (marked ⚔) share a cap of **10 tiers** in total.

| Mastery | Tier 3 effect |
|---|---|
| Evasion | 6% chance to evade attacks |
| Savagery ⚔ | +15% melee damage |
| HP Regen | 3 HP per second in combat |
| Mana Regen | 3 mana per second in combat |
| Stamina Regen | 6 stamina per second in combat |
| Precision | +15% hit chance |
| Eldritch Power ⚔ | +30% spell damage |
| Predator ⚔ | +15% damage to isolated creatures |
| Mage Killer ⚔ | +15% damage to casters |
| Absorption | 7.5% of damage taken returned as HP |
| Poison / Bleed / Disease Immunity | +20% immunity |
| Paralysis / Curse Immunity | Immune (−33% / −66% duration at tiers 1–2) |
| Counter Attack | 15% chance to counter-strike |
| Influencer ⚔ | Barded foes take +10% damage |
| Humanoid Killer ⚔ | +15% damage to humanoids |
| Ability Power | +15% relic ability damage |
| Ability Cooldown | −15% relic cooldowns |
| Healing Received | +20% healing received |
| Tank Fortitude | +10% resists in Tank stance |
| Ranged Fury ⚔ | +30% ranged attack damage |
| Increased Min / Max Damage ⚔ | +6 min / max damage per swing |
| Herding Efficiency ⚔ | +7.5% herding efficiency |
| Hits Bonus | +10% max HP |
| Spell Surging ⚔ | 7% chance for +35% spell damage |
| Critical Strike ⚔ | 7% chance for +35% melee damage |
| Bleed / Disease / Poison Damage ⚔ | +10% damage to bleeding / diseased / poisoned targets |
| Additional Poison Tick | 20% chance for +1 poison tick |
| Bard Stuck | 5% chance to hypnotize foes |
| Reflect Chance | 7.5% chance to reflect spells |
| Hunting Party ⚔ | +15% damage when next to you |
| Immolate ⚔ | +15% damage to burning targets |
| Menagerie ⚔ | +10% damage from pet diversity |
| Shadow Strike ⚔ | +35% stealth strike damage |
| First Strike ⚔ | +30% damage to full-health targets |
| Pack Synergy ⚔ | +12% pack instinct efficiency |
| Arcane Resonance | You gain +10% spell damage |
| Spell Power ⚔ | +15% Magery spell damage |
| Mana Reclaim | Recover 6% mana per cast |

## Hunger and bonding

### Hunger

- Hunger runs from **0 to 100**. It drops by **2 every 10 minutes**.
- Feed your pet **Unchained pet food** of its favorite type. Each food restores **25 hunger**.
- A well-fed pet deals up to **+10% damage** and earns up to **+10% XP**.

### Bonding

Pets build **bonding XP** from kills (at most one gain every 15 seconds).

- Every **1.5 million** bonding XP gives **+1% damage**, up to **+10%** at 15 million.
