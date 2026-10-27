# Spellsongs & the Bardic Codex

Bards build up **spellsong charges** with successful barding. They then release a **Spellsong**, an area buff, heal or debuff.
The **Bardic Codex** adds **Tempo auras** that buff your whole party.

How barding itself works (difficulty, success, durations) is on [Instruments & Bard Skills](../core/instruments.md).

## Spellsongs

### Charging

- Every successful **targeted** Peacemaking, Provocation or Discordance (with Musicianship effectiveness 50+) gives **1 charge**.
  There's a Musicianship / 500 chance for a second one (+1% per Lyrical mastery level).
- A successful self-taunt also gives a charge.
- Each charge makes your next bard skill **2 difficulty easier**.
- At **6 charges** your chosen spellsong plays automatically and the charges reset.

### Range

Songs hit everything valid within **6 tiles** (+2 with Lyrical mastery, more with the codex, max 12).
Silence and Repugnance hit at most 5 targets.

Each song has its own XP, which raises its duration. In the table below, "XP" means that song's XP.

### Song list

| Song | Effect on you | Effect on others |
|---|---|---|
| **Heal** | Heals **15%** of your max HP (+1% per Lyrical level) | Party members get 35% of that |
| **Pet Heal** | — | Heals pets for **7.5% per control slot** of their max HP (+0.5% per Lyrical level) |
| **Regeneration** | Heals 2.5% HP every 2.5 s (double when you're low), for 5–15 s | — |
| **Mana** | Restores **15%** of your max mana (+1% per Lyrical level) | Party members get half |
| **Armor** | **10–25%** less physical damage from monsters for 10–35 s | Allies: 5–12% |
| **Spell Resistance** | **10–25%** less spell damage from monsters for 10–35 s | Allies: 5–12% |
| **Cure** | **35–70%** poison resistance for 10–45 s | Allies: 15–30% |
| **Quicksilver** | Faster attacks for 5–15 s | — |
| **Concentration** | **Never miss** for 5–25 s | — |
| **Perfectionism** | **−25 bard difficulty** for 10–45 s | — |
| **Evasion** | Monsters are 25% less likely to hit you, for 10–30 s | — |
| **Retribution** | Healing damages enemies for 10–30 s | — |
| **Savage** | — | Your pets go **savage** (+10% damage, +5% per control slot) for 10–30 s |
| **Silence** | — | Up to 3 monsters can't cast for 10 + Musicianship/10 s (Legendary: 5 s) |
| **Repugnance** | — | Pushes up to 5 monsters back 3–6 tiles |
| **Hex** | — | Hexes monsters, boosting your spell surge damage |

Durations grow with the song's XP (+1 s per 10,000 or 20,000 XP depending on the song).

## Bardic Codex: Tempo auras

Buy the **Bardic Codex** from Selwyn the Archivist (1,500 gold).

### Requirements

To use auras you need either:

- all three bard skills at 100, **or**
- one bard skill at 80+ **and** Musicianship effectiveness 80+.

### Tempo

| | Value |
|---|---|
| Tempo pool | **1,000** (+100 per *Tempo Capacity* tier) |
| Cost to start an aura | 75 Tempo (min 50 to activate) |
| Drain while active | 4 Tempo every 2 s |
| Aura range | 8 tiles (your party) |
| Switching auras | 10 s cooldown |

**Gaining Tempo:**

- +10 per successful targeted bard skill, +5 per area use,
- +5 on monster hits and spell hits (with a chance based on Lyrical mastery),
- on kills (*Death Dance* talent),
- when you heal.

### Auras

Only one aura at a time. Allies keep the best aura affecting them.

| Aura | Skill | Party bonus |
|---|---|---|
| **Discord** | Discordance | Armor and spell **penetration**: Discordance / 10 % × Virtuoso, +1.5% per codex tier |
| **Provocation** | Provocation | **Damage reduction**: Provocation / 10 % × Virtuoso, +2% per codex tier |
| **Peacemaking** | Peacemaking | **Accuracy**: Peacemaking / 10 % × Virtuoso, +1% per tier. Also mana regen |

An aura needs at least 80 in its skill.

### Virtuoso multiplier

| Bard skills at 100 | Multiplier |
|---|---|
| 0–1 | ×1.0 |
| 2 | ×1.5 |
| 3 | ×2.0 |

The *Virtuoso* talent adds +0.1 per tier.

**Example:** all three skills at 120 with a Discord aura gives 12% × 2.0 = **24% penetration** to everyone in range.

**Big parties:** above 5 members, aura strength drops 2% per extra member (max −30%).

### Codex talents

Codex XP comes from killing monsters. See [Bardic Codex](bard-codex.md) for every talent, its per-tier value and its cost.
