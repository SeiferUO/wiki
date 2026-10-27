# Boats

## Hull and damage

- A boat has **25,000 hull HP**, +2,500 per Hull Integrity upgrade.
- At **25% HP** the planks unlock, so the boat can be boarded.
- Below 25% durability the boat is **scuttled** and can't move.
- An unused boat decays after **15 days**.

### Repairs

Use a **Ship Repair Tool** while you're the owner or pilot, and stand still. A repair heals over 5 ticks of 1.5 seconds:

```
total repair = 10% of max hull
             + up to 5% from Carpentry (5% at 100)
             + metal bonus
             + 10% per Repair Mastery tier
```

| Tool metal | Charges | Repair bonus | Your cooldown |
|---|---|---|---|
| Iron | 25 | — | 30 s |
| Dull Copper | 30 | +2% | 27 s |
| Shadow Iron | 35 | +4% | 24 s |
| Copper | 40 | +6% | 21 s |
| Bronze | 45 | +8% | 18 s |
| Gold | 50 | +10% | 15 s |
| Agapite | 55 | +12% | 12 s |
| Verite | 60 | +15% | 9 s |
| Valorite | 75 | +20% | 5 s |

A boat can only be repaired once every **30 seconds**, no matter who repairs it.

### Boarding

- Throw a **Boarding Rope** at an enemy ship within 8 tiles. Its hull must be at **75% or less**.
- There's a 10-second delay between uses. A rope holds up to **50 charges**, and you can combine ropes.
- At **25% hull** the enemy's planks unlock, so you can just walk aboard.

### Dry docking

To dry dock, the boat must be **fully repaired**, with an **empty hold**, nothing left on deck and no other players aboard. You also need the key.

### Sinking

When the hull hits 0:

- The cargo hold drops into a **salvage crate** where the boat sank.
- Sailors on board die with the ship.
- After 6 seconds, every player on board is **killed** and washes ashore in Britain.
- The boat goes to the **Ship Recovery Vendor**. You can reclaim it within **7 days** for **5,000 gold**, +3,000 per cannon on galleons.

## Boat upgrades

Kills made while you're on your boat give it **boat XP**: **500 XP = 1 upgrade point**. Gains happen at most once every 10 seconds per boat.

Each upgrade tier costs points equal to the tier (tier 1 = 1 point, tier 2 = 2 points, and so on). Most upgrades go to **tier 5**.

### Vessel

| Upgrade | Per tier |
|---|---|
| Extra Cannons | +1 cannon per broadside (max 2) |
| Cannon Power | +5% cannon damage |
| Fire Rate | −10% cannon cooldown |
| Cannon Range | +1 tile range |
| Cannon Splash | +1 tile splash radius |
| Hull Speed | +1 speed tier |
| Hull Integrity | +2,500 max hull HP |
| Armored Hull | −5% hull damage taken |
| Extra Shot | +1 cannonball per shot |
| Repair Mastery | +10% repair effectiveness |

### Crew and sea

| Upgrade | Per tier |
|---|---|
| Crew Size | +1 sailor on deck (max 3) |
| Sailor Fortitude | +20% sailor HP |
| Sailor Strength | +10% sailor damage |
| Sailor Toughness | −5% melee damage taken by sailors |
| Sailor Ward | −5% spell damage taken by sailors |
| Sailor Repair | 50 + 75 × tier HP per sailor repair |
| Sailor Medic | Faster sailor heals, +15% heal amount |
| Fishing Speed | 10% faster fishing |
| Auto-Fishing | Fishes automatically while anchored. The hold caps at 500 items and auto-fishing pauses when it's full. |
| Rare Loot | +5% rare loot chance |

## Sailors

Sailors are crew members who stand on your deck. Give each one a **duty**: fighting, fishing, cleaning, healing or repairing. You can change a sailor's duty once every **2 minutes**.

- Fighting sailors only attack monsters, never players.
- Sailors level up to **10**.
- A sailor who falls off the boat is lost.

## Cannons

- Load a cannon by targeting cannonballs. It holds up to **5 shots**.
- **Range:** 12 tiles, plus Cannon Range upgrades. You need line of sight.
- **Reload:** 5 seconds × the Fire Rate modifier. You can fire any cannon at most once every 3 seconds.
- **Heat:** a shot within 10 s of the last one adds 20 heat (a slower shot has a 25% chance to add 10). At **100 heat** the cannon **overheats** for **2 minutes**.

### Damage

```
damage = (150–350 + Fishing / 2)
         × (1 + Cannon Power)
         × (1 + up to 15% Tinkering + up to 15% Remove Trap)
         × 1.35 if your boat is not moving
```

- Shooting a player on an enemy boat also damages that boat's hull.
- A ground shot splashes everything within **2 tiles** (+ Cannon Splash), and the damage is split between the targets hit.
- You can't fire at your friends, party or guild on your own boat.

### Cannonballs

| Ball | Effect |
|---|---|
| Standard | Damage |
| Poison / Greater / Deadly | Regular / Greater / Deadly poison. Greater adds poison fields, Deadly also splashes. |
| Explosive / Greater | Area blast. Greater adds fire fields. |
| Shrapnel / Greater | Bleeding. Greater also splashes. |

## Fishing at sea

### Fishing hotspots

Hotspots spawn across the seas. Fishing within **8 tiles** of one uses a charge (20–35 charges). Each catch has a chance for:

| Chance | Result |
|---|---|
| 10% | A special item: delicate scales, pearls, a waterstained map, 500–3,000 gold, a special fishing net, a lobster or crab, an SOS or a level 1–3 treasure map |
| 1% | Rusty loot: a rusty key or a rusty chest |
| 35% | A sea creature erupts from the water |

When the hotspot runs out, the last fisher gets a waterstained map, 3,000–8,000 gold, 15–40 delicate scales, a 40% chance for white pearls and a 25% chance for a special fishing net.

### Magic fish

| Fish | Effect |
|---|---|
| Prized Fish | +5 Int for 10 minutes |
| Wondrous Fish | +5 Dex for 10 minutes |
| Truly Rare Fish | +5 Str for 10 minutes |
| Peculiar Fish | Restores 10 stamina |

### Special fishing nets

A net pulls up sea creatures. With **Fishing above 100**, there's a chance of **1% per point** (10% at 110, 20% at 120) to pull up a **Legendary Kraken**.

### Waterstained treasure maps

- Maps are **level 1–5**. Double-click to reveal the chest. It lasts **2 hours**.
- The chest spawns **guardian waves** (waves = map level). Kill every wave before you open it.

| Level | Lockpicking |
|---|---|
| 1 | 50 |
| 2 | 80 |
| 3 | 100 |
| 4 | 105 |
| 5 | 110 |

Loot includes **1,000 gold × level** (plus Fortune), enhancement scrolls (25% × level), mastery items and mage items (15% × level each), imbuing resources, runic components and special loot. Your Fishing skill counts as luck for the chest.
During Sea Legends, a waterstained chest also gives **cargo points**. Opening one counts for the Treasure Hunt weekly task.

### Fisher's Guild

**Marina, the Fisher's Guildmaster**, collects sea finds. Drop them on her to log your progress and earn **Seafarer Reputation**, which you can spend in her shop.

| Collection | Reward |
|---|---|
| Rainbow Shells (every hue) | 500 reputation + a reward in your bank |
| Ancient Pottery (every shard) | 500 reputation + a restored vase |
| Regional Fish (one from every region) | 500 reputation + a rusty chest |
| Lost Sailors (every journal) | 1,500 reputation + a decoration |
| Prize fish | Record catches go on her leaderboard, by weight |

## Sea Legends

**Sea Legends** is a sea invasion that runs **twice a day**: once between 8 and 12 am and once between 4 and 8 pm (Eastern time). It rotates through Nordic Sea, Britain Sea, Compassion Sea, Delucia Sea and Cove Bay, and lasts **90 minutes** by default.

### Scoring

| Action | Points |
|---|---|
| Sea Legends sea creature | 5 |
| Legendary Pirate Captain | 50 |
| Cargo (waterstained chest) | 25 |
| Contest fish caught in the region | 3 |
| Boss (Dread Admiral) | 100 |

The boss spawns when the total score reaches **200** (set by staff) or at 75% of the contest time. Killing the boss ends the contest.

### The Sea Legend title

The top scorer becomes **Sea Legend** of that sea. They get these bonuses, and their guildmates get half:

| Bonus | Legend |
|---|---|
| Fishing speed | +15% |
| SOS chance | +5% |
| Fishing net chance | +5% |
| Boat and parrot XP | +20% |

### Contested waters

While an invasion is running, its sea is **contested**:

- No **Recall, Gate, Sacred Journey or Mark** out of it. You can only recall or gate *to* a spot on a boat.
- Boats have a 10% chance per move to hit a **hazard** (at most one per minute in the region, and one per 5 minutes per boat):
    - **scurvy**,
    - a **tidal wave** dealing 35–50 to everyone on deck within 6 tiles,
    - **eels and sea snakes** boarding the ship.
- Roaming **Legendary Pirates**, **sharks**, **drowned sailor ghosts** and **fishing hotspots** spawn across the seas.
