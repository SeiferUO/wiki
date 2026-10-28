# Taming

For loyalty, bonding, pack instinct and pet combat, see [Creatures](../core/creatures.md#pets).

## Animal Taming

- You can only attempt a tame if your **Animal Taming is at or above** the creature's taming requirement.
- **Success chance:**

    ```
    chance = (Animal Taming − requirement + 25) / 50
    ```

- A tame takes **3–4 rounds of 3 seconds**. It fails if:
    - the creature takes damage,
    - you move more than 6 tiles away,
    - you lose line of sight, or it can't walk to you.
- Creatures you've owned before are always re-tamed successfully.
- Some creatures must be **beaten below 10% HP** first, unless they've been tamed before.
- Some creatures may get angry and attack instead.
- You need enough free follower slots.
- Skill delay: up to 40 s, reset as soon as the attempt ends.
- Every successful new tame adds to your **Tamer Score**.

Each taming round also gives Animal Lore skill gains.

### Gaining Taming by hunting

You can also train Animal Taming just by **killing monsters with your pets**. Each monster kill you get credit for, while you have a pet out, is a chance to gain **0.1–0.2 Animal Taming**.

- The chance is higher at **low skill** and against **stronger monsters**.
- Very weak monsters give half the chance once you reach 70 Taming.
- Every kill without a gain raises your next chance by **+2%**, until you gain.
- Summons, golems and hirelings don't count as pets for this.
- Your skill must be set to go up, and you need room under your skill cap.

## Controlling pets

- You need **Animal Taming and Animal Lore both at or above** the pet's requirement to control it.
- Pets with a requirement of 29.1 or lower always obey.

## Animal Lore

- You can lore a creature if your **Animal Lore is at or above** its taming requirement.
- Success chance: **50% + Animal Lore**, so 50+ Lore always succeeds.
- Unchained pets open their full management window instead.

## Golems

Golems don't use taming. You need **200 combined points** of Item Identification, Tinkering, Remove Trap and Detect Hidden to control one.
