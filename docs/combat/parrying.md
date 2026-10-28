# Parrying & Shields

A shield gives you a chance to **block most of an incoming weapon hit**. Your **Parrying** skill decides how often you block, how much armor the shield gives and how well you can taunt monsters with it.

## Blocking with a shield

Every weapon hit against you, melee or ranged, from a player or a monster, rolls for a parry if you have a shield equipped:

```
chance = Parry × 0.2%  +  shield AR × 0.25% (max 20%)
```

| Bonus | Amount |
|---|---|
| **Failed-parry streak** | +5% after each failed parry, up to +15%. Needs 50+ Parry. Any successful parry resets it |
| **Iron Guard** ([Swordsmanship codex](../codex/weapon-codex.md#swordsmanship)) | +2% per tier, **PvM only** |
| **Bulwark** mastery | more parry chance by mastery level *(set by staff)* |

- **Max chance: 65%.** Min chance: 1%.
- **A successful parry blocks 65% of the hit.** You take the other 35%.
- Each parry attempt can raise your Parrying skill.

At 120 Parry with a 20% shield bonus and a full failed-parry streak, you reach 24% + 20% + 15% = **59%**.

### What else happens on a parry

- **Mana Barrier** (Wizard stance): part of the blocked damage becomes mana. See [Wizard](../masteries/wizard.md).
- **Shield Bash** (Swordsmanship and Macing codex): bashes and freezes the attacker. See [Weapon Codex](../codex/weapon-codex.md).
- **Monster abilities:** a successful parry against a monster's special ability lowers its damage by 20–35%. See [Creatures](../core/creatures.md#monster-abilities).

## Shield armor rating

A shield's armor rating (AR) starts from its base value, then:

| Modifier | Change |
|---|---|
| Low quality | −10% |
| Exceptional | +20% |
| Protection level (Defense → Invulnerability) | +10% per level, up to +50% |
| Metal | +2% (Dull Copper) up to +18% (Azurite), +2% per metal tier |
| Damage | up to −20% as durability drops |

Then your Parrying scales it:

```
shield AR = AR × (50% + 50% × Parry / 100)
```

So you get half the AR with 0 Parry, the full AR at 100 Parry and 110% at 120. The same AR feeds the parry chance above (0.25% per point, max 20%) and the taunt chance below.

## Parrying with a two-handed weapon

No shield? Against **monsters**, a two-handed weapon can parry too:

```
chance = (Parry − 50) / 100      (min 1%)
```

A successful parry blocks **25%** of the hit, or **15%** if you're holding a bow or crossbow. This doesn't work against players.

## Shield Taunt

Double-click your equipped shield, or say **[taunt**, to pull monsters onto you. Staff can switch Shield Taunt off. It can't be used in Turret Defense.

| Target | Chance | Effect |
|---|---|---|
| **Yourself or the ground** (within 8 tiles) | (Parry + shield AR) ÷ 2 % per monster | Taunts up to the **3 closest** monsters within 8 tiles |
| **One monster** (within 8 tiles) | (Parry + shield AR) ÷ 1.5 % | Taunts that monster |

- Taunted monsters attack you and deal **15% less damage to you** (melee and spells) for **15 seconds**.
- **Cooldown:** 15 seconds after a success, 5 seconds after a failure.
- Only hostile monsters can be taunted. Pets, summons and turrets can't, and the monster must be in line of sight.
- Taunting reveals you.

## Casting and meditating with a shield

Staff decide whether shields allow these and how much skill you need:

- **Casting with a shield:** you can cast while holding a shield if it's enabled and you meet the Parrying and Focus requirements *(set by staff)*. Your other hand must be empty or hold a [mage staff](../magic/mage-staves.md). It can also be turned off during PvP.
- **Meditating with a shield:** if enabled, a shield doesn't stop Meditation once you meet the same requirements.

See [Player Character](../core/player.md) for how armor affects mana regeneration.

## Durability

- Each successful parry has a chance to cost the shield 1 durability *(set by staff)*.
- **Arms Lore** protects it: 2% per 10 points, so 20% at 100 and 24% at 120.
- Below 10% durability you get warnings. At 0 the shield is destroyed.
- Shield properties can also wear down when you're hit (see [Enchanting & Crafting](../items/enchanting-crafting.md)).

## Changing a shield's look

- **Change Style** (context menu, shield in your backpack): turn the shield into a **torch, lantern or candle** look for **5 Platinum Coins**. Or target a torch, lantern or candle in your backpack to copy its look and color. That light item is used up.
- **Shield Dye:** double-click it and target a shield in your backpack to give it the dye's color.
