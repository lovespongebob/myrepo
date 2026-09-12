---
name: industry-research-speed-read
description: Six-step industry research framework (define the boundary → identify the life-cycle stage → find the stage's core question → verify unit economics and valuation fit → screen external variables → track leading indicators). Rapidly distills 3–5 industry research reports into six conclusions - industry boundary, life cycle, core logic, competitive landscape, risks, and valuation approach. Use this skill whenever the user uploads or references industry or equity research reports, asks to analyze an industry, sector, or market, judge its life-cycle stage or penetration rate, size the market (TAM), assess competitive landscape, concentration, or moats, gauge industry momentum, pick a valuation method, or asks "is this industry worth investing in" — even if they never mention the six-step method by name.
---

# Industry Research Speed Read

Core logic: **define the boundary → identify the life-cycle stage → find the stage's core question → verify unit economics and valuation fit → screen external variables → track leading indicators**.

Purpose: compress 3–5 industry research reports into a set of testable, trackable judgments rather than a summary of the reports' opinions. Stay critical throughout: the reports supply raw material; the conclusions must be your own.

Supporting resources:
- `references/checklist.md` — printable execution checklist; tick items off to avoid missing steps
- `references/report-mapping.md` — maps each step to the report sections where the material usually lives

## Trigger

Use this skill when:
- The user uploads or references industry research reports, deep-dive reports, or annual outlook/strategy reports and asks for analysis, a summary, or key takeaways
- The user asks what stage an industry or market is in, its penetration rate, its ceiling or market size, or whether it is worth investing in
- The user asks about competitive landscape, moats, industry momentum, or which valuation method fits a given industry

Out of scope: deep single-company fundamental analysis (company financial modeling), macro strategy, and pure trading questions.

## Input

- **Required**: 3–5 research reports on the target industry (prefer one deep-dive report plus one annual outlook; diverse sources are better than one firm's view)
- **Optional**: high-frequency industry data (monthly sales, prices, penetration, inventory, etc.) — with it, Step 6 tracking is much stronger
- With fewer than 3 reports, proceed anyway but explicitly flag conclusions as "limited evidence, lower confidence"

## Agent Workflow

### Step 1: Define the industry boundary (report section: industry definition and classification)

- Pick one classification standard and use it consistently throughout (e.g., GICS, ICB, NAICS, or the national/regulatory classification used in the target market). When reports use different standards, reconcile the data to one standard before comparing any numbers
- Map the value chain (upstream — midstream — downstream), and confirm exactly which segment you are analyzing; don't blend different segments into one conclusion
- Extract: core products/services and the key upstream and downstream players

### Step 2: Identify the life-cycle stage (report section: penetration data)

- Penetration rate = current users ÷ addressable customer base. When no direct figure exists, estimate with a proxy: core product sales ÷ total potential demand
- Stage thresholds: **<15% introduction | 15–40% growth | 40–70% maturity | >70% decline**
- Cross-check to avoid a single-metric misread: revenue growth (growth stage >20%, maturity <10%) and how concentrated the competitive landscape is

### Step 3: Ask the stage's core question

Each stage has different questions that matter — asking a wrong-stage question produces a wrong conclusion:

| Stage | Core task | Key checks |
|-------|-----------|------------|
| Introduction | Validate the business model | Demand authenticity (benchmark against earlier periods or other markets); profit feasibility (high purchase frequency or low price elasticity — at least one; costs can be standardized) |
| Growth | Size the market + test expansion capacity | TAM = target customers × penetration × average spend × frequency; does channel/capacity expansion match demand, or is it running ahead into overcapacity |
| Maturity | Analyze moats + profit distribution | Resource control / network effects; top-3 and top-8 concentration ratios (CR3/CR8); gross-margin distribution along the value chain (high-margin links hold the power) |
| Decline | Screen substitution risk | Progress of substitute products/technologies; whether leaders have a second growth curve |

### Step 4: Verify unit economics and valuation fit

- **Unit economics (UE) model**: profit per unit = revenue − direct costs − allocated indirect costs. Choose the smallest repeatable economic unit for the business model (a store, a unit sold, an order, a subscriber); cross-check gross margin, net margin, and operating expense ratios
- **Match valuation to stage**: introduction → market potential | growth → PEG | maturity → PE/PB | decline → beware the low-valuation trap

### Step 5: Screen external variables (PEST)

- Political: industry and trade/international policy | Economic: business cycle, interest and exchange rates | Social: demographics, consumption habits | Technological: technology maturity, substitution risk
- Converge the output to **3 core drivers/risk factors** — more than 3 means the main forces haven't been identified yet

### Step 6: Track leading indicators

- Pick 1–2 high-frequency indicators suited to the industry's position in the value chain: upstream/commodity → prices + inventories | midstream/manufacturing → production and shipment volumes | consumer-facing → retail sales or relevant price indices | services → operating metrics (utilization, traffic, bookings)
- Record the current direction (up/down); **if the indicators contradict your thesis for 3 consecutive months → revise the thesis** rather than explaining the divergence away

## Output (six conclusions)

The final deliverable must converge to these six items, each 1–3 sentences, backed by data or explicit logic, with the source report cited:

1. **Industry boundary**: core products, key value-chain links
2. **Life cycle**: penetration rate → stage → that stage's core question
3. **Core logic**: demand authenticity / unit-level profitability / three growth drivers
4. **Competitive landscape**: leaders' market share, type of moat
5. **Risk flags**: 3 core external risks
6. **Valuation approach**: the fitting method (PE/PEG/PB) and why

## Common pitfalls

- **Mixed classification standards**: reports using different taxonomies → conflicting numbers. Reconcile to one standard before quoting any figure
- **Missing penetration data**: estimate it manually as "core product sales ÷ total potential demand" and state the assumptions
- **Stage mismatch**: applying PE to a growth-stage industry, or mistaking a declining industry's low multiple for cheapness — the valuation method must follow the stage
