# 🌕 MoonTide
MoonTide is a disciplined, risk-controlled investment project.

**Phase 1: BondCycle Strategy — Pure Bond Investment Framework**


**BondCycle** (Phase 1) rotates capital between **short-term Treasuries (e.g., SGOV)** and **long-term U.S. Treasuries** using rule-based entry/exit logic driven by yield spreads, historical price percentiles, and the MOVE index.

---

## 📌 Core Principles
- **Capital preservation first**, return optimization second
- Trade **infrequently**, only on high-confidence signals
- Use **SGOV** to earn yield while waiting
- No equities in Phase 1 (SPX fallback is Phase 2)

---

## 🔁 BondCycle (Phase 1)
**Entry (buy long bonds) when:**
- Yield spread (Long-bond − SGOV) ≥ **1.0–1.5%**
- Price in **lowest ~20–30%** of 3–5y range (or model-justified)
- **MOVE < 75** preferred; **75–100** caution; **> 100** avoid unless exceptional
- Macro check optional (e.g., no imminent hawkish shock)

**Exit (sell long bonds) when:**
- Price in **top ~20%** of range
- Yield spread narrows to **< 0.5%**
- **MOVE > 100** while price is rich → sell into strength
- Macro: easing largely priced / limited upside

**Pure cycle:** `Cash → SGOV → Long Bond → SGOV → (repeat)`

---

## 📊 Data Acquisition Plan
All series saved as CSV (daily unless noted).  
Use FRED for macro/rates; later add SGOV/MOVE from market sources.

**FRED core:**
- `DGS20` — 20-Year Treasury Yield (%)
- `DGS3MO` — 3-Month T-Bill Yield (%)
- `DFEDTARU` — Fed Funds Target Upper Bound (%)
- `FEDFUNDS` — Effective Fed Funds Rate (%)
- `CPIAUCSL` — CPI (monthly, index 1982–84=100)
- `UNRATE` — Unemployment Rate (% monthly)
- `GDP` — Nominal GDP (Quarterly)

**Non-FRED (add later):**
- **SGOV** — ETF price (Yahoo Finance / `yfinance`)
- **MOVE** — Bond volatility index (Yahoo Finance `^MOVE` or licensed source)
- (Optional) **VIX** (for Phase 2 work)

---

## Other strategies in developing
1. probabilistic mode based Bond trading strategy
2. vix-based tech stock put-spread selling or spx/ndx put-spread selling
3. When hugh market crash happens, the fallback of the SPX fallback strategy is to buy long term (2-3 years) call options.

## 🧱 Repo Structure (suggested)
```
MoonTide/
├─ data/ # CSV outputs (gitignored)
├─ src/
│ ├─ init.py
│ ├─ fetch_fred_data.py # FRED acquisition (provided)
│ └─ (later) fetch_market.py# SGOV/MOVE/VIX via yfinance
├─ notebooks/ # Exploration / backtests
├─ environment.yml # Conda env lockfile
├─ .gitignore
└─ README.md
```

## Code environment
- activate env
  ```
  conda activate mtenv
  ```

- setup env
  ```
  conda env create -f environment.yml
  ```

## General goal

- guidance: realizing profit as much as possible while minimizing risk.
- create about 5%-10% annual profit by tading bond (buy-low sell-high), this strategy generally has zero risk.
- create another 5%-10% annual profit by trading equity/index (put-spread selling), this strategy should have minimum risks. the put spread already limited the risk, however, we should has some general assumption to quantify this risk. for example, if we generally assume there will be two market crashing events yearly (spx fall 10% or more), then we will lose money on this put-spread selling strategy. But we consider the crash as an opportunity because of our fallback to spx logic. If we want to have a monthly gain 0.8% ~ 1%, then selling spx put-spread should be very doable. We want to sell the safest put-spread while maintaining a monthly gain of 0.8%-1%.

- fall back to spx holding at market crash, this might bring another 5%-10% anual profit
- togther we will realize anual 15% - 25% profit, which will doble our found in 3 years
