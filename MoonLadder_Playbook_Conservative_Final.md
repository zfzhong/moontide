# 🌙 MoonLadder Strategy Playbook (Conservative Final Version)

This conservative version of **MoonLadder**, part of the **MoonTide Project**, is designed to achieve about **0.5% monthly portfolio gains** while maximizing safety.  
It uses **deep out-of-the-money SPX put spreads**, keeps drawdowns capped at ~5%, and integrates a **crash redeployment plan**.

---

## 1. Portfolio Structure
- **Total capital**: $500,000  
- **Risk sleeve**: ≤ $25,000 (≈5% of portfolio) for SPX put spreads  
- **Safe sleeve**: $200,000 in SGOV (earning ~5%)  
- **Reserve sleeve**: ~$275,000 in cash/SGOV  

---

## 2. Trade Setup
- **Instrument**: SPX European-style index options (cash-settled, §1256 tax treatment)  
- **Spread type**: Bull put spread  
- **Width**: 80–100 points, max loss per spread ≈ $6.5k–8.5k  
- **Strike rule**: Short put ≈ 12–18% below current SPX (deep OTM)  
- **Expiry**: 3 months (≈90 days)  
- **Exit rule**: Close each spread 3 weeks before expiry (≈9-week holding)  
- **Entry cadence**: Sell 1 new spread every 3 weeks  
- **Ladder**: Always 3 live spreads (never 4)  
- **Capital at risk**: 3 spreads × ~$7–8k = ~$20–25k total (≈5% of portfolio)  

---

## 3. Income Target
- **Per spread**: $600–900 collected (closing early)  
- **3 spreads live**: ≈ $2,100–2,700/month (~0.4–0.5% of portfolio)  
- **SGOV yield**: ≈ $10k/year (~$830/month, 0.15–0.2%)  
- **Total target**: ~0.5–0.7% portfolio return per month in calm markets  

---

## 4. Risk Controls
1. **Max allocation**: Never exceed $25k risk (~5% of portfolio)  
2. **Stop-loss rule**: Close if spread value rises to 3× credit received  
   - Example: sold for $10 → exit if value hits $30  
3. **Event filter**: Avoid entering before CPI, Fed, or NFP; skip weeks if implied volatility <15%  
4. **Crash plan**: If spreads hit max loss, accept it, close all, pause strategy, and redeploy $200k SGOV into SPX at lows  

---

## 5. Monitoring Checklist
- **Weekly**: confirm 3 spreads live, risk per spread ≤ $8k, total ≤ $25k, check vs stop rule  
- **Monthly**: log SGOV interest, review SPX volatility, adjust strikes to remain 12–18% OTM  

---

## 6. Mindset
- Target steady ~0.5% monthly returns, not maximum income  
- Accept occasional 5% drawdowns  
- Trust the **MoonLadder barbell**: SGOV + crash redeploy flips shocks into opportunity  

---

## ✅ Summary
MoonLadder (Conservative Final) = **3 deep OTM 3‑month put spreads (closed after 9 weeks)** + **SGOV safety net** + **crash redeploy option**  

- **Income target**: ~0.5%/month  
- **Max risk capped**: ≤ $25k (5% of portfolio)  
- Built for **resilience, safety, and long-term compounding** under the MoonTide Project
