# Traps

Two kinds of traps: **tinker traps** that players place, and **dungeon traps** hidden in the floor of dungeons.

## Tinker traps

### Placing a trap

Double-click a placeable trap in your backpack. Rules:

- You need **80 Tinkering or 80 Remove Trap**.
- You can only have **one trap placed** at a time, and only one trap can be in an area.
- Not in towns, guarded areas, safe zones or duel pits. Not near teleporters.
- In PvP you must dismount first.
- Placing takes 1.5 seconds, and you're frozen while you do it.
- **Cooldown:** 15 s, −0.25 s per point of Tinkering and Remove Trap above 100 (min 5 s).
- A trap lasts **5 minutes**, then disappears.

The trap is invisible. It goes off when a valid target **steps on it**. You never trigger your own harmful traps, and neither do your pets or your allies' pets.

### Range

| | Range |
|---|---|
| Against players | always 1 tile |
| Against monsters | by Tinkering + Remove Trap: under 200 = 1, 200+ = 2, 210+ = 3, 220+ = 4, 240 = 5 (+1 with Artisan mastery, max 6) |

You can turn off **PvP** for your traps in your options, so they never hit players.

### Trap types

| Trap | Effect |
|---|---|
| **Explosive** | Fire damage, and sets monsters **burning** |
| **Poison** | Poisons (Lesser, Regular at 75 Poisoning, Greater at 100, Deadly at 110) plus half damage |
| **Corpse** | Damage and **bleeding** |
| **Mortal Strike** | Mortal wound for 5 s (no healing) |
| **Bear Trap** | Freezes for 1 s, then slows to walking speed for 2 s |
| **Healing** | Heals whoever steps on it |
| **Curative** | Heals over 30 seconds (15 ticks) |
| **Hiding** | Hides whoever steps on it |
| **Surging** | Restores mana |

### Damage to monsters

A trap hits up to **5 monsters**, lowest HP first:

```
damage = trap base × (1 − 5% per tile from the trap)
         × (1 + skill bonuses)
         × (1 − 15% per extra monster hit)
         × tier reduction
```

- **Skill bonuses:** +0.75% per point above 100 in each of Tinkering, Remove Trap and Detect Hidden, +5% for each at 120, +2% per Artisan mastery level, + Trap Damage runes.
- **Tier reduction:** Hard −15%, Elite and Legendary −25%, Abomination and stronger **−75%**.
- **33%** of the damage lands right away. The other **66%** is dealt over 9 seconds (3 ticks).

| Trap | Base damage to monsters |
|---|---|
| Explosive | 650 |
| Corpse | 500 |
| Poison | 450 |
| Mortal Strike / Bear Trap | 150 |

### Damage to players

```
damage = 10 + 2 per point of Tinkering above 100 + 2 per point of Remove Trap above 100   (max 50)
```

The damage is **split** between every player in range.

### Healing traps

```
heal = 20–35 + (Tinkering + Healing) / 8      (+15 + 3 per Artisan level)
```

The amount is split between everyone in range.

## Dungeon traps

Dungeons have hidden floor traps.

### Spotting them

- Walking within 5 tiles gives you a **Detect Hidden %** chance to spot a trap.
- Using Detect Hidden on the area can also reveal them.
- Revealed traps hide again after about 10 seconds.

### Disarming them

Use **Remove Trap** on a trap within 2 tiles, or use its *Disarm* menu entry.

- Chance: **Remove Trap / 100**.
- A failed Remove Trap attempt has a 25% chance to set the trap off.
- A disarmed trap rearms after 10–12 seconds.

### Types

| Trap | Effect |
|---|---|
| Spike | 20–30 physical damage |
| Snow | 20–30 damage and a slow |
| Blood | Bleeding damage |
| Bone | Bone shards hitting everyone nearby for 10–15 each |
| Poison | 5–15 damage, Regular poison (30% chance Greater) |
| Lightning | 15–25 energy damage, 2 s paralyze |
| Disease | Disease damage over time, getting weaker each tick |

A trap can only go off once every 5 seconds.
