# Wizard

The mage side of the mastery system: the **Wizard Mastery** item, the mastery gauge, the wizard staff gauge and **mage stances**.

General mastery rules (leveling, orbs, Arcane Dust) are on the [Masteries](index.md) page.
The promoted spell rotation is on [Spell Promotion](../magic/spell-promotion.md).

!!! note
    Numbers marked *default* come from the Wizard Stance controller and can be changed by staff.

## Who counts as a mage

Mage abilities need one of these in hand: a **spellbook**, a **wand**, or a weapon or shield with **Spell Channeling** or **Mage Weapon**.
A Shepherd's Crook always makes you a tamer instead.

**Pure mage** features (promoted spells and the strongest stances) also need:

| Requirement | Value |
|---|---|
| Magery **or** Necromancy | 100 |
| Evaluating Intelligence | 100 |
| Focus + Meditation + Spirit Speak + Mysticism | 150 combined |

## Mastery gauge

Every damaging spell you land on a monster has a chance to add a **charge** to your mastery gauge (max 7):

| Spell circle | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 |
|---|---|---|---|---|---|---|---|---|
| Chance | 5% | 10% | 12% | 15% | 25% | 30% | 40% | 50% |

- Necromancy spells: 1.5% per point of mana cost.
- **Halved** if you have pets or summons out.
- Mastery level, Mastery Chance runes and guild buffs add more (max +30%).

At **5 charges**, your next damaging spell also releases your **mastery's mage ability** (see [Masteries](index.md#the-masteries)).
That uses **1 Arcane Dust** and resets the gauge.

## Wizard staff gauge

Each hit with a wizard staff adds **5 charge**. At **100**, your next staff hit on a monster adds a mastery charge and empties the staff gauge.

Staff damage scales with Evaluating Intelligence, Intelligence and Focus. Staves ignore monster armor, but the monster's Magic Resist reduces the damage. See [Mage Staves](../magic/mage-staves.md) for the damage formula and every mastery's staff effect.

## Mage stances

Pure mages with **no followers** can choose **two stances**:

- **Primary stance:** full effect.
- **Secondary stance:** **50%** effect.
- Changing a stance has a **30 second** cooldown.
- **Active stances** (marked ★) can only be your primary.
- Stances don't work in PvP or while you have pets, summons or golems out (and for 5 minutes after you summon).

| Stance | Effect *(default)* |
|---|---|
| ★ **Cleric** | Healing spells heal **+30%** on creatures and **+20%** on players |
| ★ **Burster** | **+25%** spell damage. Wand attacks may bounce to a nearby target |
| ★ **Illusionist** | 5% chance per spell circle to echo the spell for **+50% to +100%** damage |
| ★ **Geomancer** | 15% chance per spell circle to gain a shield worth 10% of the damage dealt (max 100) |
| ★ **Flowmancer** | 7.5% chance per spell circle to regain 25% of the damage dealt as mana |
| **Elusive Form** | After Teleporting, you evade spells and melee for **5 seconds** |
| **Mana Shield** | **30%** of incoming monster damage is taken from your mana instead |
| **Mana Barrier** | When you parry, 30% of the blocked damage becomes mana (max 15) |
| **Arcane Rebound** | When a spell fizzles: +10 mana and +10% damage on your next spell |
| **Candle of the Mind** | Below 30% mana, spells cost **20% less** |
| **Arcane Skin** | Each cast gives 1% resist against creature spells (10 stacks, 5 s each) |
| **Candleflame Insight** | Charges while you meditate (up to 30 s). Standing up gives up to **+30% spell damage** for 10 s |
| **Phoenix Spark** | Killing with a spell gives **+15% spell damage** for 8 s |
| **Umbral Reservoir** | Spell damage on poisoned, bleeding or holy-cursed targets restores 5 mana |
| **Cerebral Surge** | Resisting a spell restores 4 mana |
| **Thunderheart** | Lightning and energy spells have a 20% chance to give you Haste for 3 s |
| **Tidecaller** | Your field spells drift toward enemies |
