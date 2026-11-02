# Source checklist and availability policy

Use this file as the fixed source checklist for Iran-Israel-US escalation reports.

## A. Directly useful public sources

### Airspace and NOTAM
- SafeAirspace Israel: `https://safeairspace.net/israel/` — use risk level, FIR status, NOTAM summary, validity dates.
- SafeAirspace Iran: `https://safeairspace.net/iran/` — use risk level, FIR OIIX warnings, foreign and domestic NOTAM summaries when shown.
- SafeAirspace UAE: `https://safeairspace.net/united-arab-emirates/` — use caution level and GNSS spoofing/jamming notes.
- SafeAirspace Qatar: `https://safeairspace.net/qatar/` — use caution level and regional risk notes.
- NOTAM Info: `https://notaminfo.com/` — use for raw/near-raw NOTAM lookups when accessible.
- OPSGROUP blog: `https://ops.group/blog/` — use for public aviation-risk summaries and airspace context.

### Maritime and shipping
- MSCIO alerts: `https://www.mscio.eu/alerts/` — use recent alerts/incidents.
- UKMTO: `https://www.ukmto.org/` — use advisories, warnings, incident reports.
- MARAD: `https://www.marad.dot.gov/` or maritime.dot.gov redirects — use U.S. maritime advisories.
- GAC Hot Port News: `https://www.gac.com/hot-port-news` — use port/shipping operational updates.
- VesselFinder: `https://www.vesselfinder.com/` — use public AIS summaries only; do not over-interpret gaps.
- ShipXplorer: `https://www.shipxplorer.com/` — use public vessel/traffic visibility only.
- TankerTrackers: `https://www.tankertrackers.com/` — public pages/social summaries only unless accessible; paid detail is unavailable.

### GNSS, AIS, cyber and internet
- GPSJam: `https://gpsjam.org/` — use map/day if current data is available; state if day is incomplete.
- Flightradar24 GPS jamming map/blog: `https://www.flightradar24.com/blog/gps-jamming-map/` — use as explanatory/public GNSS source.
- Cloudflare Radar: `https://radar.cloudflare.com/` — use internet outage/traffic anomalies.
- BGP.he.net: `https://bgp.he.net/` — use BGP routing context when specific networks are relevant.

### Energy and volatility
- Investing Brent: `https://www.investing.com/commodities/brent-oil` — Brent price and change.
- OilPrice: `https://oilprice.com/` — oil price and energy news.
- CME Energy: `https://www.cmegroup.com/markets/energy.html` — futures context.
- CBOE OVX: `https://www.cboe.com/us/indices/dashboard/ovx/` — OVX reference; if value is not extractable, say so.
- Barchart crude volatility/greeks: `https://www.barchart.com/futures/quotes/CL*0/volatility-greeks` — oil vol proxy if accessible.

### Markets and rates
- TradingEconomics: `https://tradingeconomics.com/` — market, FX, commodities, bond values.
- FRED: `https://fred.stlouisfed.org/` — rates/spreads, often delayed but authoritative.
- TradingView: `https://www.tradingview.com/` — cross-market values when readable.
- Finviz: `https://finviz.com/` — equities/sector heatmap and tickers.
- TASE: `https://www.tase.co.il/en` — Israeli market context if readable.

### Prediction markets
- Polymarket Iran: `https://polymarket.com/predictions/iran` — relevant Iran market probabilities, volumes, liquidity.
- Polymarket general: `https://polymarket.com/` — broader prediction-market search.
- Manifold: `https://manifold.markets/` — supplementary public prediction markets.

### Event aggregators, GEOINT and OSINT
- Liveuamap: `https://liveuamap.com/`, `https://syria.liveuamap.com/`, `https://israelpalestine.liveuamap.com/` — event map context.
- ACLED: `https://acleddata.com/` — structured event data, usually not minute-by-minute.
- NASA FIRMS: `https://firms.modaps.eosdis.nasa.gov/` — fire/thermal anomaly context.
- Zoom Earth: `https://zoom.earth/` — public satellite/weather/fire context.

## B. Sources that are often limited or unreliable in this environment

Use these only if they open cleanly; otherwise state the limitation and use alternatives:

- Yahoo Finance MOVE: often `429 Too Many Requests`.
- MarketWatch OVX/MOVE and MarketWatch general: often restricted.
- FAA NOTAMs: often `403 Forbidden`.
- MarineTraffic: often JavaScript/paywall/limited.
- ADSB.fi: may fail to return useful public data.
- NAVTEX.lv: may not return useful output.
- SKAI GPSJAM: may fail/cache miss.
- WSJ bonds: often restricted.
- Kalshi: often readable page shell but limited data.
- Investing TA-35 URL variants may 404; search for an alternate symbol/page.
- Sentinel Hub apps: JavaScript/login dependent.
- Oracle Internet Intelligence: may redirect to a generic Oracle page.
- Downdetector: may be inaccessible.
- CriticalThreats: may be inaccessible.

## C. Access status language

Use concise labels:

- `قابل استفاده مستقیم`: current value or status was readable.
- `قابل استفاده با محدودیت`: page opens but data is partial, delayed, JavaScript-only, or requires interpretation.
- `غیرقابل اتکا در این run`: blocked, rate-limited, paywalled, login-required, or no useful output.

Never hide unavailable data. Missing high-value sources should appear in uncertainty and limitations.
