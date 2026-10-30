# Crafting

Double-click a crafting tool (smith's hammer, saw, sewing kit, tinker's tools, scribe's pen and so on) to open the crafting window.

What crafted weapons, armor, staves and spellbooks roll (quality, durability, properties and runic tiers) is on [Enchanting & Crafting](../items/enchanting-crafting.md#crafting).

## The crafting window

Pick a **category** on the left, then an item on the right. Click the **arrow** next to an item to make one, or the **page** icon for its details.

Two extra categories:

- **Last Ten:** the last 10 items you made.
- **Quest Items:** up to 10 items your active [weekly tasks](../quests/daily-weekly.md#weekly-tasks), [global quest](../quests/global.md) or guild quest need, with the material they need.

Item names are colored:

| Color | Meaning |
|---|---|
| **Purple** | Needed for one of your quests |
| **Red** | Needs a recipe you haven't learned |
| **Gold** | Needs a recipe you've learned |
| **Blue** | You can still gain skill making it |

### Item details

The details page shows your **success chance**, your **exceptional chance**, the skills needed, and a materials table with what's **required**, what's in your **backpack**, and what's in nearby **storage**.

| Button | Effect |
|---|---|
| **Make Now** | Makes one |
| **Make Number** | Asks how many, then makes them one after another |
| **Make Max** | Keeps crafting until you run out of materials or press **Cancel Make** |

When a tool wears out during a run, you automatically grab another one of the same kind from your backpack. This never happens with runic tools.

A **runic tool** only works with **its own material**. A Valorite runic hammer needs Valorite ingots, for example.

## Buttons

| Button | Effect |
|---|---|
| **Material** (bottom left) | Choose which metal, wood, leather or scales to use |
| **Make Last** | Makes the last item again |
| **Repair Item** | Repairs a damaged item of this craft |
| **Mark Item** | Choose whether your name goes on exceptional items |
| **Salvage** | Turns magic loot into **Arcane Dust** (see below) |
| **Recycle** | Turns weapons, armor or clothing back into materials (see below) |
| **Smelt Item** | Melts metal items back into ingots |
| **Cancel Make** | Stops a Make Number or Make Max run |

### Salvage

Target a magic item, a bag, or yourself (your whole backpack) to turn **magic loot** into **Arcane Dust**. Stronger properties give more dust.

It skips:

- player-crafted items, clothing and wands,
- blessed, insured and newbied items,
- artifacts and Doom set pieces,
- the items in your last-used list.

You can't salvage in combat. To get only dust and no enchanting materials, turn on **Ignore enchanting materials** in your [options](../core/options.md).

### Recycle

Target a weapon, armor or clothing piece in your backpack, or a bag to recycle everything in it. You get back about **20%** of the materials it takes to make (+0.5% per [Artisan](../masteries/index.md#artisan-crafting-power) level), in the same metal, wood or leather.

Blessed, insured and newbied items and artifacts can't be recycled.

## Using your storage

Standing within **2 tiles** of a [Resource Storage](../items/storage.md) you can use, the window shows a toggle under **Crafting Focus**:

- **Backpack:** materials come from your backpack.
- **Storage:** materials come straight from the storage.

## Output container

Inside a house, the **OUTPUT** button lets you pick a container in that house for your crafted items. While you stay in the house, everything you make goes there. Outside it, items go to your backpack as usual.

- The container must be in the same house, and you need access to it.
- Trash containers can't be used.

## Crafting Focus

**Crafting Focus**, at the bottom of the window, sends each item you make straight to a task. Use the arrows to switch:

| Focus | What happens to crafted items |
|---|---|
| **None** | They stay in your backpack |
| **BOD Book** | They fill matching bulk orders in your BOD book |
| **Weekly Quest** | They count toward your [weekly tasks](../quests/daily-weekly.md#weekly-tasks) |
| **Global Quest** | They count toward the active crafting [global quest](../quests/global.md) |
| **Guild Quest** | They count toward your guild's crafting quest |

## Exceptional chance bonuses

These all add to your exceptional chance:

| Source | Bonus |
|---|---|
| [Artisan mastery](../masteries/index.md#artisan-crafting-power) | 2.5% + 1% per level |
| **Crafting Luck** ([gear](../items/gear-properties.md) and [runes](../items/ankhs-runes.md)) | 1% per point |
| Crafting talisman | Its exceptional bonus, for its own craft |
| [Guild](../core/guilds.md) exceptional chance buffs | Per buff level |
| **Master Chef's Apron** | Its bonus |
| **Woodworker's Bench** | +30% for its craft |

## Recipes

Some items need a **recipe**. Double-click a recipe scroll to learn it. Once learned, the item turns from red to gold in the crafting window.
