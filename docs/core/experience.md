# Experience System

Killing monsters gives **XP**. The same XP goes, at full value, to **every progression system you qualify for**: masteries, codexes, pets, summons, runes, your boat and more.

## XP from a kill

```
creature XP = creature max HP / 50      (min 1, max 3,500)
```

Champion spawn minions give **⅓**.

No XP from: tamed or summoned creatures, non-monsters, vendors, the Britain Zoo, Turret Defense, or anything during a **MOBA match**.

## Sharing a kill

Your share depends on how much damage you did (your pets' damage counts as yours).

- You must deal at least **5%** of the creature's HP (**1%** for mini-bosses and bigger) and be within **50 tiles**.
- **Solo:** you get XP × your damage %.
- **Groups** get a bonus multiplier, but each player's damage share counts only up to a ceiling:

```
group multiplier = 1 + 0.5 × (players − 1)
your XP          = creature XP × min(your damage %, ceiling) × group multiplier
```

| Players | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10+ |
|---|---|---|---|---|---|---|---|---|---|
| Damage ceiling | 70% | 60% | 50% | 40% | 35% | 30% | 25% | 22.5% | 20% |

**Party sharing:** party members within 50 tiles pool their damage and split it **equally**, so everyone in the party gets the same share.

## XP bonuses

| Bonus | Amount |
|---|---|
| **Danger Zone** | up to +50% |
| **Community Dungeon Trial** region | +10% |
| **Vial of XP** | +15% |
| **Scholarship** (armor, clothing, runes) | +1% per point (max 50) |
| **Server XP event** | set by staff |
**All bonuses together are capped at +65%.** [Rested XP](#rested-xp) comes on top of that.

## Rested XP

- If you go **8 hours or more** without earning XP, you build up **250 rested XP per hour**, up to **10,000**.
- While you have rested XP, kills give **double XP**: the extra XP is paid out of the pool. It doesn't count toward the +65% cap, so your other bonuses never stop the pool from being spent.
- You'll see a window at login when you have rested XP.

## When you can't earn XP

- You're dead.
- You have a pending **PvM captcha**.
- You haven't moved for 4 minutes.
- Another account from your IP is within 30 tiles (unless you're VIP).

## Where the XP goes

Every system below gets the **full** XP amount when you meet its requirement:

| System | Requirement |
|---|---|
| [Masteries](../masteries/index.md) | one active mastery |
| [Grimoire](../magic/grimoire.md) | Wizard mastery item and the pure mage skills |
| [Spell songs](../bard/spellsongs.md) | Musicianship 50+ and a song selected |
| Bard mastery | 200+ combined bard skills |
| [Summons](../pets/summons.md) | Spirit Speak 50+, a spellbook and a Summon Mastery tome |
| [Summoner Rituals](../magic/rituals.md) | Spirit Speak 50+, a Summoner Lantern and a ritual selected |
| [Chivalry](../magic/chivalry.md) | Chivalry 50+ and a Paladin Tome (or Chivalry 100) |
| [Necromancy](../magic/necromancy.md) | Necromancy 50+ |
| [Weapon codexes](../codex/weapon-codex.md) | 100 in the weapon skill with that weapon type equipped (Archery also needs a quiver) |
| [Golems](../pets/golems.md) and [Unchained pets](../pets/unchained.md) | the pet is out with you |
| [PvM runes](../items/ankhs-runes.md) | always (Rune XP) |
| [Boat](../items/boats.md), sailors, Mariner Parrot | you're on your boat |
| Mentoring | you're someone's student |
