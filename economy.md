# Economy

Understanding credits, income sources, and spending strategies.

---

## Starting Resources

| Resource | Base Value | Modified By |
|----------|------------|-------------|
| Credits | 1,500 | Prestige (+10% per level) |
| Lives | 20 | Prestige (+1 per 5 levels), Core Reinforcement upgrade |

---

## Income Sources

### 1. Kill Rewards

Every enemy killed gives credits based on type and wave.

| Enemy | Base Reward | Wave 50 Reward | Wave 100 Reward |
|-------|-------------|----------------|-----------------|
| Scout | 1 | 2 | 5 |
| Armored | 2 | 4 | 10 |
| Swarm | 1 | 2 | 5 |
| Shielded | 4 | 8 | 20 |
| Heavy | 8 | 16 | 40 |
| Stealth | 4 | 8 | 20 |
| Carrier | 6 | 12 | 30 |
| Boss | 50 | 100 | 250 |
| Titan | 100 | 200 | 500 |

**Scaling Formula:**
- Waves 1-49: `baseReward x (1 + wave x 0.02)`
- Waves 50+: `baseReward x (2 + (wave - 50) x 0.08)`

---

### 2. Wave Completion Bonus

At the end of each wave, you receive:

**Base Bonus:** `50 + (wave x 25)` credits

| Wave | Completion Bonus |
|------|-----------------|
| 1 | 75 |
| 10 | 300 |
| 25 | 675 |
| 50 | 1,300 |
| 100 | 2,550 |

---

### 3. Milestone Bonuses

Reaching certain waves gives extra credit bonuses:

| Wave | Bonus Credits |
|------|--------------|
| 5 | +100 |
| 10 | +250 |
| 15 | +400 |
| 20 | +600 |
| 25 | +1,000 |
| 50 | +2,500 |
| 75 | +5,000 |
| 100 | +10,000 |

---

### 4. Interest

At the end of each wave, you earn **5% interest** on your current credits.

**Base Interest Cap:** 500 credits per wave

**Increasing the Cap:**
- Investment Returns upgrade: +15% cap per level (10 levels max)
- Large Cap powerup: 2x cap for one game
- Prestige 30 (Veteran): +25% cap

**Example:**
- 10,000 credits with base cap = 500 interest
- With max Investment Returns (+150%): cap becomes 1,250
- With Prestige 30 (+25%): cap becomes 1,562

---

### 5. Wave Bonus Upgrade

The Wave Bonus permanent upgrade adds flat credits per wave:

| Level | Bonus Per Wave |
|-------|---------------|
| 1 | +5 |
| 2 | +10 |
| 3 | +15 |
| ... | ... |
| 10 | +50 |

---

## Spending

### Turret Costs

See [Turrets](turrets.md) for all costs. Range from $150 (Pulse) to $25,000 (MOAT).

### Turret Efficiency Upgrade

Reduces turret costs by 5% per level (5 levels max = 25% discount).

| Level | Discount |
|-------|----------|
| 1 | -5% |
| 2 | -10% |
| 3 | -15% |
| 4 | -20% |
| 5 | -25% |

---

## Selling Turrets

You can sell placed turrets for a percentage of your total investment.

**Base Sell Value:** 75% of total spent (purchase + all upgrades)

**Increasing Sell Value:**
- Salvage Master upgrade: +4% per level (10 levels = +40%)
- Prestige bonus: +1% per prestige level

**Example:**
- Level 6 Pulse Cannon total cost: 150 + 180 + 270 + 600 + 1,200 + 2,400 = 4,800
- Base sell: 4,800 x 0.75 = 3,600
- With max Salvage Master (+40%): 4,800 x 1.15 = 5,520 (capped at 100% + bonuses)

---

## Economy Strategies

### Early Game (Waves 1-20)
1. **Start with 2-3 Pulse Cannons** - don't overspend
2. **Save some credits** - interest starts building
3. **Upgrade to level 2-3** - better than more turrets
4. **Hit milestone waves** for bonus income

### Mid Game (Waves 21-50)
1. **Push turrets to level 4+** - major power spikes
2. **Let interest build** between waves
3. **Balance saving and spending** - don't hoard excessively
4. **Invest in Investment Returns** upgrade early

### Late Game (Waves 51+)
1. **Max out key turrets (level 6)** - huge stat boosts
2. **Interest cap matters more** - upgrade it
3. **Sell and rebuild** when strategies need adjustment
4. **Use credit powerups** strategically

---

## Economic Math

### Interest vs Spending

**Question:** Should I save for interest or spend now?

**Answer:** Generally spend if:
- You're near interest cap already
- You're struggling to survive
- The upgrade gives a major power spike (level 4+)

Save if:
- You're comfortably surviving
- You're nowhere near interest cap
- Next upgrade is incremental

### Sell/Rebuy Efficiency

With base 75% sell return:
- Rebuilding costs 25% of investment
- Only worth it for major strategy changes
- Better with Salvage Master upgrade

With max Salvage Master (115% return):
- Actually profitable to sell!
- Enables flexible repositioning

---

## Quick Reference

| Stat | Base Value |
|------|------------|
| Starting Credits | 1,500 |
| Starting Lives | 20 |
| Interest Rate | 5% |
| Interest Cap | 500 |
| Sell Return | 75% |
| Wave Bonus Base | 50 + wave x 25 |
