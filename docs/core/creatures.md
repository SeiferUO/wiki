# Creatures

How monsters are built, how they fight, and how pets and summons work underneath.

!!! note
    Numbers marked *default* come from in-game balance controllers and can be changed by staff.
    Pet breeding and Unchained pets have their own pages under [Pets](../pets/breeding.md).

## Monster or follower?

A creature is a **monster** when nobody controls or summoned it. Pets and summons are **followers**.
Most PvM bonuses on this wiki only work against monsters.

## Difficulty tiers

Every monster belongs to a difficulty tier based on its maximum HP. From weakest to strongest:

**New → Easy → Medium → Hard → Elite → Legendary → Abomination → Mini-boss → Expedition (Easy / Medium / Hard) → Doom → Community → Dungeon boss → Champion → Harrower**

The tier sets a monster's stats, damage, armor, skills, parry, accuracy, poison resistance, Fame/Karma and how fast it moves.
These values, and the HP that decides each tier, are set by staff in the Creature Attribute controller and can change in game.

- Str, Dex, Int and damage are rolled **±10%** around the tier's values. Skills are capped at 150.
- **Mage monsters** get 70% Strength and 80% damage. Melee monsters get 65% Intelligence.
- Archers always have 100 Archery.
- Fame and Karma are randomly ×0.5, ×1 or ×2 the tier's value.

### Detect Hidden

Tougher monsters find stealth players more easily:

| Tier | Detect Hidden |
|---|---|
| New | 20 |
| Easy | 35 |
| Medium | 50 |
| Expedition (Easy) | 60 |
| Hard | 65 |
| Elite, Expedition (Medium) | 75 |
| Legendary, Mini-boss | 80 |
| Expedition (Hard) | 90 |
| Dungeon boss | 100 |
| Abomination, Community | 110 |
| Champion | 115 |
| Doom, Harrower | 120 |

### Sight range

| Tier | Notices you from |
|---|---|
| Below Hard | 6 tiles |
| Hard | 8 tiles |
| Elite | 10 tiles |
| Legendary | 12 tiles |
| Abomination and above | 15 tiles |

### Movement speed

Stronger tiers move faster. Some things slow monsters down:

- **Slowed:** 60% slower.
- **Disoriented:** slower by the disorient amount.
- Monsters stronger than Legendary are 35% slower in regions where mounts aren't allowed.
- A monster can never be slowed to less than 40% of its normal speed.

## How monsters hit you

Melee follows the normal [weapon rules](weapons.md). On top of that:

- **Monster melee is capped at 35 damage per hit** against players.
- Your defensive bonuses against monsters (see below) are **capped at 50%**.
- **Parrying monsters:** monsters with Parry have a Parry/100 chance to block 20–25% of your hit.

### Monster abilities

Special abilities (breath, area attacks, damage over time) use their own damage roll:

| Target | Damage |
|---|---|
| Player **with** pets or summons out | the monster's **maximum** damage |
| Player with no followers | minimum damage −2 to +5 |
| Damage-over-time on a player | 8–15 with followers, 5–8 without |
| A pet of 3+ control slots | max damage −5 to +10 |
| A smaller pet | max damage −5 to +5 |
| Pet whose owner holds a real weapon | +25% |

A successful parry, or an **armor absorb**, reduces ability damage by 20–35%.
The absorb chance depends on your armor material, per piece worn:

| Material | Absorb chance per piece |
|---|---|
| Cloth, leather | 0% |
| Studded | 2% |
| Bone, wood, stone | 3% |
| Ringmail | 4% |
| Chainmail | 5% |
| Plate, dragon | 7.5% |

### Your defenses against monsters

These add together and are **capped at 50%**:

| Source | Reduction |
|---|---|
| Creature-type armor/clothing properties (Undead, Arachnid, Daemonic, Draconic, Elemental, Giant, Vermin, Infidel) | +1% per point against that type |
| Creature-type runes | +1% per point against that type |
| Dispel Evil (Chivalry) | spell bonus |
| Magic food (Physical / Magical Resistance) | 10% |
| Guild prestige buffs | 5% per level |
| Bard protection, Taunt (15%+), Rising Star | bard bonuses |
| Druid stances (Ram, Worm, Ophidian Mage) | 10% + Nature mastery level |

Wizard stances (Mana Shield, Elusive Form, Arcane Skin) apply after the cap.

### Defensive item properties

- **Reactive Paralyze** (armor, clothing, runes): % chance to paralyze the attacking monster for 2.5 s.
- **Reflective** (armor, clothing, runes): % chance to deal the hit's damage back to the monster.

## Monster healing and curing

Monsters with Healing bandage themselves below 78% HP (6.5 s per bandage).

| | Formula |
|---|---|
| Heal chance | (Healing + 10) / 100 |
| Heal amount | Anatomy/10 + Healing/6 + 4 to Anatomy/8 + Healing/3 + 4 (+10 on self) |
| Cure chance | (Healing − 30)/50 − 10% per poison level (needs 60 Healing and 60 Anatomy) |

Poisoned monsters naturally cure after **10–15 seconds**.
Against a player with **Poison mastery** it takes longer: 2 s per mastery level (minimum 10 s), +0–5 s.
Pets cure after 5–10 s.

Champion-tier monsters, champion minions and global quest bosses **don't regenerate HP**.

## Pets

### Taming and control

- You need **Animal Taming and Animal Lore both at or above** the creature's taming requirement to control it.
- Creatures with a taming requirement of 29.1 or lower always obey.
- **Golems** need 200 combined points of Item Identification, Tinkering, Remove Trap and Detect Hidden instead.

### Loyalty and bonding

- Each piece of food has a 50% chance to raise loyalty by 10 (max 100).
- Feeding also restores stamina: 15 per food item − 50.
- **Bonding takes 3 days** of feeding. Your **base** Animal Taming must be at or above the pet's taming requirement.
  Feed it again to see how long is left.
- Unchained pets use a hunger system (0–100%) and favourite foods instead.

### Pet resurrection

A resurrected bonded pet comes back with:

```
15 HP + max HP × (Spirit Speak + Veterinary + Animal Lore) / 7.5 %   (max +50%)
```

- Nature mastery adds +1% per level.
- Veterinary Boost runes add more.
- Each resurrection costs every skill **0.2 points**. Skills never drop below half their cap.

### Pet power scrolls

Drop a pet power scroll on an Unchained pet or golem to raise one skill's cap by **+1**, up to:

| Scroll | Max cap |
|---|---|
| Creature Powerscroll | 110 |
| Mythical Creature Powerscroll | 115 |
| Legendary Creature Powerscroll | 120 |

The pet must already have the skill. You can't use scrolls in PvP.

### Pack instinct

Pets with the same pack instinct, all attacking the same target within 5 tiles, deal bonus damage:

| Pack size | All single-slot pets | Mixed pack |
|---|---|---|
| 2 | +20% | +10% |
| 3 | +30% | +15% |
| 4 | +40% | +20% |
| 5+ | +50% | +25% |

The **Howling Pack Pelt** artifact cloak adds +3% per tier.

### Pets in PvP

- Pet melee against players is capped at **15 damage** *(default)*.
- Pet Wrestling and Tactics count as **100 max** in PvP.
- Pet Strength counts as 250 per control slot (min 150) for damage *(default)*.

### Pack animals

A pack animal that sits idle (no movement, order or target change) for **48 hours** drops everything it carries on the ground and disappears.

## Summons

- **Dispel difficulty** goes up by Spirit Speak × 0.1 while the summoner is alive. It goes up by another 5 at 120 Spirit Speak.
- Summoned creatures always obey their caster.
