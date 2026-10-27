# Turret Defense

**Turret Defense** is a tower defense fun zone for **1 to 3 players**. Monsters march down a path toward your **Defense Core**. You hire mercenary turrets on stations along the path, upgrade them with **Turret Gold** and keep the core alive for as many waves as you can.

You don't fight yourself: players can't attack in the arena, and only turrets, bombs and fire deal damage.

## Starting and joining

- Double-click the **Turret Defense Stone** and press **Start Game**. You can tick **Private Game** to keep others out.
- While a public game is running, other players can double-click the stone to join, up to **3 players**. Two players on the same IP can't play together *(set by staff)*.
- Each game may cost a **Realm Defender Token** to start or join *(set by staff)*. Tokens drop as [rare loot](../items/rare-loot.md) and are also used for [Pit Trials](../quests/pit-trials.md).
- Every player starts with **100 Turret Gold**. You have a short preparation time *(set by staff, 1 minute by default)* before wave 1.
- Turret Gold only exists inside the game. It resets to 0 when you leave.

!!! warning "Leaving ends your game"
    Walking out of the arena or pressing the quit button on the status bar removes you from the game, destroys your turrets and wipes your Turret Gold. If the last player leaves, the game ends. Logging out inside the arena takes 10 minutes.

Travel and field spells (Recall, Gate, Mark, the field spells and Wall of Stone) don't work in the arena. Shield Taunt is disabled.

## Waves

- A new wave starts every **2 minutes** *(set by staff)*, whether the last one is dead or not.
- The game lasts **20 waves** by default *(set by staff)*. Survive them all for a victory.
- Monsters get stronger each wave. Each monster's level is the wave number **plus the number of players**, so more players means tougher monsters.
- More players also means more monsters: +50% per extra player.
- **Every 5th wave is a mini-boss wave:** a Goliath, an Oake (which comes with Silvani) or a Dread Spider Queen.
- **From wave 10**, surprise attacks can hit: 3 + 2 per player extra monsters, at most once every 5 minutes.

| Waves | Monsters |
|---|---|
| 1–9 | Easy: zombies, mongbats, slimes, bone magi, giant rats |
| 10–14 | Easy and medium mixed |
| 15–19 | Medium: orcs, air and ice elementals, imps, gargoyles, skeletons |
| 20–29 | Hard: liches, ettins, earth elementals, drakes, harpies |
| 30–39 | Elite: balrons, daemons, shadow dwellers, toxic and valorite elementals, dragons |
| 40–49 | Elite and legendary mixed |
| 50–59 | Legendary: ancient wyrms, cyclopes, ancient liches, blood elementals and more |
| 60–69 | Legendary and abomination mixed |
| 70+ | Abomination: fog, carrion lich, molten cyclops, pit fiend, titan, devourer |

### The Defense Core

When a monster gets within 2 tiles of the core, it vanishes and the core **loses HP equal to the monster's remaining HP**. The core shows its damage overhead. If it's destroyed, the game is over.

## Turret Gold

| Source | Gold |
|---|---|
| Starting gold | 100 |
| Your turret kills a monster | the monster's gold value: 1–10 (easy) up to 35–50 (abomination), 100 for mini-bosses |
| **Wave reward** (paid when the next wave starts) | 10 × wave × the share of the wave you killed, split between players, max 350 each. Nothing below 25% killed |
| **Gold Token** drop | walk over it for 5–15 gold |
| Selling a turret | half of what you spent upgrading it |

## Turrets

Double-click an unlocked **Turret Station** to hire a turret for **25 Turret Gold**. Each station holds one turret.

| Turret | Style | Special abilities |
|---|---|---|
| **Warrior** | Melee, short range | Level 3 power attack, 6 double strike, 9 whirlwind, 10 Massacre |
| **Archer** | Ranged | Level 3 quicksilver, 6 triple shot, 9 frenzy arrow, 10 arrow storm |
| **Fire Mage** | Fire spells | Level 6 flamestrike, 9 explosion, 10 explosion with fire trails. Kills have a 25% chance to leave a fire field |
| **Lightning Mage** | Lightning spells | Level 6 and 9 freezing lightning, 10 freeze and chain lightning |
| **Poison Mage** | Poison spells | Level 6 poison, 9 area poison, 10 poison plus Poisoning for nearby turrets |

- Special abilities have a cooldown of **60 s, 2 s shorter per level** (42 s at level 10).
- Mage turrets regenerate mana from level 3.

### Stations

- At the start of each game, **half the stations are free**. The rest are locked.
- From **wave 5** you can unlock a locked station with Turret Gold: **100** for the first, and the price **doubles** with each unlock.

### Leveling turrets

Turrets go from level 1 to **10**. Each level raises their stats, damage and gear.

- **XP** comes from the damage they deal and from kills (10 + 2 × wave per kill). A turret needs **150 × its level** XP to level up.
- **Upgrade** (double-click your turret): pay **25 gold, doubling each level** (25, 50, 100 … 6,400) for an instant level.
- **Damage bonus:** every 3 levels adds +25% damage for warriors and archers, or +30% spell damage for mages.
- **Claim Value** sells the turret back for half of what you spent upgrading it.

### Hunger, thirst and ailments

Turrets wear out as they fight:

- Each hit has a small chance (5% per level) to add **hunger** or **thirst**. Together they cut melee damage by up to 50%. Thirst also cuts XP gain by up to 50%.
- From **level 5**, hitting certain monsters can give a turret an ailment:

| Ailment | From | Effect | Cure |
|---|---|---|---|
| **Melting** | dragons, daemons, gargoyles, drakes, molten cyclops | loses 2% HP every 10 s | Vesper Water |
| **Illness** | liches, Dread Spider Queen, blood elementals, devourer | loses 2% HP every 10 s | Purification Elixir |
| **Frozen** | air and ice elementals | can't use special abilities | Everlasting Fire |
| **Blind** | shadow dwellers | — | Elven Glasses |

Ettins, earth elementals, cyclopes and titans can **repel** a hit, damaging the turret for 5% of its HP.

## Shop

Buy from the **Turret Defense Supplier** (double-click him) with Turret Gold. Items last **5 minutes** and are used on a turret.

| Item | Cost | Effect |
|---|---|---|
| Purification Elixir | 50 | Cures illness |
| Vesper Water | 50 | Cures melting |
| Everlasting Fire | 50 | Cures freezing |
| Elven Glasses | 50 | Cures blindness |
| Fruit Basket | 25 | Clears hunger |
| Bilgewater Ale | 25 | Clears thirst |
| Getafix's Potion | 100 | +25% Strength for 5 minutes |
| Lich Juice | 100 | 20 surging spells (+25% damage each, mage turrets) |
| Healing Kit | 50 | Heals 25% of max HP |
| Experience Flask | 500 | Instant level up |

## Monster drops

Monsters can drop items when they die (more often the more HP they have, up to 50%):

| Item | Effect |
|---|---|
| **Shop items** | any of the above except the Experience Flask, plus the **Power-Up Shroom** (+1 turret damage, up to 50) |
| **Wildfire Bomb** | Place it on the path; after 3 seconds it deals 15% of max HP to monsters within 4 tiles |
| **Toxic Bomb** | Place it on the path; after 3 seconds it poisons monsters within 2 tiles (Greater) |
| **Fire Field Orb** | Drops a fire field at your feet that burns monsters for 2.5–5% of their max HP |
| **Purifying Crystal** | Cures every ailment and halves hunger and thirst for all turrets within 12 tiles |
| **Gold Token** | 5–15 Turret Gold |
| **DefenseCore Repair Kit** | Heals the core 10%. 25% chance from monsters worth 100 gold (mini-bosses) |

## End of the game

When the game ends, win or lose, everyone is sent out of the arena and:

- You gain **Turret Levels** equal to the waves survived, for the leaderboard.
- **Reward roll:** a chance of **1% per wave ÷ number of players** for a random **toy**, placed in your bank box *(staff can switch rewards off)*.
- To qualify for the reward you must have dealt at least **20% of the median damage** of the group. Damage statistics are shown at the end.

## Leaderboard

The **Turret Defense Leaderboard** stone ranks the top 10 by **Total Levels**, **Games Played**, **Average Level** and **Best Run** (most waves in one game).
