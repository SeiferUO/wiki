# Instruments & Bard Skills

How instruments work and how Peacemaking, Provocation and Discordance are calculated.

!!! note
    The [Battle Lute](../bard/battle-lute.md) counts as an instrument while you wield it.
    Bard masteries and Spellsongs are on the [Spellsongs](../bard/spellsongs.md) page.

## Playing an instrument

You use the instrument you last played. A wielded Battle Lute is always used first.

### Musicianship effectiveness

Every bard skill first checks your **Musicianship effectiveness**:

```
effectiveness = Musicianship + (Peacemaking + Provocation + Discordance) / 3     (max 120)
```

Your chance to play well is effectiveness / 100.
If you play badly, the bard skill fails and the instrument loses a use.

### Range

```
range = 8 + skill / 15  tiles
```

At 120 skill that's **16 tiles**.

### Uses

Each attempt, success or failure, uses one charge. **Exceptional instruments have twice the uses.**

## Difficulty

Every creature has a bard difficulty based on its [tier](creatures.md#difficulty-tiers):

| Creature tier | Difficulty |
|---|---|
| New | 60 |
| Easy | 80 |
| Medium | 100 |
| Hard | 120 |
| Elite | 130 |
| Legendary / Abomination | 145 |
| Mini-boss and Expeditions | 150 |
| Dungeon boss and above | 160 |

### What lowers difficulty

| Source | Difficulty |
|---|---|
| Exceptional instrument | −5 |
| Wood: Oak −2.5, Ash −5, Yew −6, Heartwood −7.5, Bloodwood −8, Frostwood −8.5 | |
| **Slayer instrument** against the matching type | −10 |
| Musicianship effectiveness above 100 | −0.5 per point |
| Each extra bard skill at 60+ (beyond the first) | −10 |
| Each spellsong charge you're carrying | −2 |
| Injured target | up to −10 (1 per 10% HP missing) |
| Perfectionism | −25 |
| Lyrical mastery | −0.25 per level |
| Effective Barding runes (PvM) | −1 per point, max −50 |

Each skill also has its own built-in adjustment (see below).

### Success chance

```
chance = (skill − difficulty + 25) / 50
```

You see your approximate chance every time you try.

**Example:** 120 Peacemaking against a Hard monster (120), exceptional instrument, all three bard skills at 60+:
difficulty = 120 − 5 − 10 (peace bonus) − 20 (two extra skills) = 85, so chance = (120 − 85 + 25) / 50 = 100%.

!!! tip "Slayer instruments"
    Runic carpentry tools have a 25% + 0.1% per Carpentry point chance to give an instrument a random slayer.

## Cooldowns

After any bard action, **all** bard skills are locked for **1.5 seconds**. Then each skill has its own cooldown:

| Result | Cooldown |
|---|---|
| Failure | 2 s |
| Success (single target) | 10 s |
| Peacemaking area | 8 s |
| Provocation self-taunt | 7.5 s |

Lyrical mastery shortens cooldowns by 0.033 s per level (minimum 3 s on success, 1 s on failure).

## Peacemaking

### Single target

- Difficulty: creature difficulty **−10**.
- **Duration: 100 − difficulty / 1.5 seconds, between 10 and 20 s.**
- **Legendary and stronger monsters** are calmed for 10 s and then **immune for 25 s**.
- **Pets (PvP):** 1 s per 10 Peacemaking, max 12 s.
- **Players:** clears their target and interrupts their spell.

**Breaking peace:** each time a calmed monster is hit, it has a 1% chance per attacker, +1% per hit so far, to break free.

### Area (target yourself)

- Calms up to **1 monster per 10 Peacemaking**, closest first.
- Only stops their attack. It doesn't hold them like a targeted peace.
- Doesn't affect players or pets.

## Provocation

### Monster vs monster

- Difficulty: average of both creatures' difficulty **−5**, **+15 for each one that is Legendary or stronger**.
- You **can't provoke** creatures with more HP than the Legendary tier, or pets.
- Both creatures must be within your bard range of each other.
- A provoked monster has a **5% chance per hit taken** to get confused and stop.
- Provoked monsters deal **+25%** damage to the monster they were sent at.

### Taunt (target yourself)

- Up to **1 monster per 20 Provocation** in range and line of sight is taunted onto **you**.
- Taunted monsters deal **15% less damage** to you for 15 s.

## Discordance

### Single target

- Difficulty: creature difficulty **−10**.
- Can't be used on pets.

**Effect strength:**

```
effect = (Discordance + Musicianship effectiveness) / 240 × 17.5%   (+0.5% per Lyrical level)
```

At 120/120 the effect is **17.5%**. It's 25% weaker against Abomination-tier and stronger monsters.

A discorded monster **takes that much more melee damage** and **deals that much less**.

**Duration:**

| Creature tier | Duration |
|---|---|
| Below Elite | 15 s |
| Elite | 12.5 s |
| Legendary | 10 s |
| Mini-boss and Expeditions | 7.5 s |
| Dungeon boss and above | 5 s |

Barding Duration runes add up to +50% in PvM.

### Area (target yourself)

- Up to **1 monster per 20 Discordance**, closest first.
- Difficulty −10. Durations are **halved**.

## Spellsong charges

When your Musicianship effectiveness is 50+, each successful targeted bard skill gives **1 spellsong charge**.
You have a Musicianship/500 chance to get a second one (+1% per Lyrical level).

- Every charge makes your next bard skill **2 difficulty easier**.
- At **6 charges** a Spellsong fires. If the target is Mini-boss tier or weaker, that peace or discord lasts **twice as long**.
