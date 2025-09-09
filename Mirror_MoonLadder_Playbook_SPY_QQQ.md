# 🌙 Mirror MoonLadder Playbook (SPY + QQQ Version)

## Core Principle
Mirror MoonLadder is the "twin" of MoonLadder.  
- Always **long the benchmark index (SPY/QQQ)**.  
- **Protective puts** cap downside risk.  
- **Covered calls** on rallies harvest income.  
- If protective puts are breached → **redeploy into LEAPS** (24–30 month call spreads).  

---

## Sleeve 1: SPY (Defined-Risk Long)
- **Unit Example:**  
  - Buy 100 SPY @ 650 = $65,000  
  - Buy 600 put (long-dated) ≈ $5,000 cost  
  - Max loss per unit ≈ $5,000  
- **Dynamic Rule:**  
  - If SPY climbs above 675 → Sell 700 call (income sleeve)  
  - If SPY falls back → Buy back 700 call (remove cap)  
- **Allocation:** Up to **6 units = $30k risk sleeve**  

---

## Sleeve 2: QQQ (Defined-Risk Long)
- **Unit Example (Live Trade):**  
  - Buy 100 QQQ @ 579.4 = $57,940  
  - Buy 530 put (Sep 18, 2026) @ 24.3 = $2,430  
  - Max loss per unit = 4,940 + 2,430 = **$7,370**  
- **Dynamic Rule:**  
  - If QQQ climbs above ~600 → Sell 650/670 call (income sleeve)  
  - If QQQ dips near 550–530 → Hold; put limits loss  
- **Allocation:** Up to **4 units = ~$30k risk sleeve**  

---

## Crash Trigger (< Put Strike)
- If SPY < 600 or QQQ < 530 →  
  - Protective put is ITM → loss capped at risk budget.  
  - Close sleeve and **redeploy into LEAPS call spreads**:  
    - SPY or QQQ LEAPS ATM/OTM spreads (e.g., 600/700, 580/680).  
    - Stock basket LEAPS: NVDA, MSFT, AAPL, AMZN, META, TSLA (ATM + 15–20% OTM).  
- Goal: turn crashes into **convex upside opportunities**.  

---

## Portfolio Integration ($500k Fund)
- **MoonLadder (SPX put spreads)**: $30k sleeve  
- **Mirror MoonLadder (SPY + QQQ protected longs)**: $60k risk sleeve total  
  - SPY sleeve = $30k (~6 units)  
  - QQQ sleeve = $30k (~4 units)  
- **SGOV + cash reserves**: $200k–250k (yield ≈ 0.36%/month)  
- **Flex capital**: $160k–200k reserved for LEAPS redeploy in crashes  

---

## Benefits
- SPY + QQQ sleeves both have **capped downside risk**.  
- Harvest income via calls in **rallies and sideways markets**.  
- Protective puts ensure losses are survivable.  
- LEAPS redeploy converts **market crashes into long-term opportunities**.  
- Risk symmetry: MoonLadder = short convexity income; Mirror MoonLadder = long convexity resilience.  

---

## ✅ Summary
- **SPY Sleeve:** 6 units, $30k max risk  
- **QQQ Sleeve:** 4 units, $30k max risk  
- **Total Mirror MoonLadder:** $60k risk sleeve (12% of portfolio)  
- Core design: **Long equity, protected by puts, monetized by calls, convex in crashes**.  
