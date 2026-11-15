# Grimoire

The **Grimoire of Mastery** lets mages upgrade individual Magery spells with points earned from killing monsters.
Upgraded spells gain extra effects in PvM.

!!! note
    Numbers on this page are *default* values from the Grimoire Mastery controller and can be changed by staff.
    Some effects are weaker for characters who aren't mages (under 150 combined Magery, Meditation, Spirit Speak, Eval Int, Mysticism and Focus).

## Points

- Killing monsters gives Grimoire XP.
- XP for the n-th point: **800 × n + 2 × (n − 1)²**.
- Double-click the Grimoire to spend points. Each spell has **3 tiers**:

| Tier | Cost |
|---|---|
| 1 | 2 points |
| 2 | 3 points |
| 3 | 4 points |

A fully upgraded spell costs 9 points. You can reset your points for gold.

## Attack spells

| Spell | Tier 1 | Tier 2 | Tier 3 |
|---|---|---|---|
| **Magic Arrow** | 300% damage, 60 s cooldown; [Arcane Mark](#combos) | 300% damage, 40 s cooldown | 300% damage, 20 s cooldown |
| **Harm** | 300% damage, 60 s cooldown; below 33% health: [Execute](#combos) | 40 s cooldown | 20 s cooldown |
| **Fireball** | 10% chance to burn (10 damage over 5 s) | 12 fire-rain meteors | 4 fire fields |
| **Lightning** | +10% damage, 5% chance to hinder; [Static](#combos) | +20% damage, 10% to hinder | +30% damage, 15% to hinder, every 4th Lightning arcs |
| **Mind Blast** | +15% mana damage, +15% vs melee monsters, mage monsters −10% damage for 2 s | +20% / +30% / −15% for 2.5 s | +25% / +45% / −25% for 3 s |
| **Energy Bolt** | chains to up to 5 more monsters within 6 tiles, sharing its damage; [Overload](#combos) +25% vs frozen, paralyzed or rooted targets | same, +50% | same, +75% |
| **Explosion** | also hits 2 monsters within 3 tiles for 25% of its damage; [Detonate](#combos) | 4 monsters within 4 tiles, 50% | 6 monsters within 5 tiles, 75%, 33% chance of fire fields |
| **Chain Lightning** | range 3, +25% damage | range 4, +50%, 1 storm vortex | range 5, +75%, 2 storm vortexes |
| **Flame Strike** | a line of fire from you to the target hits monsters on it | + 25% chance per tile to leave fire fields | + explosions along the line |
| **Poison** | 25% chance to raise the poison level | 25% chance to spread to 5 targets within 3 tiles | +25% poison damage |
| **Fire Field** | +25% damage to monsters | + extra fire layers around the wall (3×3) | 5×5 layers |
| **Poison Field** | stronger poison | stronger, + extra layers (3×3) | strongest, 5×5 layers |

## Curses (on monsters)

| Spell | Tier 1 | Tier 2 | Tier 3 |
|---|---|---|---|
| **Curse** | target takes +15% spell damage for 4 s | +25% for 6 s | +35% for 8 s |
| **Clumsy** | −15% attack and cast speed for 3 s | −25% for 4 s | −35% for 5 s |
| **Feeblemind** | −20% spell damage for 5 s | −35% for 7 s | −50% for 10 s |
| **Weaken** | −15% to −35% Strength for 8 s (more against stronger monsters) | −25% to −55% for 12 s | −35% to −75% for 16 s |
| **Paralyze** | paralyzes 3 monsters within 3 tiles for 3 s; [Brittle](#combos) | 5 within 4 tiles | 8 within 5 tiles |

## Buffs and utility

| Spell | Tier 1 | Tier 2 | Tier 3 |
|---|---|---|---|
| **Heal** | +10% healing | +20% | +30% |
| **Greater Heal** | +10% healing | +20% | +25% |
| **Protection** | shield absorbs 250 damage | 350 | 500 |
| **Reactive Armor** | damage aura for 3 s | 6 s | 8 s |
| **Magic Reflect** | 3% passive reflect | 6% | 9% |
| **Agility** | melee evasion against you −5% for 10 s | −10% for 15 s | −15% for 20 s |
| **Strength** | +5% melee critical chance for 10 s | +10% for 15 s | +15% for 20 s |
| **Cunning** | +5% spell surge chance for 10 s | +10% for 15 s | +15% for 20 s |
| **Teleport** | 15 damage to monsters within 1 tile of where you land | 20 damage within 2 tiles | 25 damage within 3 tiles |

Non-mages get half the effect from Agility and Cunning, and less healing.

The extra field layers need an active mage mastery and don't work in duels.

**Mages without followers** (no summons, pets or golems out) get twice the Magic Arrow and Harm bonus damage on half the cooldown, twice the chance for Lightning to hinder, and after an Explosion their next spell on the same target deals **+25% per tier** (within 15 s).

A **hindered** monster (Lightning) is frozen for 2 / 3 / 4 s (half as long for tough monsters) and can't be hindered again until 10 s after it ends.

## Combos

Upgraded spells also set each other up. Cast them in the right order for extra damage. These only work on monsters, never in PvP or duels, and characters who aren't mages get **half** of each bonus.

| Combo | Spell | How it works |
|---|---|---|
| **Arcane Mark** | Magic Arrow | Each Magic Arrow marks the monster (up to **5 marks**, for 15 s). Your next *other* damaging spell on it uses all the marks: **+5 / 8 / 10% damage per mark** (tier 1 / 2 / 3), so up to +50%. |
| **Brittle** | Paralyze | Monsters you paralyze become Brittle. Your next damaging spell on them deals **+20 / 35 / 50%** and shatters the freeze. |
| **Execute** | Harm | Below **33% health**, every Harm deals **+75 / 125 / 175%** of its damage, with no cooldown. If it kills the monster, you get **5 / 7 / 9 mana** back. |
| **Overload** | Energy Bolt | **+25% per tier** against anything frozen, paralyzed or rooted (by Paralyze, Lightning's hinder...). |
| **Static** | Lightning | Each Lightning on the same monster within 8 s adds a stack (up to 5). Each new Lightning deals **+10% per stack** already built, so up to +50%. At **tier 3**, every 4th Lightning on the same monster arcs to up to 6 monsters around it for half its damage. |
| **Detonate** | Explosion | On a **burning** monster the fire bursts: up to **5 / 6 / 7** monsters within **3 / 4 / 5 tiles** take **50 / 75 / 100%** of the Explosion's damage, and each has a **50 / 65 / 80%** chance to catch fire, ready for the next Explosion. |

A few combos to try:

- **Magic Arrow ×5 → Energy Bolt or Lightning:** spend five marks on a big spell.
- **Paralyze → Energy Bolt:** Brittle *and* Overload on the same bolt.
- **Lightning, Lightning, Lightning...:** Static builds up the longer you stay on one monster.
- **Fireball or Explosion to set a pack on fire → Explosion:** Detonate spreads the fire through the pack.
- **Finish with Harm** once a monster is under a third of its health.

## Spell scrolls bonus

Separately from the Grimoire, mages build up per-spell **scroll mastery** for Fireball, Flame Strike, Explosion, Lightning, Mind Blast, Energy Bolt, Magic Arrow, Poison and Harm.
Each point gives **+1% PvM damage** with that spell, up to 100 points (+0.5% if you have 75+ Animal Taming).
