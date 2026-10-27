# Player Character

Stats, skills, regeneration, death, insurance and the other rules that apply to every character.

!!! note
    Numbers marked *default* come from in-game balance controllers or server config and can be changed by staff.

## Stats

| | Value |
|---|---|
| Total stat cap | **225** |
| Single stat cap (trained) | 100 |
| Single stat max (with items and buffs) | 150 |
| Hit points | Strength / 2 + 50 |
| Weight limit | 40 + 3.5 × Strength + 0.5 × Camping (+50 stones at 100 Camping) |

Stat scrolls and stat balls can raise the total cap.

## Skills

| | Value |
|---|---|
| Total skill cap | **700**, up to **720** with Skill Orbs |
| Single skill cap | 100 |

Each **Skill Orb** raises your total skill cap by **+1**, up to a maximum of **720**.

### Skills that can go above 100

Only these skills can have their **cap raised above 100** (for example with power scrolls):

Alchemy, Animal Lore, Animal Taming, Arms Lore, Begging, Blacksmithing, Camping, Carpentry, Cooking, Detect Hidden,
Discordance, Fishing, Fletching, Focus, Forensic Evaluation, Herding, Hiding, Inscription, Lockpicking, Lumberjacking,
Mining, Musicianship, Peacemaking, Poisoning, Provocation, Remove Trap, Spirit Speak, Stealth, Tailoring,
Taste Identification, Tinkering, Tracking, Veterinary.

All other skills are reset to a cap of 100 when you log in. Items and buffs can still raise their **effective** value above 100.

!!! warning "Skills above 100 in PvP"
    Many formulas count skills as **100 max in PvP**: Tactics, Meditation, Inscription and the bard skills used by the Battle Lute.
    Skill points above 100 are mainly for PvM.

## Regeneration

### Hit points

```
seconds per HP = 10 / (1 + regen points)
```

| Regen point source | Points |
|---|---|
| Hit Point Regeneration item property | +1 per point |
| Hunger (PvM only) | +1 per 10% hunger |
| Health Regen jewels and runes (PvM) | +1 per point, max 30 |
| Druid Nature form (PvM) | +10 + Nature mastery level |

**Max 30 points** (0.32 s per HP). Magic food (Hit Point Regeneration) adds 25% on top.

### Stamina

```
seconds per stamina = 10 / (2 + Focus / 10 + regen points)
```

Regen points come from Stamina Regeneration properties, hunger (PvM), and Stam Regen jewels and runes (max 30).
At 100 Focus with no items, that's **0.83 s per stamina point**.

### Mana

Mana regen starts at **7 seconds per point** and each source below makes it faster *(default)*:

| Source | Effect |
|---|---|
| **Meditation** | −6 s at 100 (counts as 100 max in PvP) |
| **Focus** | −5.75 s at 100 |
| **Taste Identification** | −6.15 s at 120 |
| **Intelligence** | −0.25 s at 125 Int |
| **Hunger** | up to 23% faster when full |
| **Actively meditating** | 35% faster |
| Magic food (Mana Regeneration), PvM | 30% faster |
| Mana Regen jewels and runes, PvM | 1% faster per point, max 30% |
| Bard aura (party), PvM | ~3% faster per point |
| Tangle / Hat of the Magi artifacts, PvM | 5% faster per tier |

- **Fastest possible: 0.25 s per point** (0.65 s per point in PvP).
- **Slowest: 7 s per point.**

!!! tip "Armor and mana"
    Armor that isn't meditable slows mana regen. **Taste Identification cancels the penalty**, fully at 120.
    On Felucca, a shield only counts against you if your Parry is below 80.

## Taking damage

### Burst protection

When creatures hit you for **25+ damage within 1.5 seconds**, extra damage is reduced:

```
reduction = (damage in window − 25) / 25 × 30%     (max 60%)
```

This stops monster packs and pets from one-shotting you.

### Bandages

Bandages only **slip from damage in PvP**. In PvM you can bandage freely while being hit.

## Death

When you die:

- One random item on your corpse (weapon, armor or jewelry with at least 15% durability left) loses **1–3 durability**. It never drops below 15%.
- 33% chance that all your equipped armor and weapons lose durability equal to **5% of their maximum**. This doesn't happen in duel pits.

### Resurrection

In PvM you come back with **35% HP, 25% mana and full stamina**. If you were mounted, you're put back on your mount automatically (where mounts are allowed).

### Places where you keep your gear

You keep everything you're wearing when you die in:
the new player dungeon, community champion spawns, safe zones, deathmatch arenas, invasion zones, duel pits and the Pit Trial.

New players with active **New Player protection** also keep their gear. In Covetous they're sent to the dungeon entrance instead of dying.

## Insurance

Insurance protects your **last-used item in each slot**:
weapon, shield, spellbook, helm, chest, arms, gloves, legs, gorget, ring, bracelet, necklace, earrings and one utility item.

- If an insured last-used item would drop on death, it stays on you and you pay to reinsure it.
- You can pay in **gold** (from your bank) or **reward points** (1 point per 250 gold).
- Cost depends on the item: base type, material, quality, artifact status and each PvM property. Range **10–125,000 gold**. Some regions change the cost.
- **Utility items** (Summoner Lantern, Eldritch Orb, quivers and resource collectors) cost a flat 12,500 gold or 5 points.
- If you can't afford to reinsure, the item is still saved this time, but it **will drop on your next death**.
- The player who killed you gets **half the cost** (max 50,000 gold or 2,500 points).
- If you die again **within 2 minutes of resurrecting**, your items are protected for free.
- Insurance doesn't work in PvP combat, if a pet killed you, or if you killed yourself.

You get a warning when your bank or points can't cover your insurance on the next death.

## Murder counts

### Reporting

When a player kills you, a **report window** opens a few seconds after death for each player who attacked you. It stays open for 5 minutes.

- **Yes** gives that player **+1 murder count** (short and long term) and +1 lifetime kill on their account. Murdering a **Young** player counts **double**.
- At **5 Kills** a player becomes a **murderer** (red).
- A Paladin Guild member's first murder **kicks them from the guild**.
- You can't report the same player again for **5 minutes**.
- No report window for deaths in duel pits, or if you're in the Thieves Guild.

Everyone who fought you in the last 30 seconds also gets **fame** (your fame ÷ 200) and **karma**: −850 for killing an innocent (less if they're already very low), +50 for killing a criminal or murderer.

### Decay

| | Decay |
|---|---|
| Short-term murders | −1 every **8 hours** of game time |
| Long-term murders (Kills) | −1 every **40 hours** of game time |

Murder counts only decay while you're logged in.

## Experience gain

You only earn XP (masteries, pets, summons, quivers, bard, talismans and monthly challenges) when:

- you are alive,
- you have moved in the last 4 minutes,
- you don't have a pending anti-bot check,
- no other account from your IP is within 30 tiles (VIP accounts are exempt).

## Movement

Druids in a warrior, archer or mage stance move at **mounted speed** on foot.

## Young players

Young characters can't be attacked by monsters in protected regions.
When they die, they're teleported to safety and keep their items in their backpack.
