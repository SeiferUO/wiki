# Template Manager

The **Template Manager** saves full skill-and-stat setups so you can switch between builds. Open it with **[template**. The manager is bound to you.

## Template slots

- Up to **9 slots**. Unlock them with **Platinum Coins**:

| Slot | Cost |
|---|---|
| 1st | 10 coins, and slot 2 unlocks free with it |
| after that | 10 + 10 × slots already unlocked |

- You can name templates (up to 15 characters).
- **Store** saves your current skills and stats into a slot. **Load** replaces all your skills and stats with the slot's.

## Loading rules

- **15 seconds** between switches.
- Not in a **dueling arena**, not during a **MOBA match**, and not while polymorphed.
- The template's stats can't total more than **230** (outside Sphere areas).
- Every skill must be within your current skill cap.
- Loading a template **dismisses your summons** and resets bard tempo.

## Combat template (PvP)

A special **Combat Template** slot can switch you automatically when PvP starts.

- Fill it by copying your current skills, or by copying one of your templates. Non-combat skills are filtered out.
- **[togglepvp** turns the auto-switch on or off. **[togglepvpwarning** asks you first ("Use your combat template?") instead of switching right away.
- When a player attacks you, or you attack one, you switch to the combat template:
    - Summons you couldn't control under it are dismissed.
    - Pets you couldn't control are told to stop.
- After **1 minute without combat**, your previous template comes back.
- It never triggers in dueling arenas, during MOBA, or against your friends.

## Dueling template

The dueling arena uses its own template:

- exactly **7 skills** at 100,
- stats totaling **225** (250 for Sphere), each between 10 and 125.

It's applied when the duel starts, and your previous template is restored afterward.
