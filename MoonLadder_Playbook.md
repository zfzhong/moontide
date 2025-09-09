# 🌙 MoonLadder Strategy Playbook

MoonLadder is part of the **MoonTide Project**, designed to generate steady income from SPX option spreads while keeping most capital safe in SGOV and reserves. It balances **short-term premium harvesting** with a **crash redeployment plan**.

---

## 1. Portfolio Structure
- **Total capital**: $500,000  
- **Risk sleeve**: ~$40,000 (≈8%) for SPX put spreads  
- **Safe sleeve**: $200,000 in SGOV (earning ~5%)  
- **Reserve sleeve**: $260,000 in cash/SGOV  

---

## 2. Trade Setup
- **Instrument**: SPX European-style index options (cash-settled).  
- **Spread type**: Bull put spread, 100 points wide.  
- **Target delta**: Short put ≈ 10-delta (≈90% probability OTM).  
- **Entry cadence**: Sell **1 new spread every Monday**, expiring ~28 days out.  
- **Ladder**: After 4 weeks, always 4 spreads live at any time.  
- **Capital at risk**: ≈$9.2k per spread × 4 = ≈$37k max risk.  

---

## 3. Income Target
- **Per spread**: ≈ $800 credit.  
- **4 spreads live**: ≈ $3,200/month (~0.64% portfolio).  
- **SGOV yield**: ≈ $10k/year (~0.2% portfolio/month).  
- **Total target**: **0.8–0.9% per month** portfolio-level return in calm markets.  

---

## 4. Risk Controls
1. **Max allocation**  
   - Never exceed 4 spreads live (~$40k risk).  

2. **Stop-loss rule**  
   - If spread value rises to **3× credit received**, close early.  
   - Example: sold for $8 → exit if value hits $24.  

3. **Event filter**  
   - Avoid opening new spreads right before **CPI, Fed, or NFP**.  
   - Skip weeks where implied volatility is abnormally low (<15%).  

4. **Crash plan**  
   - If spreads hit max loss in a crash, accept it and **close all positions**.  
   - Stop strategy temporarily.  
   - Redeploy **$200k SGOV** into SPX at crash lows to capture long-term rebound.  

---

## 5. Monitoring Checklist
- **Weekly**  
  - Confirm 4 spreads live.  
  - Check each spread vs 3× credit stop.  
  - Ensure exposure ≤ $40k.  

- **Monthly**  
  - Log SGOV yield received.  
  - Review SPX volatility regime (adjust delta if vol shifts significantly).  

---

## 6. Mindset
- Expect **small, steady wins** most months.  
- Accept that **occasional 8% drawdowns** may happen.  
- Trust the **MoonLadder barbell**: SGOV + crash redeploy flips market shocks into opportunity.  

---

## ✅ Summary
MoonLadder = **4-spread ladder + SGOV safety net + crash redeploy option**.  
- Income target: ~0.8%/month.  
- Max risk capped at ~8% of portfolio.  
- Built for resilience and long-term compounding under the MoonTide Project.

## Logic connectoing to fallback to SPX
- We want to sell SPY at the striker which is about 10% down from the current price.
