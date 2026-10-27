# Stealth & Thievery

## Hiding

- **You can't hide** while something that's fighting you is within range and line of sight:

    ```
    range = (100 − Hiding) / 2 + 8 tiles     (max 18)
    ```

- Below 100 Hiding there's a skill check. At **100+ Hiding you always succeed** if nobody is fighting you.
- Friends of a house always succeed inside it.
- Skill delay: **10 s** (Shadow mastery shortens it by 0.25 s per level, max 5 s).

!!! tip "Auto-stealth"
    With **80+ Hiding and 80+ Stealth** (outside PvP), hiding also starts stealth right away.

**Pets hide with you:** followers within 8 tiles that have Hiding skill (or a human body) hide too.
Their next hit is a stealth attack.

## Stealth

- Needs **80 Hiding** and you must already be hidden.
- Success chance: **80% + Stealth / 3 %**.
- Steps allowed: **Stealth / 5** (24 at 120).
- Shadow mastery adds extra steps and shortens the delay. It also arms a **stealth attack**: your next hit does bonus damage, more from behind or on a tracked target. See [Weapons](../core/weapons.md#4-pvm-bonus-damage).

## Detect Hidden

### Active

```
range = Detect Hidden / 10 tiles   (min 2, halved if the skill check fails)
```

For each hidden target: your Detect Hidden ±10 vs their Hiding ±10. If yours is higher, they're revealed.
Inside a house you're a friend of, range is 22 and everyone inside is found.

### Passive

Everyone with Detect Hidden constantly checks for hidden players within **4 tiles**. Each check has a small chance to reveal them:

```
chance per check = (Detect Hidden − (Hiding + Stealth) / 2 + 1) / 1000
```

Passive detection doesn't work in towns, safe zones, duel pits, jail, Covetous or the Stygian champion.

!!! info "Monsters and Shadow mastery"
    Monsters have Detect Hidden based on their [tier](../core/creatures.md#detect-hidden).
    Shadow mastery cuts a monster's detection advantage by up to **75%** at level 30.

## Stealing

- Only **Thieves' guild members** can steal from players, and not while they have murder counts.
- You must be empty-handed and not polymorphed.
- Items over **10 stones**, blessed items and **insured items** can't be stolen.
- You can't steal from players in safe zones, duel pits, Thornwall or the new player dungeon.
- Difficulty is the item's weight × 10. For stacks, you take up to (Stealing / 10) / weight items at once.
- Stealable artifacts need 100 Stealing.

**Getting caught:** chance = (150 − Stealing) / 150 (37.5% at 100, 20% at 120).
Everyone within 8 tiles sees the attempt. Stealing from an innocent outside the guild makes you criminal.

## Snooping

- On Felucca you can snoop anyone, as long as you're allowed to act harmfully toward them.
- In guarded towns you can't snoop blue human NPCs.
- If Snooping < a random 0–100, the target is told you're peeking.
- Each snoop costs 4 Karma.

## Poisoning

- On Felucca you can only poison **one-handed slashing or piercing weapons**, food, darts and shuriken.
- Poison charges on a weapon: **18 − 2 × poison level** (Lesser 18, Regular 16, Greater 14, Deadly 12, Lethal 10).
- On failure below 80 skill, there's a 5% chance to poison yourself.
- Skill delay: 10 s. Not usable in duel pits.
- Each success costs 20 Karma.

Hitting a monster with a poisoned weapon also gives Poisoning skill gains.

## Remove Trap

| Trap | How it works |
|---|---|
| Trapped containers | skill check against trap power (power to power + 10) |
| Dungeon traps | skill check. On failure, 25% chance to set it off |
| Treasure chests | checked every 10 s. Each failure spawns an Ancient Guardian. At 100+, it's a safe disarm after a waiting time that depends on chest level |
| Remove Trap trainer | trains you up to 100 |

Skill delay: 10 s.
