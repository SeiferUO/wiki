# Meta Relics

**Creature Ability Relics** teach abilities to [Unchained pets](unchained.md). Target your pet with a relic from your backpack to teach it. Rules for learning (lineage match, 2 relics per pet, dragon limits) are on the [Unchained Pets](unchained.md#relic-abilities) page.

## How relics fire

A relic fires when the pet fights, if its cooldown is ready and a roll succeeds.

**Chance per attempt:**

| Relic type | Base chance |
|---|---|
| Single-target attacks | 25% |
| Area attacks, debuffs and self-buffs | 15% |

- **+1% per pet stage** (up to +10%).
- **+10%** while the pet is stage 5 or lower.
- **−10%** if the pet has more abilities than control slots.

**Cooldown:** every relic shares the same base cooldown, **50 seconds − 0.5 s per relic level** (45 s at level 10). The pet's own cooldown reduction then applies (Dex, control slots, stage and the Ability Cooldown mastery; see [Cooldowns](unchained.md#cooldowns)).

**Damage:** a relic hit is based on one of the pet's melee hits:

```
damage = pet melee hit × control slots
         + 5% per relic level
         + Intelligence ÷ 25 (÷ 35 for 1-slot pets)
```

Then:

| Modifier | Effect |
|---|---|
| Ability Power mastery | +5 / 10 / 15% |
| Molten pet vs a **burning** target | +50% (uses up the burn) |
| Assassin class | +25% |
| Stage 17+ | +15% |
| Shepherd's crook *Creature Ability Damage*, PvM rune *Follower Ability Damage* | +their % |
| Area relic on a 1-slot pet | half damage |
| Damage-over-time ticks | ⅕ damage per tick |
| More abilities than control slots | −25% |

The **reach** of most area relics grows with the pet's control slots (for example Tempest hits within 3 tiles per slot, Splash looks 4 tiles per slot).

## Relics by lineage

### Molten

| Relic | Effect |
|---|---|
| Angry Fire | Fire damage to the target, with a chance to ignite it. |
| Engulf | Expanding fire rings around the target: fire damage to nearby enemies, chance to ignite. |
| Explosion | Expanding fire bursts around the pet hit all nearby enemies. |
| Fire Orb | Surrounds the pet with an infernal shield for a short time. |
| Firecannon | A rapid barrage of fire shots (2 per control slot). Each shot deals 20% less than the one before. |
| Hell Burst | Fire damage to the target and up to 5 nearby enemies. |
| Inferno | Fire damage in decaying ticks; chance to ignite (10% per relic level). |
| Melting Spells | Charges the pet's spells: **5 + control slots + level ÷ 3** charges. Each charged spell deals **+25% damage** and detonates a burning target. |
| Meteors | A meteor shower around the target hits several nearby enemies. |
| Molten Fire | Fire strike on the target, then scattered strikes nearby that can set the ground on fire. |
| Raging Breath | Fire breath in a straight line, hitting everything in its path. |
| Swarm | Fireballs at up to 3 nearby enemies at once. |

### Aero

| Relic | Effect |
|---|---|
| Chill | Cold damage and slower attacks. Hits twice if the target is already chilled. |
| Crystalize | Slows the target and deals cold damage in ticks to nearby enemies. |
| Frozen Touch | Cold damage and slower attacks for a few seconds. |
| Lightning Force | Freezes the target, then several decaying energy strikes. |
| Quicksilver | Buff: more Dexterity and full stamina (faster attacks). |
| Sharp Thoughts | Buff: faster casting and full mana. |
| Splash | Cold shards at the 3 closest enemies, one after another. |
| Tempest | Energy damage to nearby enemies, paralyzing each for a few seconds. |
| Velocity | Buff: shorter cooldowns on all abilities and full stamina. |
| Water Spout | A water spout erupts outward: cold damage to all nearby enemies. |

### Blood

| Relic | Effect |
|---|---|
| Blood Disease | Bleeds the target, with a chance to spread to nearby enemies. |
| Blood Frenzy | Consumes blood on the ground nearby for faster attacks. |
| Blood Healing | Consumes blood on the ground nearby to heal. More blood heals more. |
| Blood Rage | Buff: better accuracy. |
| Bloody Talons | Physical damage to the target and nearby enemies, bleeding each. |
| Expunge | Several waves of blood damage against nearby enemies. |
| Life Drain | Drains life from the target and nearby enemies and heals the pet for the damage. |
| Regeneration | Heals the pet over several ticks. |
| Sacrifice | Spends some of the pet's HP to deal damage. Higher levels cost less HP. |
| Savagery | Buff: more melee damage. |
| Spell Leech | Buff: the pet heals whenever spells hit it. |

### Death

| Relic | Effect |
|---|---|
| Agonization | Physical damage in decaying ticks. |
| Baneful Strike | Several strikes of cold, energy and poison damage. Each deals 15% less than the one before. |
| Blinding Strike | Physical damage and blinds the target (lower accuracy). |
| Death Touch | Poison and energy damage; strikes again for bonus damage on low-HP targets. |
| Disease | A spreading poison damage-over-time. |
| Doom | Curses the target; a heavy cold and energy burst hits it 5–7 seconds later. |
| Fade | Buff: the pet turns semi-transparent and evades melee attacks. |
| Witch Brew | Damages nearby enemies and heals the pet's master and allied creatures nearby. |
| Wither | Cold, poison and energy damage to nearby enemies. |

### Earth

| Relic | Effect |
|---|---|
| Charge | Dashes to a target within 7 tiles for fire damage, then bursts on everything within 2 tiles. |
| Cleave | Physical damage to every enemy in melee range. |
| Colossal Blow | Physical damage and freezes the target for a few seconds. |
| Concentration | Buff: better accuracy. |
| Confusing Blow | Poison damage and silences the target's spellcasting. |
| Crushing Blow | Physical damage and lowers the target's armor briefly. |
| Double Strike | An extra physical strike. |
| Earth Shield | Buff: shields the pet from certain abilities used against it. |
| Genesis | Heals the pet; heals more when it's badly hurt. |
| Grasping Claw | Physical damage and bleeding. If the target already bleeds, it also pierces its defenses. |
| Massacre | Several fire strikes; more strikes the more hurt the pet is. |
| Repel | Damages the target. Only works while Earth Shield is down. |
| Taunt | Nearby enemies (3 tiles per control slot) switch to the pet, and it gains physical and magic resistance for 7 seconds (more at higher stages, up to +50%). |
| Vigor | Refills stamina for the pet, its master and nearby allied creatures. |

### Mystic

| Relic | Effect |
|---|---|
| Blast | Energy damage and lowers the target's magic resistance. |
| Calming Touch | Pacifies the target. Deals damage if it's already pacified. |
| Clarity | Buff: full mana and bonus Intelligence (more spell power). |
| Conductive Blast | Energy damage and a short freeze. |
| Eldritch Shield | Buff: reflects all spells cast at the pet. |
| Empowerment | Buff: the pet's next few spells deal +25% damage. |
| Mana Drain | Restores the pet's mana. Only fires when its mana isn't full. |
| Mystic Blast | Waves of arcane energy around the pet. |
| Runic Curse | Lowers the target's magic resistance by 15% for a few seconds. |
| Teleport | Teleports to a target within 12 tiles and hits it and everything within 2 tiles. |

### Noxious

| Relic | Effect |
|---|---|
| Intoxicate | Poison damage; disorients the target if its HP is low. |
| Manticore Venom | Marks the target; a heavy poison burst hits it 5–7 seconds later. |
| Paralytic Venom | Poisons the target and slows its attacks. |
| Poison Cloud | A poison cloud damages and poisons nearby enemies. |
| Poison Spit | Several barrages of poison projectiles; each hit poisons. |
| Poison Strike | Poison damage and lowers the target's poison resistance. |
| Root | Poison damage and freezes the target. Bonus damage if it's already frozen. |
| Spell Venom | Buff: the pet's spells also poison. |
| Targeted Weakness | Poison damage; hits twice if the target is already poisoned. |
| Venomous Blood | Blood projectiles in a ring: poison and physical damage to nearby enemies. |

### Dragon relics

Only dragons can learn these. A dragon can have **one wave** and **one breath or barrage**, counting innate abilities.

| Relic | Lineage | Kind | Effect |
|---|---|---|---|
| Molten Wave | Molten | Wave | Fire cone, 2 tiles long per control slot. |
| Glacial Wave | Aero | Wave | Cold cone, 2 tiles long per control slot. |
| Blood Wave | Blood | Wave | Physical cone, 2 tiles long per control slot. |
| Earth Wave | Earth | Wave | Physical cone, 2 tiles long per control slot. |
| Shockwave | Mystic | Wave | Energy damage to the target and enemies around the pet (1 tile per control slot), freezing them. |
| Magma Breath | Molten | Wave | Fire breath. |
| Molten Barrage | Molten | Barrage | 2 fire projectiles per control slot; can set the ground on fire. |
| Blood Barrage | Blood | Barrage | 2 blood projectiles per control slot. |
| Eldritch Barrage | Mystic | Barrage | 2 eldritch projectiles per control slot. |
| Earth Blast | Earth | Breath | 3 earth blasts at the target. |
| Snow Breath | Aero | Breath | Cold breath over an area. |
| Shadow Breath | Death | Breath | Poison and energy cone, 2 tiles long per control slot. |
| Swamp Breath | Noxious | Breath | Poison cone that leaves poison fields. |

The dragon pauses for 1–2 seconds while using a wave, breath or barrage.
