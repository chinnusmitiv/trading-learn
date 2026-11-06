## Step 1: Capital Preservation — The Foundation

The first rule of trading: **protect capital before pursuing profit.** Without capital, you can't trade. The core model is the **Fixed Fractional Risk Model**:

- Risk a fixed **0.5%–2%** of total account equity per trade (most pros use 1%).
- This automatically shrinks position size after losses and grows it after gains (compounding).
- It prevents a single bad trade or losing streak from wiping out the account.

**Position Sizing Formula:**

```
Position Size (units) = (Capital × Risk %) ÷ (Entry Price − Stop-Loss Price)
```

**Example (₹5,00,000 account, 1% risk):**
- Max loss per trade = ₹5,000
- Entry = ₹500, Stop = ₹490 → Risk per share = ₹10
- Position size = 5,000 ÷ 10 = **500 shares**

Key principle: **Position size is derived from risk and stop distance — never chosen first.** A wider stop → fewer units; a tighter stop → more units.

---

## Step 2: R-Multiples — The Universal Unit of Measurement

Popularized by Van K. Tharp, the **R-multiple** normalizes every trade outcome to a single unit so you can compare results across different position sizes and instruments.

**Definition:**
- **1R** = the initial dollar risk on the trade (Entry − Stop) × position size.
- A **−1R** outcome = the stop was hit (you lost your full planned risk).
- A **+2R** outcome = you made 2× your initial risk.

**Example:**
| Exit Price | Rupee Result (250 shares, ₹10 risk/share) | R-Multiple |
|---|---|---|
| ₹1,400 (stop) | −₹5,000 | −1R |
| ₹1,430 | +₹2,500 | +0.5R |
| ₹1,460 | +₹10,000 | +2R |
| ₹1,480 | +₹15,000 | +3R |

**Expectancy in R:**

$$\text{Expectancy} = (\text{Win Rate} \times \text{Avg Win in R}) - (\text{Loss Rate} \times \text{Avg Loss in R})$$

Example: 40% win rate, avg win +2R, avg loss −1R →
$$0.40 \times 2 - 0.60 \times 1 = 0.80 - 0.60 = +0.20R \text{ per trade}$$

A positive expectancy means the system is profitable over a large sample. **This is the only real measure of edge** — not any single trade's dollar result.

---

## Step 3: Drawdown Controls — The Circuit Breakers

Drawdown is the peak-to-trough decline in equity. The recovery math is **asymmetric and brutal**:

| Drawdown | Gain Needed to Recover |
|---|---|
| 10% | 11.1% |
| 25% | 33.3% |
| 50% | 100% (double) |
| 75% | 300% |

This asymmetry is why **stopping a drawdown early is exponentially more valuable** than trying to recover from a deep one.

### The Three-Tier Drawdown Protocol

| Tier | Drawdown from Peak | Action |
|---|---|---|
| **1** | 0–5% | Normal variance. No changes. Keep trading the plan. |
| **2** | 5–15% | **Reduce position size by 50%.** Diagnose causes. Tighten entry filters. |
| **3** | 15%+ | **Cease all trading.** Full strategy review. Return to demo until profitable for 1 month. |

### Supporting Controls (layered)

| Layer | Rule | Purpose |
|---|---|---|
| Daily loss limit | Stop at 2–3R for the day (e.g., −3% of account) | Prevents revenge-trading spiral |
| Consecutive loss rule | Pause after 3–5 straight losses | Mental reset, check for regime change |
| Correlation cap | Total open risk across correlated positions ≤ 3% of account | Prevents one event from hitting multiple positions simultaneously |
| Volatility adjustment | Reduce size when ATR / market volatility spikes | Adapts risk to current conditions |

---

## Putting It All Together — The Daily Workflow

1. **Before the market opens:** Check equity vs. peak → determine your drawdown tier → set today's max risk per trade (1R value).
2. **When a setup appears:** Place the stop at the logical invalidation level first.
3. **Calculate size:** `Position = (Equity × Risk%) ÷ Stop Distance`. Round down.
4. **Check portfolio heat:** Sum all open risks. If total exceeds ~3% of account, skip or reduce.
5. **During the trade:** Track progress in R. Trail stops at +1R, +2R milestones to lock in gains.
6. **End of day:** Log outcome in R. If daily loss limit hit → stop. If 3+ consecutive losses → pause 60 min, re-evaluate.
7. **Weekly/monthly:** Review equity curve. If drawdown tier has changed, adjust sizing per the protocol above.

The entire system reduces to one idea: **risk a small, fixed fraction; measure everything in R; and automatically shrink when equity falls.** This keeps you in the game long enough for positive expectancy to play out.

