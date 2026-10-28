# Enchanting & Crafting

How special properties get onto gear: the **Enchanting Table**, **Enhancement Scrolls**, and **crafting** with or without runic tools.
For what each property does and its limits, see [Gear Properties](gear-properties.md).

## Enchanting Table

Stand within 3 tiles of an **Enchanting Table** and target an item in your backpack. A window lists every property that item type can take.

**What can be enchanted:** weapons, armor, spellbooks and mage staves.

**What can't:**

- artifacts,
- newbied items,
- insured items (remove the insurance first),
- blessed items, unless the blessing comes from an active **Item Bless Deed**.

### Cost per point

Each +1 costs:

| | Cost |
|---|---|
| Gold | 500 (taken from your backpack, then your bank) |
| Arcane Dust | 25 |
| Imbuing material | 1 (it depends on the property, e.g. Fire Ruby for Weapon Damage, Daemon Claw for Savagery) |

- **Total mode** raises a property straight to its max in one click. It costs the same as raising it one point at a time.
- **Lowering** a property costs 500 gold per point, and you get nothing back.
- You can only add a **new** property if the item is under its property limit (3, or 4 for crafted items that came out with 4).
- The table can't go above a property's **item max**. Going over that takes an Enhancement Scroll (below).

## Enhancement Scrolls

Enhancement Scrolls come in four kinds: **Weapon, Armor, Spellbook** (also mage staves) and **Shepherd's Crook**. Each one is for a single property.

- A scroll adds **+1** to its property.
- Scrolls can push a property **past its item max ("overcap")** by 15% of the max, and always by at least +1.
    - Example: a property capped at 20 can be scrolled to 21.
- They follow the same item rules as the table: no artifacts, and blessed items only under an Item Bless Deed.
- They can only add a new property if the item has **fewer than 3** special properties.
- Scrolls of the same kind and property stack.

Scrolls drop from treasure chests, waterstained chests and other loot. Specific-property scrolls also exist as rewards.

## Degradation

**Only the overcap part degrades.** Anything at or below a property's item max is safe.

When you use an overcapped item, there's a chance it loses **1 point** of one overcapped property:

- Weapons when you fight, armor when you're hit, spellbooks when you cast, crooks when your pets fight.
- Harvesting and crafting can wear down Harvesting Luck and Crafting Luck. Opening treasure chests can wear down luck properties.
- There's a cooldown between two degradations *(set by staff)*.

Ways to protect it:

| Protection | Effect |
|---|---|
| **Arms Lore** | Chance to stop it: Arms Lore / 480 (25% at 120) |
| **Overcharge charges** | Each charge absorbs one degradation. Separate charges for weapons, armor and spellbooks. |
| Domination *Fortification* buff | Extra chance to stop it (Guild Militia) |

You get overcharge charges by turning in Enhancement Scrolls (1 charge per scroll, matching type) or from an **Overcharging Token** (+5 of each type).

## Crafting

Crafted weapons, armor, spellbooks and mage staves roll special properties when made. Artifacts never do: they have preset properties instead (see [Artifacts](artifacts.md)).

### Quality

| Step | Chance |
|---|---|
| **Exceptional** | Normal crafting rules |
| **Exceptional → Mastercrafted** | Arms Lore above 50 (up to 7% at 120) + crafting skill above 90 (up to 8% at 120) + Artisan mastery (up to about 15%) + **15% with a runic tool** |

Mastercrafted items get extra properties (see below). Your crafting message tells you your Mastercrafted chance.

**Artifacts** you craft can still turn Exceptional: +1% per point of Arms Lore and crafting skill above 100, plus Artisan.

### Durability

Crafted weapons and armor get **50–75 HP**, plus:

- +20 Exceptional or +40 Mastercrafted,
- +1 per Artisan level,
- +1 per 10 Arms Lore,
- +10 / 25 / 40 / 60 / 80 for Durable / Substantial / Massive / Fortified / Indestructible.

The total is capped at 255.

### Weapons

Arms Lore adds **Damage Increase**: +1 per 12.5 skill (8 at 100, 9 at 120).

**Colored metal or wood (no runic)** gives a durability level:

| Durability | Metals / woods |
|---|---|
| Durable | Dull Copper, Shadow Iron, Oak, Ash |
| Substantial | Copper, Bronze, Yew |
| Massive | Gold, Agapite, Heartwood |
| Fortified | Verite, Valorite, Bloodwood |
| Indestructible | Azurite, Frostwood |

**Special properties:**

| Tool | Properties | Value |
|---|---|---|
| Regular tool | **1** (2 if Mastercrafted) | Random, up to the property's item max |
| Runic tool | the runic's attribute count − 1, between 1 and 3 | Random, up to the item max |

Runic tools and Mastercrafted weapons also get a random **slayer**: Exorcism, Troll Slaughter, Arachnid Doom, Dragon Slaying, Repond, Elemental Ban or Ogre Trashing.

**Runic levels** (the runic must match the material):

| Runic | Durability | Damage | Accuracy |
|---|---|---|---|
| Dull Copper / Oak | Durable | — | Accurate |
| Shadow Iron / Ash | Durable | Ruin | — |
| Copper / Yew | Fortified | Ruin | Surpassingly |
| Bronze / Heartwood | Fortified | Might | Surpassingly |
| Gold / Bloodwood | Indestructible | Force | Eminently |
| Agapite / Frostwood | Indestructible | Power | Eminently |
| Verite | Indestructible | Power | Exceedingly |
| Valorite | Indestructible | Vanquishing | Exceedingly |
| Azurite | Indestructible | Vanquishing | Supremely |

Shepherd's Crooks roll from the [crook property list](gear-properties.md#shepherds-crook) instead.

### Mage staves

Staves roll spellbook properties. The wood sets the strength (a % of each property's max) and the count:

| Wood | Regular tool | Runic tool |
|---|---|---|
| Oak | 15%, 1 property | 40%, 1 |
| Ash | 25%, 1 | 55%, 1 |
| Yew | 35%, 1 | 65%, 1–2 |
| Heartwood | 50%, 1–2 | 75%, 2–3 |
| Bloodwood | 65%, 1–2 (2–3 Mastercrafted) | 80–100%, 3 |
| Frostwood | 80%, 2–3 (3 Mastercrafted) | 80–100%, 3–4 |

### Armor

**Regular tool:** **2 properties** (3 if Mastercrafted), each 1–5.

**Runic tool** (must match the material):

- Properties: the runic's attribute count − 1, between 1 and 3, each 1–5.
- Exceptional or Mastercrafted pieces also get protection and durability levels:

| Runic | Protection | Durability |
|---|---|---|
| Dull Copper, Spined, Oak | Defense | Durable |
| Shadow Iron | Defense | Substantial |
| Copper, Horned, Ash | Guarding | Substantial |
| Bronze, Yew | Guarding | Massive |
| Gold, Barbed, Heartwood | Hardening | Massive |
| Agapite, Bloodwood | Hardening | Fortified |
| Verite, Scaled, Frostwood | Fortification | Fortified |
| Valorite | Fortification | Indestructible |
| Azurite | Invulnerability | Indestructible |

### Runic tool tiers

A better runic mainly gives **more properties** (and better protection, damage and durability levels). It barely changes the property values themselves.

| Runic | Attributes | Intensity |
|---|---|---|
| Dull Copper | 1–2 | 10–35 |
| Shadow Iron | 2 | 20–45 |
| Copper | 2–3 | 25–50 |
| Bronze | 3 | 30–65 |
| Gold | 3–4 | 35–75 |
| Agapite | 3–4 | 40–80 |
| Verite | 3–5 | 45–90 |
| Valorite | 4–5 | 50–100 |
| Azurite | 4–5 | 80–100 |
| Spined | 1–3 | 20–40 |
| Horned | 3–4 | 30–70 |
| Barbed | 3–5 | 40–100 |
| Scaled | 4–5 | 70–100 |
| Oak | 1–2 | 1–50 |
| Ash | 2–3 | 35–75 |
| Yew | 2–3 | 40–90 |
| Heartwood | 2–4 | 50–100 |
| Bloodwood / Frostwood | 3–4 | 50–100 |

### Spellbooks

Inscribed spellbooks roll spellbook properties based on your **Magery + Inscription**:

| Magery + Inscription | Properties |
|---|---|
| under 150 | 1–2 |
| 150+ | 2–3 |
| 175+ | 2–4 |
| 200+ | 3–4 |

- **Strength** = (Magery + Inscription) / 235, max 100% of each property's range (reached at 235).
- Half the time, one of the properties is a summon-spell property. A book never gets more than one.
- Crafted books also get a random slayer and 100 durability.
