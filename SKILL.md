---
name: iran-war-escalation
description: produce precise Persian escalation-risk reports for Iran, Israel, and United States conflict or ceasefire scenarios using public OSINT, airspace/NOTAM, maritime, GNSS/AIS, energy, cross-asset market, prediction-market, diplomacy, and military-logistics indicators. Use this skill for one-off or recurring status reports where the user expects current numbers, explicit source limitations, weighted mosaic analysis, and the fixed Persian report structure.
---

# Iran War Escalation

Use this skill when the user asks for a current escalation-risk assessment involving Iran, Israel, the United States, Hormuz, ceasefire status, airspace/NOTAM, shipping, oil, markets, Polymarket, or OSINT. Default to Persian.

## Non-negotiable reporting rules

- Treat every output as a risk assessment, not a prediction.
- Use multiple independent evidence categories before raising or lowering the score materially.
- Current numeric indicators must be numeric whenever public data is accessible. Do not write vague labels such as "بالا" in the value field if an actual number is available.
- If a numeric source is inaccessible, write exactly why: rate-limited, restricted, JavaScript-only, paywalled, login-required, stale, or not found.
- Distinguish confirmed facts, credible reports, unverified claims, and market-implied signals.
- Never infer operational intent from one market move or one social-media claim.
- Cite sources for current facts and market values.
- Keep analysis strategic. Do not provide tactical targeting, evasion, or operational advice.

## Required workflow

1. Establish timestamp and assessed window.
2. Check source availability using `references/source-checklist.md`.
3. Gather current signals across `references/indicator-taxonomy.md`.
4. Pull numeric market values using `references/market-watchlist.md`; prioritize tool finance data where available and public web sources otherwise.
5. Score using `references/scoring-rubric.md`, then sanity-check against corroboration/de-escalation signals.
6. Produce the report using `references/report-template.md`.
7. Include missing-data caveats every time restricted feeds are unavailable.

## Direct-source priority list

For this skill, always try these direct public sources before generic web search:

- Airspace/NOTAM: SafeAirspace Iran, Israel, UAE, Qatar; NOTAM Info; OPSGROUP blog; FAA NOTAM only if accessible.
- Maritime: MSCIO alerts, UKMTO, MARAD, GAC Hot Port News, VesselFinder, ShipXplorer, TankerTrackers public pages.
- GNSS/AIS/cyber: GPSJam, Flightradar24 GPS jamming map/blog, Cloudflare Radar, BGP.he.net.
- Energy/volatility: Investing Brent, OilPrice, CME Energy, CBOE OVX, Barchart crude volatility/greeks.
- Rates/markets: TradingEconomics, FRED, TradingView, Finviz, Yahoo/MarketWatch only when not rate-limited/restricted.
- Prediction markets: Polymarket Iran page, Polymarket general, Manifold. Kalshi only if readable.
- Regional/OSINT: Liveuamap, Syria Liveuamap, Israel-Palestine Liveuamap, ACLED, NASA FIRMS, Zoom Earth.

## Numeric-value discipline

In the table, the `مقدار فعلی` column should contain:

- Brent, WTI, gold, DXY, VIX, MOVE, OVX, Treasury yields, FX pairs, BTC/ETH: exact last/close value plus timestamp or session if available.
- Polymarket Iran: relevant market probability, volume/liquidity, and 24h change if visible.
- SafeAirspace/NOTAM: exact risk level, FIR/area, NOTAM number, validity window, and issuing authority if available.
- MSCIO/UKMTO/MARAD: incident count/alert level/date/time/location when visible.
- If unavailable: `داده قابل اتکا در دسترس نیست — [reason]`.

## Weighting guidance

Give highest practical weight to official or physical indicators: airspace closure, NOTAM, embassy/citizen evacuation, military logistics, maritime incidents, and verified energy/shipping disruption. Market indicators are confirmatory unless moves are large and cross-asset. Polymarket and crypto are supplementary.

## Output constraints

- Use the exact Persian report sections in `references/report-template.md`.
- Keep routine reports concise, but never omit critical numeric values or source limitations.
- End every report with exactly three horizontal separator lines.
