# Monthly Challenge

Every month has its own **Monthly Challenge**: earn **monthly challenge XP** from almost everything you do, and unlock that month's **20 rewards** along the way. Say **[Challenge** to see the current dungeon quest, or open the month's challenge window from the [Compendium](../core/compendium.md).

## Rewards

- Each month has **20 rewards** in **4 stages**, unlocked every **10,000 XP** up to **200,000 XP**. Claimed rewards go to your bank.
- Rewards are themed to the month: outfit pieces, a monthly pet egg, decorations, hued item tokens, a **title**, emotes, crafting benches and more. For example, October has Halloween outfit pieces, the October pet egg, pumpkins, a ghostly lantern and the title *The Creep*.
- Each month has its own **leaderboard**.
- XP is tracked per month, so a new month starts from zero.

## Earning monthly XP

| Activity | Monthly XP |
|---|---|
| **Killing monsters** | creature HP ÷ 200 (1–75 per kill; you must be within 30 tiles and able to earn XP) |
| Paragons, lesser bosses | +15 |
| Mini champion bosses | +25 (and 3 Achievement Points) |
| Dungeon bosses | +50 (and 5 Achievement Points) |
| Boss top-3 damage (10%+ of the damage) | 2,500 / 1,500 / 500 |
| Treasure map chest guardians | guardian HP ÷ 50, more with Lockpicking (up to +120%) |
| Daily quests, weekly tasks, global quests | see [Daily & Weekly](daily-weekly.md) and [Global Quests](global.md) |
| [Invasions](invasions.md), [Pit Trials](pit-trials.md) | based on your score |
| Fishing, prize fish, Fisher's Guild turn-ins, sea chests | various |
| Bulk orders, dungeon idols, escorts, event NPCs | various |

### Diminishing returns

All monthly XP is scaled down as your month's total grows:

```
multiplier = 0.85 − (this month's XP ÷ 1,000,000), never below 0.68
```

So you keep 85% of the XP early in the month, dropping to 68% from about 170,000 XP.

Other modifiers:

- **Haven** region: half XP.
- **Danger Zones:** kill XP is reduced by 25% (treasure map guardians aren't affected).
- **February:** +25% when you're near party or guild members.

## The dungeon quest

Each challenge runs in a **designated dungeon** that changes every **6 hours** (the window shows the countdown). Inside:

| Feature | What it gives |
|---|---|
| **Evolved creatures** | Some monsters are secretly evolved. Killing one gives HP ÷ 2 monthly XP (max 125), or all of its HP (max 250) while you have the Evolved bonus. |
| **Evolved mini-boss** | A much stronger mini-boss. Everyone with looting rights gets the **Evolved bonus** for 30 minutes. The top damager also gets **+500**. |
| **Evil Totems** | Destroy them for +5 each. |
| **Hidden treasure chests** | Walk near one to reveal it. Picking it summons guardians. The chest gives monthly XP equal to your Lockpicking + Luck bonus, and its loot improves with both. |

Totems and chests are refreshed every 30 minutes.
