# Champion Spawns

A champion spawn is a dungeon-wide fight. Clear 16 levels of spawn around the altar and the **champion** appears.

## The champions

| Spawn | Champion | Drops Champion Idol |
|---|---|---|
| Deceit | Paradigm | ✅ |
| Glacia | Frozen Wyrm | ✅ |
| Sandstorm | Sandspire | ✅ |
| Destard | Progenitor Dragon | ✅ |
| Eventide | Goliath | ✅ |
| Shame | Terathan Queen | ✅ |
| Delucia | Molten Wyvern | ✅ |
| Wrong | The Tinker | — |
| Exile | Tortuar | — |
| Hollow | Barracoon | — |
| Ocean | Osiredon | — |
| Doom (community) | the **Stygian Champion** | — |

Altars set to a random type pick one of Deceit, Glacia, Sandstorm, Destard, Eventide, Delucia, Shame or Wrong each time they restart.

## Starting a spawn

An altar wakes up once **8 crystal skulls** sit on it. Skulls come from two places:

- **Champion Crystals:** Hard and stronger monsters in Deceit, Glacia, Sandstorm, Wrong, Destard, Eventide, Shame, Delucia, Hollow and Exile have a **1%** chance to drop a crystal for that dungeon. Fishing from a boat has a **0.1%** chance per catch to give an **Ocean** crystal. Target the matching altar to place it. Crystals decay after about 7 hours.
- **Dungeon kills:** killing monsters in the dungeon fills a hidden meter for its altar. Each time it fills, a crystal skull is placed for the player who made the last kill *(points set by staff)*.

Everyone who places a skull becomes a **crystal contributor** and gets a bonus at the end (see [Rewards](#community-rewards)). When the 8th skull lands, contributors get a window telling them the spawn has started.

!!! note
    You can't place crystals while the spawn is already running, or from a Haven region.

## Levels

- The altar shows your progress with **red skulls** (levels) and **white skulls** (progress through the current level, one per 20%).
- Killing **90%** of the current level's kill count advances to the next level. Kill counts and when the spawn gets tougher are *set by staff*.
- Only creatures from the **current stage** count toward progress.
- The spawn has 4 stages of creatures. Each stage pulls the spawn area tighter (100% → 75% → 50% → 25% of the radius).
- After level 16, the **champion** appears in the middle of the altar. If it wanders more than 75 tiles away, it's pulled back.

**Stalling:** if a level isn't finished within **10 hours**, the white skulls are lost. With no white skulls, the spawn drops a level instead.

Spawn creatures are champion minions: they give reduced [XP](../core/experience.md) and no [rare-loot](../items/rare-loot.md) kill points, and can't be tamed.

## Killing the champion

The champion is a dungeon boss and uses the shared [boss rewards](index.md#boss-rewards): top-3 rewards, Void Skulls and scaling. Its corpse is worth **Champion Idol** chances too:

- Paradigm, Frozen Wyrm, Sandspire, Progenitor Dragon, Terathan Queen, Goliath and Molten Wyvern have a **25%** chance to drop their **Champion Idol** for the [Tome of the Harrower](harrower.md).
- Paradigm also has a 75% chance to drop the **Vile Heartstone** (a [Peerless](peerless.md) offering).

### Community rewards

When the spawn ends, everyone who damaged spawn creatures or the champion earns **Community Champion Rewards**:

```
rewards = your damage ÷ damage per reward
damage per reward = 1,000 × number of participants (min 5,000, max 12,500)
```

- **Crystal contributors** get +1 reward and 10 reward points.
- The **top 3 damage dealers** of the whole spawn get a power scroll.
- Rewards per player per spawn are capped *(set by staff)*.

Say **[claimrewards** to claim them one at a time. Each claim rolls:

| Chance | Reward |
|---|---|
| 30% | 250–500 gold |
| 20% | 500–750 gold |
| 10% | a magic item (better roll ranges are rarer) |
| 8% | a magic spellbook |
| 7% | 500–750 gold |
| 5% each | treasure map (level 1–2), arcane scroll, mastery orb |
| 3% each | rare-hued dungeon cloth, special item |
| 2% | rare-hued item |
| 1% | power scroll |
| 1% | treasure map (level 3–5) |

### Restarting

After the champion dies, the altar rests for **8–36 hours** before it can start again.

## The Stygian Champion (Doom)

The Doom spawn is a **community** event:

- The portal to the Doom Realm opens **every 3 days** (the timer restarts when the spawn ends). Everyone gets a window, a server broadcast and a Discord message.
- Click **join** in the window to be teleported in (not from jail or during a duel).
- You can speed it up by offering items at the stone: an **artifact** takes 2 hours off, an **Expedition Ticket** 1 hour, an **essence** 30 minutes.

**Doom Realm rules:**

- **No PvP**: players and their pets can't harm each other. Explosion potions and Chain Lightning don't hit players.
- **No item loss**: you keep your equipment and backpack when you die.
- **No mounts** (you're dismounted on entry and remounted when you leave). Druid shapeshift speed is off.
- No Recall, Gate Travel, Mark, Wall of Stone or Energy Field.
- You can't loot other players' corpses.
- Its champion is the **Stygian Champion**, a much tougher Doom Exodus.
- Players who dealt **10,000+ damage** to it and are nearby share a pool of **Void Skulls**, dealt out evenly. The pool is full size with 10+ players and shrinks with fewer (never below ⅓).
- Dealing **10,000+ damage** during the event also gives a bonus item.
