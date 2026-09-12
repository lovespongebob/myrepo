# Cold-Start Playbook

How to run the six steps when the user provides no reports and no data — just a request. The goal is a genuinely useful first read, honestly labeled, that the user can upgrade later.

## Ground rules

1. **Never stall for lack of documents.** Deliver the best evidence-backed read you can, tag confidence honestly, and end with the upgrade path.
2. **Search first when you can.** If web search is available, spend it on the few numbers that decide the stage call: market size, growth rate, penetration or a proxy, and the top players' share. Everything else can come from reasoning.
3. **Date your knowledge.** For fast-moving figures recalled from internal knowledge, state the approximate vintage ("as of ~2024") and tag [Low confidence] rather than presenting them as current.
4. **Show the arithmetic** for every [Estimated] number, in one line the user can check and challenge.

## Estimating penetration with nothing (Fermi proxies)

Penetration = current users ÷ addressable base. Build both halves from observable pieces:

- **Addressable base**: start from population or number of households/businesses in the geography, cut by who could plausibly use the product (age band, income tier, business size). Two or three cuts maximum — more cuts means false precision.
- **Current users**: work from any observable anchor — units sold per year × replacement life, subscriber counts from the largest players scaled up by their rough market share, or store counts × plausible customers per store.
- **Sanity check** the result against an analogous market that is further along (a country, a demographic, or an adjacent product that adopted earlier). If your estimate implies this market is ahead of the analog without a reason, the estimate is wrong.

When even a proxy is too shaky, classify the stage qualitatively instead: introduction feels like "explaining the product is still necessary"; growth like "new entrants and funding everywhere"; maturity like "competition is about share and price"; decline like "customers are migrating to a substitute". Say you staged it qualitatively.

## Free evidence sources (generic categories, any country)

| What you need | Where to look for free |
|---------------|------------------------|
| Market size, volumes, prices | National statistics office; industry/trade association annual releases; customs/trade data for goods |
| Company-level share, margins, unit economics | Listed competitors' annual reports and investor presentations — the single richest free source; earnings call transcripts |
| Demand direction | Search-interest trends; app store rankings; marketplace best-seller lists; foot-traffic or booking platforms |
| Supply/expansion signals | Job postings volume at key players; announced capacity/store openings; commercial real-estate listings |
| Policy | The regulator's own site; legislative trackers; trade-association policy pages |
| Ongoing tracking (Step 6) | Monthly releases from the above — pick sources that publish on a schedule so the user can actually follow them |

Point the user to source *categories* and name the specific outlet only when you are confident it exists in their geography.

## Confidence tagging discipline

- **[Sourced]** — traceable to a document the user gave you or a source you actually found in search. Cite it.
- **[Estimated]** — your own calculation from sourced or observable inputs. Show the one-line arithmetic.
- **[Low confidence]** — recalled figures, qualitative staging, or anything a single new data point could overturn.

A brief that is 80% [Estimated] is fine — the tags are what keep it trustworthy. A brief that hides its estimates is worse than no brief.

Four evidence rules that keep [Sourced] honest:

1. **A claim is a fact about the claim.** A company stating it saves customers 30% verifies only that the statement was published; the outcome itself is a separate, unverified proposition. Attribute it — "the company reports…" — and never let the attribution slide into fact on a later mention.
2. **Deduplicate to root sources.** Ten articles citing the same underlying report are one source, never ten; cite the root and note the coverage.
3. **Carry both dates.** A source's publication date and the period its data covers are different things — "a 2026 article about 2023 shipments" is 2023 evidence. Never let the date you accessed something stand in for either.
4. **Never average a conflict.** When figures disagree, first align definition, time period, geography and unit — most conflicts dissolve there. What still conflicts stays side by side with a stated reason for the figure you adopt; splitting the difference manufactures a number nobody published.

## The upgrade path (always include for cold starts)

End with the 2–3 acquisitions that would raise confidence most, ranked by impact — typically:
1. One deep-dive report on the industry (names the boundary, chain, and players properly)
2. The penetration or sales series that decides the stage call
3. The largest listed competitor's latest annual report (unit economics and margins)

Frame each as "getting X would firm up conclusion(s) N", so the user knows exactly why it's worth the effort.
