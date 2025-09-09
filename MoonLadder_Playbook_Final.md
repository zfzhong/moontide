# 🌙 MoonLadder Strategy Playbook (Final Version)

The **MoonLadder Strategy**, part of the **MoonTide Project**, is built around:  

1. **Weekly 4-Week Rolling Ladder** → steady income with risk sleeve ≤ $30k  
2. **Crash Redeploy Plan (LEAPS)** → convex upside in market crashes (SPX −10% or more)  

The strategy is designed to target **~0.5% monthly portfolio gains** while keeping risk capped at ~6% of total capital.

---

## 1. Portfolio Structure
- **Total capital**: $500,000  
- **Risk sleeve**: ≤ $30k (≈6%) in active put spreads  
- **Safe sleeve**: $200k in SGOV (earning ~0.36%/month ≈ $720/month)  
- **Reserve sleeve**: ~$270k in cash/SGOV (used for crash redeploy)  

---

## 2. Weekly 4-Week Rolling Ladder

### Setup
- **Entry**: Every Friday, sell a new SPX put spread expiring in 5 weeks.  
- **Exit**: Close after 4 weeks (≈1 week before expiry).  
- **Ladder**: Always 4 concurrent spreads live.  

### Example (SPX 6500, Sell 6000/5925 Put Spread)
- **Credit**: ≈ $360 gross, ≈ $325 net after early exit  
- **Max loss**: ≈ $7,140  
- **Risk sleeve**: 4 spreads × $7,140 = $28.5k (~5.7% portfolio)  
- **Weekly harvest**: ≈ $325  
- **Monthly income**: ≈ $1,300–1,600  
- **Add SGOV yield**: ≈ $720/month  
- **Total portfolio income**: ≈ $2,020–2,320/month (~0.40–0.46%)  

### Benefits
- Risk sleeve stays under $30k cap.  
- Removes last-week gamma/volatility risk.  
- Predictable weekly cadence and steady income.  

---

## 3. Crash Redeploy Plan (LEAPS)

If SPX falls **≥10% from recent highs**:  

1. Accept spread sleeve loss (max $25–30k).  
2. Redeploy ~$50–70k of reserve into **24–30 month LEAPS call spreads**:  
   - **Index LEAPS**: SPX or SPY ATM/OTM spreads (e.g., 6500/6900).  
   - **Stock Basket LEAPS**: NVDA, MSFT, AAPL, AMZN, META, TSLA. Buy ATM, sell 15–20% OTM. $5–10k per stock.  
3. Keep the remainder ($200k+) in SGOV/cash to deploy further if SPX −20% or deeper.  

### Purpose
- Shallow crash (−10%): LEAPS rebound offsets spread loss.  
- Deep crash (−20%+): LEAPS deliver large asymmetric profits, turning crisis into opportunity.  

---

## 4. Monitoring Checklist
- **Weekly**:  
  - Verify 4 live spreads, risk ≤ $30k.  
  - Confirm each spread closed after 4 weeks.  
- **Monthly**:  
  - Log SGOV interest.  
  - Review implied volatility regime before new trades.  
- **Crash trigger**:  
  - If SPX −10% or more → activate LEAPS redeploy plan.  

---

## ✅ Summary
MoonLadder (Final) = **Weekly 4-Week Put Spread Ladder + LEAPS Crash Redeploy**  

- **Income target**: ~0.5%/month (spreads + SGOV)  
- **Risk cap**: ≤ $30k (≈6% of portfolio)  
- **Crash plan**: redeploy reserve into 24–30 month LEAPS on SPX + stock basket  
- Built for **steady income + resilience in crashes** under the MoonTide Project.
