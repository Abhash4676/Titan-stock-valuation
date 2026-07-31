# Titan Company Limited — Stock Valuation Model

DCF + Relative Valuation built in Excel for **Titan Company Limited (NSE: TITAN)**, India's leading organised jewellery, watches, and eyewear retailer (Tanishq, Titan Watches, Titan Eye+).

**[Download the workbook]("C:\Users\abhas\Downloads\Titan stock valuation model final.xlsx")**

![Dashboard](./screenshots/dashboard.png)

## What this model does

- 5-year driver-based forecast (FY26E–FY30E) built from revenue growth, EBIT margin, D&A, capex, and working-capital assumptions
- Free Cash Flow to Firm (FCFF) discounted at a CAPM-derived WACC
- Gordon Growth terminal value
- Two-way sensitivity grid: WACC × terminal growth, fully formula-driven (no macros)
- Relative valuation against 4 organised-jewellery peers (P/E and EV/EBITDA)
- One-page Dashboard: KPI cards, valuation football field, and a revenue trend chart

## Method

- **Historicals:** FY21–FY25 consolidated revenue, EBIT margin, and net income sourced from public filings and market-data sites (Screener.in, Business Standard capital-market reports); items not individually disclosed in summary results (D&A, capex, NWC, debt/cash) are documented estimates — flagged clearly in the workbook's source notes
- **Forecast:** revenue growth tapers 15.0% → 11.0%; EBIT margin normalises toward Titan's historical 11%–11.5% band; tax rate 25%
- **WACC:** Rf 6.9% (10Y G-Sec), Beta 0.90, ERP 6.5% → Ke 12.75%; blended WACC ≈ 12.7%
- **Terminal growth:** 5.0%, at/below long-run nominal India GDP growth

## Key output

| Metric | Value |
|---|---|
| Intrinsic Value / Share (DCF) | ~₹785 |
| Comps-implied Value / Share | ~₹1,070–₹1,155 |
| Current Market Price (Jul-2026) | ₹4,698 |
| WACC | 12.7% |

## A finding worth reading before the numbers

Titan trades at roughly a **90x trailing P/E** — far above both the DCF intrinsic value and the peer-comps range above. That gap isn't a modelling error: the market is pricing in a multi-decade compounding growth story (India's organised-jewellery penetration is still low, and Titan is the category leader) that a 5-year explicit DCF horizon and a 5% terminal growth rate can't capture. The workbook's Dashboard sheet walks through why, and what to stress-test (longer explicit high-growth period, higher terminal growth, or a terminal exit multiple) before concluding the stock is mispriced — the same judgement call an equity research desk makes on any high-multiple growth compounder.

## Workbook structure

```
Titan_Stock_Valuation_Model.xlsx
├── Dashboard              KPI cards, football field, revenue trend chart
├── Inputs                 All assumptions (blue = editable)
├── Historical Financials  FY21–FY25 actuals + sources
├── Forecast                FY26E–FY30E driver-based projection
├── DCF Valuation           WACC build, FCFF discounting, terminal value, EV → per-share bridge
├── Comparable Companies    Peer P/E & EV/EBITDA
└── Sensitivity Analysis    WACC × terminal-growth grid
```

Colour convention: **blue** = hardcoded input, **black** = formula, **green** = link to another sheet.

## Tools

Excel · DCF · CAPM · Comparable Company Analysis

---
*Educational / portfolio project. Not investment advice. Figures compiled from public sources in Jul-2026 — refresh from Screener.in / stockanalysis.com before relying on this for a live decision.*
