# Commands : daily
## Usages :
- `<prefix>daily` : Daily reward claimable every 24 hours (with a claim window of max 24 hours)
- `<prefix>daily streak` : Streak tracking (current and best) and streak advantages

`<prefix>` = Current bot prefix (default : `!`)

## System Logic :
### Daily Reward :
The **daily reward** can range from **1** to **250 🪙 coins** (with a **streak** longer than **50 days**, the max reward is **750 🪙 coins**).

**Streak advantages :**
- If your current streak is **longer** than **15 days**, you will get an additional **50% bonus** on the coins you earn.
- If your current streak is **longer** than **50 days**, you will get an additional **100% bonus** on the coins you earn, plus **250 🪙 extra coins**.

### Streak Recovery :
To recover your lost streak, a button will appear when you run the command `<prefix>daily streak`.

You can recover your lost streak if and only if you **have enough coins** (see 'Streak Recovery Price Scaling') and you **don't have** a new **streak** in progress of **more than 2 days**.

> [!CAUTION]
> If your **current streak** is **longer than 2 days**, you have **no way of recovering your lost streak**. 

### Streak Recovery Price Scaling : 
| From (day) | To (day) | Cost |
|--------|--------|--------|
| 1 | 5 | 500 🪙 |
| 6 | 20 | 400 🪙 |
| 21 | 50 | 300 🪙 | 
| 50 | Infinity | 250 🪙 |

There's no limit to the number of coins you will have to pay to get your lost streak back.
