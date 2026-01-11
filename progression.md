# Progression

Long-term progression systems that carry between games.

---

## Overview

| System | Currency | Purpose |
|--------|----------|---------|
| Prestige | Levels + PP | Permanent stat bonuses |
| Permanent Upgrades | Prestige Points (PP) | Specific gameplay boosts |
| Research Lab | Prestige Points (PP) | Unlock turrets/features |
| Achievements | N/A (awards PP) | Milestones and challenges |
| Daily Rewards | N/A (awards PP) | Login streak bonuses |

---

## Prestige System

### Requirements
- Reach **wave 50** in a single game
- Maximum prestige level: **50**

### How to Prestige
1. Reach wave 50+
2. Open pause menu or wait for game over
3. Click "Prestige" button
4. Confirm to reset and earn bonuses

### Per-Level Bonuses

Each prestige level gives:

| Bonus | Amount Per Level |
|-------|-----------------|
| Starting Credits | +10% |
| Starting Lives | +1 per 5 levels |
| Interest Rate | +0.5% |
| Sell Value | +1% |
| Global Damage | +2% |

**Example at Prestige 10:**
- +100% starting credits (3,000 instead of 1,500)
- +2 starting lives (22 instead of 20)
- +5% interest rate (10% instead of 5%)
- +10% sell value (85% instead of 75%)
- +20% global damage

### Prestige Milestones

| Level | Title | Special Reward |
|-------|-------|----------------|
| 1 | Initiate | Plasma Mortar unlocked |
| 3 | Defender | Laser Beam unlocked |
| 5 | Guardian | Temporal Field unlocked |
| 10 | Commander | Singularity unlocked |
| 15 | Elite | +50% prestige point earnings |
| 25 | Legend | +10% turret range |
| 30 | Veteran | +25% interest cap |
| 35 | Master | +5% critical strike chance |
| 40 | Champion | +10% wave completion bonus |
| 45 | Ascendant | +1 turret level bonus |
| 50 | Immortal | +1 additional turret level (total +2) |

### Prestige Points Earned

**From prestiging (wave 50+):**
```
(wave - 50) x 10 PP
```

**From game over (wave 10+):**
```
(scoreBonus + waveBonus) x prestigeMultiplier

Where:
- scoreBonus = log10(score + 1) x 150
- waveBonus = floor(waves / 10)
- prestigeMultiplier = min(1 + prestige x 0.1, 3.0)
```

The multiplier caps at 3x when you reach prestige 20.

---

## Permanent Upgrades

Spend Prestige Points on permanent bonuses that apply to all future games.

### All Upgrades

| Upgrade | Effect Per Level | Max Level | Base Cost | Multiplier |
|---------|-----------------|-----------|-----------|------------|
| Core Reinforcement | +1 life | 10 | 50 PP | 1.5x |
| Investment Returns | +15% interest cap | 10 | 40 PP | 1.4x |
| Turret Efficiency | -5% turret cost | 5 | 75 PP | 2.0x |
| Critical Strike | +2.5% crit chance | 10 | 60 PP | 1.6x |
| Shield Breaker | +8% shield damage | 5 | 80 PP | 1.8x |
| Quick Start | +1 free starting turret | 3 | 200 PP | 3.0x |
| Salvage Master | +4% sell value | 10 | 50 PP | 1.5x |
| Wave Bonus | +5 credits per wave | 10 | 30 PP | 1.3x |

### Cost Formula
```
cost = baseCost x costMultiplier^currentLevel
```

### Example Costs

**Core Reinforcement (50 PP base, 1.5x):**
| Level | Cost | Total Invested |
|-------|------|----------------|
| 1 | 50 | 50 |
| 2 | 75 | 125 |
| 3 | 112 | 237 |
| 4 | 168 | 405 |
| 5 | 253 | 658 |
| 10 | 1,924 | 5,765 |

### Recommended Priority

1. **Investment Returns** - More income every game
2. **Core Reinforcement** - Survive longer, earn more PP
3. **Wave Bonus** - Cheap, consistent income boost
4. **Salvage Master** - Enables flexible strategies
5. **Critical Strike** - Reliable damage increase
6. **Shield Breaker** - Helps vs late-game shields
7. **Turret Efficiency** - Expensive but saves credits
8. **Quick Start** - Very expensive, marginal benefit

---

## Research Lab

Idle research that progresses in real-time, even when offline.

### Research Tree

```
TIER 1 (No prerequisites)
├── Plasma Mortar (2h, 200 PP)
└── Laser Beam (3h, 250 PP)
         │
         ▼
TIER 2
├── Temporal Field (6h, 600 PP) ← requires Laser Beam
│
└── Singularity (8h, 1000 PP) ← requires Mortar + Temporal
              │
              ▼
TIER 3
├── MOAT Flamethrower (24h, 3000 PP) ← requires Singularity
└── Quantum Core (36h, 3500 PP) ← requires Singularity
```

### Research Items

| Item | Time | Cost | Prerequisites | Unlocks |
|------|------|------|---------------|---------|
| Plasma Mortar | 2 hours | 200 PP | None | Plasma Mortar turret |
| Laser Beam | 3 hours | 250 PP | None | Laser Beam turret |
| Temporal Field | 6 hours | 600 PP | Laser Beam | Temporal Field turret |
| Singularity | 8 hours | 1000 PP | Mortar + Temporal | Singularity turret |
| MOAT Flamethrower | 24 hours | 3000 PP | Singularity | MOAT turret |
| Quantum Core | 36 hours | 3500 PP | Singularity | Reactor shield |

### Quantum Core Shield

Once researched, your reactor core gains a regenerating energy shield:
- Absorbs damage before lives are lost
- Regenerates between waves
- Can be restored with Shield Burst powerup

**Note:** All turrets are available from the start of the game. Research provides an alternate unlock path.

---

## Achievements

Earn Prestige Points by completing challenges.

### Wave Achievements (Single Game)

| Achievement | Requirement | Reward |
|-------------|-------------|--------|
| First Steps | Reach wave 10 | 100 PP |
| Getting Started | Reach wave 25 | 250 PP |
| Halfway There | Reach wave 50 | 500 PP |
| Centurion | Reach wave 100 | 1,000 PP |
| Marathon Runner | Reach wave 250 | 2,500 PP |
| Endurance Master | Reach wave 500 | 5,000 PP |

### Kill Achievements (Total)

| Achievement | Requirement | Reward |
|-------------|-------------|--------|
| Rookie Hunter | Kill 1,000 enemies | 10 PP |
| Seasoned Hunter | Kill 10,000 enemies | 50 PP |
| Elite Hunter | Kill 100,000 enemies | 200 PP |
| Legendary Hunter | Kill 1,000,000 enemies | 1,000 PP |

### Turret Achievements

| Achievement | Requirement | Reward |
|-------------|-------------|--------|
| Pulse Master | Max level a Pulse Cannon | 15 PP |
| Scatter Master | Max level a Scatter Shot | 15 PP |
| Rail Master | Max level a Rail Gun | 15 PP |
| Cryo Master | Max level a Cryo Emitter | 15 PP |
| Tesla Master | Max level a Tesla Coil | 15 PP |
| Arsenal | Build every turret type | 50 PP |
| Full Arsenal | Unlock all turrets via research | 25 PP |

### Perfect Wave Achievements

| Achievement | Requirement | Reward |
|-------------|-------------|--------|
| Flawless Start | Survive 5 waves without losing a life | 20 PP |
| Impenetrable | Survive 25 waves without losing a life | 100 PP |
| Untouchable | Survive 50 waves without losing a life | 250 PP |
| Perfect Streak | 10 waves in a row without losing a life | 75 PP |

### Boss Achievements

| Achievement | Requirement | Reward |
|-------------|-------------|--------|
| Boss Slayer | Defeat first boss | 15 PP |
| Boss Hunter | Defeat 10 bosses | 50 PP |
| Boss Vanquisher | Defeat 50 bosses | 200 PP |
| Boss Annihilator | Defeat 100 bosses | 500 PP |
| Titanfall | Defeat a Titan | 100 PP (hidden) |

### Special Achievements

| Achievement | Requirement | Reward |
|-------------|-------------|--------|
| First Game | Play your first game | 5 PP |
| Regular Player | Play 10 games | 15 PP |
| Dedicated | Play 50 games | 50 PP |
| Committed | Play 100 games | 100 PP |
| Obsessed | Play 500 games | 500 PP |
| Reborn | Prestige for the first time | 25 PP |
| Ascendant | Reach prestige 5 | 100 PP |
| Transcendent | Reach prestige 10 | 250 PP |
| Legendary | Reach prestige 25 | 500 PP |
| Immortal | Reach prestige 50 | 1,000 PP |
| Week Streak | Log in 7 days in a row | 50 PP |
| Month Streak | Log in 30 days in a row | 200 PP |
| High Scorer | Score 10,000 | 20 PP |
| Score Master | Score 100,000 | 100 PP |
| Million Club | Score 1,000,000 | 500 PP |
| Purist | Reach wave 20 with only Pulse Cannons | 75 PP (hidden) |

---

## Daily Rewards

Log in each day to claim Prestige Points.

### Base Reward
**10 PP** per day

### Streak Bonus
+5 PP for each consecutive day (max +35 at 7 days)

| Streak | Daily Reward |
|--------|--------------|
| Day 1 | 10 PP |
| Day 2 | 15 PP |
| Day 3 | 20 PP |
| Day 4 | 25 PP |
| Day 5 | 30 PP |
| Day 6 | 35 PP |
| Day 7+ | 45 PP |

**Formula:** `10 + min(streak, 7) x 5`

Missing a day resets your streak to 0.
