# Poisoning & Poison

How poison works, how to poison weapons and food, and what makes poison stronger.

## Poison levels

A poisoned target takes damage every few seconds for **10 ticks**. The first tick comes 3.5 seconds after being poisoned.

```
tick damage = 1 + (target's current HP × poison %)   (kept between the min and max)
```

| Poison | % of current HP | Damage per tick | Tick every |
|---|---|---|---|
| Lesser | 2.5% | 4–26 | 3 s |
| Regular | 3.125% | 5–26 | 3 s |
| Greater | 6.25% | 6–26 | 3 s |
| Deadly | 12.5% | 7–26 | 4 s |
| Lethal | 25% | 9–26 | 5 s |

- Damage is based on **current** HP, so poison hits hardest on healthy targets.
- Half the time, a tick repeats the previous tick's damage.
- A target that's already poisoned can't be poisoned again by a weapon hit.

## Poisoning skill

Use the skill, target a **poison potion**, then target what you want to poison (within 2 tiles). It takes 2 seconds.

You can poison **one-handed slashing or piercing weapons** and **food**.

| Potion | Skill range | Weapon charges |
|---|---|---|
| Lesser Poison | 0–60 | 18 |
| Poison | 30–70 | 16 |
| Greater Poison | 60–100 | 14 |
| Deadly Poison | 80–100 | 12 |

- Your chance to succeed goes up as your skill moves from the bottom to the top of the potion's range. You get the empty bottle back.
- Each success costs **20 Karma**.
- If you fail below 80 skill, there's a **5% chance to poison yourself**.
- Skill delay: **10 s**. Not usable in duel pits.

### Poisoned weapons

Each hit with a poisoned weapon has a chance to poison the target:

```
chance = 10% + Poisoning / 10 %      (20% at 100, 22% at 120)
```

- Swords don't poison a target that's bleeding.
- **Charges:** a successful poison always uses a charge against players. Against monsters it only uses one **65% − 0.4% per Poisoning point** of the time (25% at 100, 17% at 120).
- **Assassin's Touch** ([Fencing codex](../codex/weapon-codex.md)): with a fencing weapon, each tier gives a **10% chance** (up to 50%) to keep the charge when it would be used against a monster.
- Hitting monsters with a poisoned weapon gives Poisoning skill gains.
- Spears don't keep poison: their charges are cleared at every server restart.

### Poison spell

The Magery **Poison** spell (3rd circle) poisons its target. Its strength depends on your **Magery + Poisoning**:

| Magery + Poisoning | Poison |
|---|---|
| up to 130 | Lesser |
| above 130 | Regular |
| above 170 | Greater |
| 200 or more | Greater, with a 10% chance of Deadly |

- **Against players**, the spell loses 10 points for every tile past 3 tiles of distance. Players can resist it with Magic Resistance.
- **Monsters** have a chance to resist the spell, depending on the monster. Poison-immune monsters always resist.
- With the [Grimoire](../magic/grimoire.md), the spell gets stronger with its tier (see [below](#grimoire-poison-spell)).

### Poisoned food

Whoever eats poisoned food is poisoned with that potion's poison. See [Food](../core/food.md).

## Stronger poison (PvM)

Against monsters, your poison ticks deal more damage from:

| Source | Bonus |
|---|---|
| Poison mastery | +2% per level (+60% at 30) |
| Poisoning above 100 | +1% per point (+20% at 120) |
| Doom *Toxic* armor set | half of the set's poison bonus |
| **Poison Damage** [PvM runes](../items/ankhs-runes.md) | + rune value |
| Monsters weak to poison | + their weakness |
| [Grimoire](../magic/grimoire.md) Poison spell, tier 3 | +25% |

**Pets** that poison get:

- +2% per level of their master's Poison mastery,
- +2.5% per point of their master's Poisoning above 100,
- +2.5% per point of their **own** Poisoning above 100,
- with the Unchained mastery *Additional Poison Tick*, a 10/15/20% chance per tick to add one more tick.

### Poison mastery

With [Poison mastery](../masteries/index.md#poison-venom) active:

- Monsters you poison stay poisoned longer: **+1 tick per 2 mastery levels**.
- **Venom Burst:** each tick, a chance to deal all the remaining ticks' damage at once and end the poison.
    - Chance = (Poisoning / 120) × (mastery level / 30), max 35%. At least 5% with 100+ Poisoning.
    - Cooldown: 30 s, down to 15 s at 120 Poisoning and level 30.
    - Only within 12 tiles of you. Bursts from your pets have a lower chance (25% for 1-slot pets, 50% for 2-slot, 75% for 3+).
- **You** can't be poisoned outside PvP.
- Your **pets** have a 10% + (level / 30) chance per tick to shake off poison (outside PvP).

### Grimoire Poison spell

With the [Grimoire](../magic/grimoire.md), your Poison spell gets stronger with its tier (on monsters):

| Tier | Effect, each tick |
|---|---|
| 1 | 25% chance to raise the poison one level |
| 2 | 25% chance to spread the poison to up to 5 unpoisoned monsters within 3 tiles |
| 3 | +25% damage |

## Resisting poison

Each of these is a chance to **not get poisoned at all** (all of them work outside PvP only, except where noted):

| Source | Chance |
|---|---|
| **Poison Resistance** properties on armor, clothing and jewelry, and Poison Resistance [PvM runes](../items/ankhs-runes.md) | 1% per point |
| [Druidic](../masteries/druidic.md) **Ophidian** and **Bug** forms | 15–45% |
| Bard **poison protection** | the bonus value |
| Doom **Toxic** armor set | the set's bonus |
| **Poison mastery** | always immune |
| New players (New Player protection) and players in Covetous | always immune |

Once poisoned, you can still shake it off:

- **Poison mastery:** the poison is cured on its first tick (outside PvP).
- **Orange petals** cure Lesser to Deadly poison on its next tick (not Lethal).
- **Protection shields** absorb poison ticks before your HP (outside PvP).

### Pets and summons

| Source | Chance |
|---|---|
| Unchained pet mastery **Poison Immunity** | 10 / 15 / 20% by tier |
| **Creature Poison Resistance** on your Shepherd's Crook | 1% per point |
| **Follower Poison Resistance** [PvM runes](../items/ankhs-runes.md) | 1% per point |
| Your **Poison mastery** (once poisoned) | 10% + level / 30 per tick to shake it off |

Some monsters are **immune** to poison.
