# Druidic Mastery

The **Nature** mastery. Druids shapeshift into creatures based on the weapon they hold. Each form has its own buff, passive and special ability.

General mastery rules (leveling, orbs, Arcane Dust) are on the [Masteries](index.md) page.

!!! note
    Numbers marked *default* come from the Mastery Balance controller and can be changed by staff.

## How it works

1. Activate Nature mastery and open the **stance window**.
2. Pick a stance. You **shapeshift** into that creature. Which stances you see depends on what you hold:
    - **Melee weapon:** melee stances.
    - **Bow or crossbow:** archery stances.
    - **Wizard staff or spellbook:** mage stances.
3. While shapeshifted you move at **mounted speed** on foot.
4. Choosing *Human* returns you to normal. Dying also ends the form.

### Stance switching

- Cooldown between stance changes: **60 s − 0.25 s per Nature level**.
- Every switch gives a temporary **stance buff**:

    ```
    buff = 5% + up to 25% more with level (max 30%)
    duration = 30 s + 2 s per Nature level
    ```

    Casting speed and spell damage buffs are half as strong and last half as long.

### Special ability gauge

Damage you deal to monsters fills a gauge. When it's full, you can unleash your stance's special ability.

```
gauge = 1,000 − 50 per Nature level   (min 250 damage)
```

## Melee stances

| Stance | Switch buff | Passive | Special ability |
|---|---|---|---|
| **Tiger** | Accuracy | +5% damage and more with level | Brutal flurry: 3 rapid strikes (100%, 75%, 56% damage) |
| **Ram** | Melee damage (max 30%) | 10% damage resistance + level | Charge toward an enemy from range |
| **Ophidian** | Critical chance (crits deal +35%) | Poison resistance | Whirlwind hitting up to 5 enemies several times |
| **Crab** | Attack speed | +10 + level HP regen points (PvM) | Shell shield: 100 + 25 per level HP (max 250) |
| **Terathan** | Cures your poison | Chance to poison (Lesser to Deadly by Poisoning skill) | Poisons the enemy, or deals double damage if it's already poisoned |
| **Peacock** | Heals 15% of your HP (up to 30%) | **Faster swings**: 5% + 1% per level (max 25%) | Lightning tempest in an area |

## Archery stances

Each switch into an archery stance gives you **5 special ammo** for that stance.

| Stance | Switch buff | Passive | Ammo / special |
|---|---|---|---|
| **Purger** | Projectile damage | Chance to ignore armor (adds half the monster's armor as damage) | Toxic shot that bypasses armor |
| **Worm** | Attack speed | 10% damage resistance + level | Bleeding shots |
| **Bug** | Cures your poison | Poison resistance | Acid spray in a cone |

## Mage stances

| Stance | Switch buff | Passive | Special ability |
|---|---|---|---|
| **Ophidian Mage** | Restores mana | 10% damage resistance + level | Lightning tempest in an area |
| **Drakeling** | Spell damage | Chance to set monsters burning (7.5% + level, max 30%) | Wave of fire |
| **Gargoyle** | Casting speed | Chance for spells to surge (+30% damage) | Barrage of Stygian fireballs on one target |

## Tamer role

With a Shepherd's Crook (or empty hands), Nature is a pet-support mastery:

- **Veterinary is stronger** on your pets: +0.5% per level, max +15%.
- Pets can **surge**, regenerating a large amount of HP, mana and stamina.
- Pet resurrection heals more: +1% per Nature level.

## Other Nature bonuses

- Summons get +1 per level, max +30.
