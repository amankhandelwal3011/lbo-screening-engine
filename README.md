# LBO Screening Engine — India Take-Private Candidates

An interactive dashboard that screens 25 listed Indian companies for private-equity take-private feasibility, then models a full 5-year LBO for the shortlisted names.

**Live demo:** https://amankhandelwal3011.github.io/lbo-screening-engine/

## What it does

1. **Stage 0 — Deal feasibility:** excludes government-owned companies, financial companies, and companies above an editable enterprise-value cap.
2. **Stage 1 — Screening:** filters survivors on EBITDA margin, FCF conversion, ROCE, EV/EBITDA, and net debt/EBITDA.
3. **LBO engine:** for any shortlisted company — sources & uses, a 5-year debt schedule with a cash sweep (senior debt repaid first), exit value, IRR and MOIC, and a returns-attribution breakdown.
4. **Scenarios:** base / downside / upside cases, plus IRR sensitivity heatmaps across leverage, exit multiple, growth and margin.
5. **Ranking:** a composite score (base IRR, downside IRR, FCF conversion, ROCE, entry valuation) with a Strong Buy / Watch / Pass classification.
6. **IC memo:** an auto-generated one-page investment committee memo for the top-ranked deal.

Every assumption and threshold is editable and recalculates the full model live.

## Verification

The Castrol India result (12.0% IRR, 1.8x MOIC at default assumptions) was independently rebuilt by hand in Excel — sources & uses, the debt schedule, exit value and IRR all tie out to the dashboard.

## Data

25 NSE/BSE-listed companies, financials sourced from Screener.in. Values in ₹ crore.

## Tools used

Financial model logic, screening framework, and assumptions designed independently. Built as a single self-contained HTML/JavaScript file.
