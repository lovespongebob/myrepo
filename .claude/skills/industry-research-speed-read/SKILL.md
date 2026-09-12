---
name: industry-research-speed-read
description: Six-step industry analysis framework (define the boundary → identify the life-cycle stage → find the stage's core question → verify unit economics and valuation fit → screen external variables → track leading indicators) that produces a practical six-conclusion brief - industry boundary, life cycle, core logic, competitive landscape, risks, and valuation/economics. Works in two modes - with 3–5 uploaded research reports, OR cold start from a plain-English request with no documents or data at all. Use this skill whenever the user uploads industry or equity research reports for analysis, OR simply asks to understand, evaluate, size, or enter an industry, sector, or market in everyday language — "help me understand the coffee shop business", "is X industry worth investing in", "should I start a business in Y", "what stage is Z market in", questions about penetration rate, TAM, competitive landscape, moats, industry momentum, or valuation. No reports or data are required to trigger it.
---

# Industry Research Speed Read

Core logic: **define the boundary → identify the life-cycle stage → find the stage's core question → verify unit economics and valuation fit → screen external variables → track leading indicators**.

Purpose: turn whatever the user has — 5 research reports or one plain-English sentence — into a set of testable, trackable judgments they can act on. The reports (or your own knowledge) supply raw material; the conclusions must be reasoned, labeled by confidence, and angled at the user's actual decision.

Supporting resources:
- `references/checklist.md` — printable execution checklist for report-based runs
- `references/report-mapping.md` — maps each step to the report sections where material usually lives (report mode)
- `references/cold-start-playbook.md` — proxy estimation methods and free evidence sources when the user has nothing (cold-start mode)

## Trigger

Use this skill when:
- The user uploads or references industry research reports and asks for analysis, a summary, or takeaways
- The user asks in plain language to understand or evaluate an industry, sector, or market — "is this a good business", "should I invest in / enter / sell to this industry", "how big is this market", "who wins in this space" — **even with no documents or data at all**
- The user asks about life-cycle stage, penetration, TAM, competitive landscape, moats, momentum, or which valuation method fits

Out of scope: deep single-company financial modeling, macro strategy, pure trading questions.

## Choose the mode (don't ask the user to)

- **Report mode** — the user provided reports or data files → follow the workflow below using `references/report-mapping.md` to locate material; cite sources.
- **Cold-start mode** — the user provided only a request → same six steps, but evidence comes from web search (if available) and your own knowledge, with `references/cold-start-playbook.md` for estimating missing numbers. Never refuse or stall for lack of documents; the whole point is to deliver a useful first read from nothing.
- Mixed (one report, a few data points) → run cold-start and fold in whatever they gave you as the highest-priority evidence.

## Before analyzing: lock onto the user's decision

The same industry brief looks different for different decisions. From the request, identify:
1. **Industry and segment** (their words, then mapped to a proper boundary in Step 1)
2. **Geography** (a market's stage differs by country — if unstated, use the user's likely home market or the global market, and say which you assumed)
3. **The decision behind the question**: invest in stocks | start or enter the business | sell to the industry | career move | general learning. If unstated, infer it; state the inferred goal in one line at the top of the output so a wrong guess is instantly visible.

## Optional intake — invite steering, never require it

When the session is interactive and the request is open-ended (e.g., "help me understand X"), offer one compact intake round before analyzing — a chance for the user to steer, presented so that skipping it is effortless. Cover at most three things in one message (use a structured question tool like AskUserQuestion when available, plain text otherwise):

1. **Goal** — what's behind the question: investing | starting or entering the business | selling to the industry | career move | just learning
2. **Materials** — anything they'd like analyzed: reports, data files, links, even rough notes ("or nothing — I can start from scratch")
3. **Focus** — specific topics to go deeper on: e.g., a particular segment, competitor, geography, technology, or risk

Always close the intake with an explicit escape hatch — "or just say **go ahead** and I'll proceed with sensible assumptions" — and treat a partial answer as complete: fill unanswered slots by inference, exactly as if the intake hadn't happened. One round only; never follow up an intake with more questions.

Skip the intake entirely when: the request already specifies the goal or focus ("should I invest in X", "compare A and B segments"), the user asked for an immediate answer, the run is non-interactive/automated, or the user declined an intake earlier in the conversation. In those cases fall back to the default: infer everything, state assumptions, and ask at most one clarifying question — only when the answer would materially change the conclusions (e.g., geography completely ambiguous). A good analysis with visible assumptions beats an interrogation.

**Honoring focus topics**: user-named topics get a dedicated **Focus** section in the output (after the six conclusions), each addressed with the same evidence-and-tags discipline. The six conclusions still always appear — the focus deepens the brief without replacing its structure.

## Agent workflow (both modes)

### Step 1: Define the industry boundary
Pick one classification standard (e.g., GICS, ICB, NAICS, or the local regulatory classification) and use it consistently; reconcile conflicting report taxonomies before comparing numbers. Map the value chain (upstream — midstream — downstream), confirm the exact segment, and name the key players. In cold-start mode, a simple three-box value-chain sketch in text is enough.

### Step 2: Identify the life-cycle stage
Penetration rate = current users ÷ addressable customer base. No direct figure → estimate with a proxy (core product sales ÷ total potential demand; see the cold-start playbook). Thresholds: **<15% introduction | 15–40% growth | 40–70% maturity | >70% decline**. Cross-check with revenue growth (growth >20%, maturity <10%) and concentration so one shaky number doesn't decide the stage.

### Step 3: Ask the stage's core question

| Stage | Core task | Key checks |
|-------|-----------|------------|
| Introduction | Validate the business model | Demand authenticity (benchmark vs. earlier periods or other markets); profit feasibility (high frequency or low price elasticity — at least one; standardizable costs) |
| Growth | Size the market + test expansion | TAM = target customers × penetration × average spend × frequency; is channel/capacity expansion matching demand or overshooting |
| Maturity | Analyze moats + profit split | Resource control / network effects; CR3/CR8 concentration; margin distribution along the value chain |
| Decline | Screen substitution risk | Substitute progress; do leaders have a second growth curve |

### Step 4: Verify unit economics and valuation fit
Profit per unit = revenue − direct costs − allocated indirect costs, on the smallest repeatable unit (a store, a unit, an order, a subscriber). Match valuation to stage: introduction → potential | growth → PEG | maturity → PE/PB | decline → beware the low-multiple trap. **If the user's goal isn't stock investing, translate this step**: for a founder/entrant, "entry economics" (startup cost, time to unit break-even, what scale requires); for a supplier, which link of the chain holds budget and margin; for a career move, whether the stage supports hiring and wage growth.

### Step 5: Screen external variables (PEST)
Political (industry/trade policy) | Economic (cycle, rates, FX) | Social (demographics, consumption habits) | Technological (maturity, substitution). Converge to exactly **3 core drivers/risks** — more means the main forces haven't been found yet.

### Step 6: Set up tracking
Pick 1–2 high-frequency indicators by value-chain position: upstream → prices + inventories | midstream → production/shipment volumes | consumer-facing → retail sales or price indices | services → operating metrics. Tell the user **where to check each one for free** (statistical agencies, trade associations, listed competitors' filings — see playbook). Rule: indicators contradicting the thesis for 3 consecutive months → revise the thesis, don't explain it away.

## Output

Plain English, minimal jargon — define any term you must use (TAM, PEG) in a short clause on first mention. Every conclusion carries a confidence tag: **[Sourced]** (from a provided report or verifiable data), **[Estimated]** (proxy or reasoned calculation — show the arithmetic), **[Low confidence]** (would change with better data). Structure:

```
Goal I'm answering: <one line — the inferred decision and assumed geography>

## Bottom line
2–4 sentences that directly answer the user's actual question. Verdict first, then the one reason that matters most.

## The six conclusions
1. Industry boundary — core products, key value-chain links [tag]
2. Life cycle — penetration → stage → the core question that stage raises [tag]
3. Core logic — demand authenticity / unit-level profitability / top growth drivers [tag]
4. Competitive landscape — leaders' share, type of moat [tag]
5. Risk flags — the 3 core external risks [tag]
6. Valuation / economics — fitting method and rough read, translated to the user's goal [tag]

## Focus: <topic>          (only when the user named focus topics in the intake or request)
One short section per named topic, same evidence-and-tags discipline as the conclusions.

## What to watch
1–2 indicators · where to find each free · current direction · "if these contradict this view for 3 straight months, revise it"

## How to make this analysis stronger   (cold-start or thin-evidence runs only)
The 2–3 specific documents or data points that would upgrade confidence most, and where to get them.
```

Keep the whole brief readable in under 3 minutes. Depth goes into the reasoning, never into length.

## Common pitfalls

- **Mixed classification standards** → conflicting numbers; reconcile to one standard before quoting anything
- **Missing penetration data** → estimate "core product sales ÷ total potential demand", state the assumptions, tag [Estimated]
- **Stage mismatch** → PE on a growth industry, or reading a declining industry's low multiple as cheap; the method follows the stage
- **Cold-start overconfidence** → internal knowledge has a cutoff date; say so for fast-moving figures and tag them honestly rather than presenting recalled numbers as current
