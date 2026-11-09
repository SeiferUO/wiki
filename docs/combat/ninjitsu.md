# Ninjitsu

!!! danger "No effect in PvP"
    Ninjitsu does **nothing in PvP** except one thing: **+1% weapon damage against players per 10 points** (max **+10%**).
    That's the same bonus as Chivalry, and the two don't stack: only the higher skill counts.
    See [Weapons](../core/weapons.md#chivalry-in-pvp).

    - Techniques can't be used during PvP combat, and none of them work on players or on players' pets and summons.
    - A technique armed before the fight (Focus Attack, Counter Attack, Evasion, Iron Will...) does nothing once PvP combat starts.
    - Hitting players gives no Perfection, and the codex passives don't work in PvP.

Ninjitsu is a melee skill with twelve **techniques**. They run on **Perfection**, a resource you build by fighting monsters, not on mana.
The **Codex of the Shadow Blade** upgrades every technique and the way you gain Perfection.

## Getting started

- Characters who pick Ninjitsu at creation start with a **Katana** and the **Codex of the Shadow Blade**.
- The codex is also sold by **Selwyn the Archivist** for 1,500 gold. See [Weapon Codex](../codex/weapon-codex.md).
- Ninjitsu goes up to **100**. It rises when you land hits on monsters (35% chance per hit that builds Perfection).

### Commands

| Command | What it does |
|---|---|
| `[ninjitsu` | Opens the technique hotbar (or `[ninja`) |
| `[ninjitsu 1-12` | Uses a technique by its number on the hotbar (top row 1–6, bottom row 7–12) |
| `[ninjitsu evasion` | Uses a technique by name |
| `[ninjainfo` | Opens the technique descriptions |
| `[ninjacodex` | Opens the codex (it must be in your backpack) |

The hotbar shows your Perfection bar. A technique turns **gold** while it's active or armed, shows its **cooldown** in red,
and is **greyed out** until you have the skill for it.

## Perfection

Perfection is the resource every technique spends. You can hold **100** (+10 per *Perfection Capacity* tier, max 130).

| Action | Perfection |
|---|---|
| Hitting a monster | +0.5 |
| Critical hit on a monster | +1.5 |
| Missing | 50% chance to lose 0.5 |
| Each step you take | 3% chance for +0.5 (10% while hidden) |

- Hitting **players** or their pets gives no Perfection.
- *Perfection Flow* adds +10% to every gain per tier. *Composure* lowers the chance to lose Perfection on a miss.
- Codex talents add more ways to gain it: *Swift Stride*, *Shadow Step* and *Deflection* (see below).

## Skill scaling

Every technique reaches **full power at its required skill + 50** (never above 100). Below that, its power is
your skill ÷ that number. A character with a few points of Ninjitsu can use **Focus Attack**, but it won't be reliable until 50.

| Technique | Required skill | Full power at | What scales |
|---|---|---|---|
| Focus Attack | 0 | 50 | Chance not to miss, chance to crit |
| Iron Will | 20 | 70 | Life healed per hit |
| Counter Attack | 25 | 75 | Chance to counter |
| Tokuno Mark | 30 | 80 | (poison level scales on its own, see below) |
| Vanish | 35 | 85 | Stealth steps |
| Evasion | 45 | 95 | Duration |
| Kiai Strike | 50 | 100 | Chance not to miss, damage bonus |
| Honorable Execution | 60 | 100 | Bonus damage, heal on a kill |
| Momentum Strike | 75 | 100 | Number of targets |
| Shadowrush | 90 | 100 | Damage per tile |
| Death Mark | 100 | 100 | Always full power |
| Iaijutsu | 100 | 100 | Always full power |

## Techniques

Costs and cooldowns are before codex upgrades. *Perfection Efficiency* lowers every cost.

| # | Technique | Skill | Perfection | Cooldown |
|---|---|---|---|---|
| 1 | Focus Attack | 0 | 10 | 6 s |
| 2 | Iron Will | 20 | 15 | 25 s |
| 3 | Counter Attack | 25 | 10 | 12 s |
| 4 | Tokuno Mark | 30 | 10 | 10 s |
| 5 | Vanish | 35 | 20 | 30 s |
| 6 | Evasion | 45 | 25 | 30 s |
| 7 | Kiai Strike | 50 | 15 | 15 s |
| 8 | Honorable Execution | 60 | 25 | 15 s |
| 9 | Momentum Strike | 75 | 40 | 30 s |
| 10 | Shadowrush | 90 | 30 | 20 s |
| 11 | Death Mark | 100 | 30 | 25 s |
| 12 | Iaijutsu | 100 | 50 | 20 s |

### Focus Attack
Your next attack within 8 seconds is more likely to hit and to be a **critical hit** (×1.5 damage).
Both chances reach 100% at 50 Ninjitsu.

### Iron Will
For 6 seconds, every hit you take heals you for **3% of your life** and gives **1 Perfection** (at most twice per second).

### Counter Attack
For 2 seconds, the next melee attack against you is turned aside and answered with a counter strike.
A successful counter shortens the cooldown to 4 seconds. A failed counter attempt still ends the stance.

### Tokuno Mark
Your next hit on a monster within 8 seconds poisons it. The poison grows with your Ninjitsu: **Regular**, **Greater** at 60,
**Deadly** at 90. It's one level stronger from stealth, and *Tokuno Venom* adds more (max **Lethal**).

### Vanish
Drop a smoke bomb and vanish, even in combat: enemies lose you as their target, you can take **6 steps** unseen,
and your next attack is a stealth attack.

### Evasion
You become ethereal for **3 seconds**: weapons can't hit you and you take no damage, but you can't swing,
use techniques or do anything harmful.

### Kiai Strike
Hold your stance for **3 seconds** without attacking (an attack, spell or technique restarts the count).
Your next hit on a monster within 8 seconds is more likely to hit and deals **+25% damage**.
It doesn't combine with Focus Attack or Honorable Execution.

### Honorable Execution
Your next hit within 8 seconds is a killing attack (**+40% damage**).

- **If it kills:** you heal **15% of your life** and get **+20% swing speed** for 8 seconds.
- **If it doesn't:** you take **25% more** melee and spell damage for 7 seconds.

### Momentum Strike
Rapidly strike the **3 closest monsters** within 5 tiles, then return to where you stood.
*Momentum Reach* adds a chance to strike one more.

### Shadowrush
Dash to a monster up to **5 tiles** away (8 with the codex) and strike: **+8% damage per tile** travelled.
The target must be at least 2 tiles away and the path must be clear.

### Death Mark
Mark a monster for **5 seconds**. When the mark ends, it bursts for **25%** of all the weapon damage you dealt to it
(up to 45% with the codex).

### Iaijutsu
A lightning draw that ignores your swing timer and spends **all** your Perfection (50 at least):
**+1.5% damage per point** spent, so a full bar strikes for 2.5×. Your current target must be within reach of your weapon.

### Stealth bonus
Damaging techniques used while a **stealth attack is ready** (after hiding or Vanish) deal **+25% damage**
(+5% per *From the Shadows* tier).

## Codex of the Shadow Blade

Double-click the codex (or say `[ninjacodex`) to spend points.

!!! warning "100 Ninjitsu required"
    Codex talents only work at **100 base Ninjitsu**, and codex XP is only earned at 100.
    Below that you keep the talents you bought, but none of them do anything.

### Points

- Killing monsters gives codex XP: the same XP as the kill, after every XP bonus (see [Experience System](../core/experience.md)).
- You only earn it at **100 base Ninjitsu**.
- **Catch-up bonus**, like the weapon codexes:

    | Points earned | Codex XP |
    |---|---|
    | 0–49 | ×2 |
    | 50–99 | ×1.5 |
    | 100–149 | ×1.25 |
    | 150+ | ×1 |

- XP for the n-th point: **800 × n + 2 × (n − 1)²**.
- Each tier costs 1 point more than the tier before (the first tier costs the "base" below).
- **Reset:** 100 gold per point spent, paid from your bank.

### Way of the Blade

| Talent | Tiers | Base cost | Effect per tier |
|---|---|---|---|
| Focus Attack Power | 5 | 3 | +10% critical damage |
| Execution Power | 5 | 2 | +5% execution damage |
| Momentum Power | 5 | 1 | +5% strike damage |
| Momentum Reach | 5 | 3 | 5% chance to strike one more target |
| Shadowrush Power | 5 | 2 | +1% damage per tile |
| Shadowrush Range | 3 | 1 | +1 tile (max 8) |
| From the Shadows | 5 | 2 | +5% stealth bonus |
| Death Mark Power | 4 | 2 | +5% burst (max 45%) |
| Iaijutsu Power | 5 | 2 | +10% damage at 100 Perfection |
| Kiai Power | 5 | 2 | +25% Kiai damage |
| Tokuno Weaponry | 5 | 1 | +1% critical chance with ninja weapons |

Ninja weapons: Bokuto, Daisho, Kama, Lajatang, No-Dachi, Nunchaku, Sai, Tekagi, Tessen, Tetsubo, Wakizashi and Yumi.

### Way of the Mind

| Talent | Tiers | Base cost | Effect per tier |
|---|---|---|---|
| Counter Stance | 4 | 1 | +0.25 s Counter Attack stance |
| Counter Recovery | 3 | 1 | −1 s cooldown after a successful counter |
| Counter Bleed | 5 | 2 | 2.5% chance a counter makes the monster bleed (75% of a weapon hit over 5 ticks) |
| Evasion Duration | 5 | 2 | +0.5 s ethereal |
| Execution Recovery | 5 | 1 | +4% life healed on an execution kill |
| Execution Discipline | 3 | 1 | −1 s exposed after a failed execution |
| Smoke and Mirrors | 3 | 1 | −4 s Vanish cooldown, +2 stealth steps |
| Iron Will Recovery | 3 | 2 | +1% life per hit taken |
| Kiai Focus | 3 | 1 | −0.25 s Kiai charge |
| Tokuno Venom | 2 | 2 | +1 poison level (max Lethal) |

### Way of Perfection

| Talent | Tiers | Base cost | Effect per tier |
|---|---|---|---|
| Perfection Flow | 5 | 2 | +10% Perfection gained |
| Perfection Capacity | 3 | 3 | +10 max Perfection |
| Composure | 5 | 1 | −10% chance to lose Perfection on a miss |
| Perfection Efficiency | 3 | 3 | −5% technique cost |
| Swift Stride | 5 | 1 | +1% chance per step to gain Perfection |
| Shadow Step | 5 | 1 | +2% chance per step while hidden |
| Deflection | 5 | 2 | 5% chance to gain 1 Perfection when you dodge a monster's attack (not while ethereal from Evasion) |
