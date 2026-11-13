# MU.US Red Team

Run 2026-11-07-semis, as of 2026-11-07, written from commit 2ab7741a44d2 (the dossier, before the bull's claims). Rendered from redteam.json by check_redteam.py.

**Bear verdict: caution.** Strongest objection: R1.

## Summary

Caution, not avoid. FY2026 operating margin of 74.6% came from price (DRAM ASP up about 180% on bits up about 25%) against a previous peak of 49.3% and a FY2023 trough of -37.0%. A 50% fall from $690 needs only about $24.7bn of operating income at the own median 14.1 times EV/EBIT: 25% of FY2026's, or an 18.6% margin on FY2026 revenue. In 2022-23 trailing EBIT fell 81% in three quarters from a 7.1 times multiple like today's 7.4. Against that, the stock is already 43% below its June high at 3.9 times consensus FY2027 EPS, and $134bn of take-or-pay obligations exist. No single objection is decisive at this price; size small and date the position to the 16 Dec 2026 results.

## Pre-mortem: down 50% within 24 months

The stock halves to about $345 by November 2028 because the shortage price that produced a 74.6% operating margin unwinds as supply from Samsung, CXMT and Micron's own new fabs arrives while data-centre spending digests. At that price the market is paying the own median EV/EBIT multiple for operating income of about $24.7bn, an 18.6% margin on FY2026 revenue, which is the industry median margin and still 2.5 times FY2025's operating income.

1. **Dec 2026 to Feb 2027.** The November-quarter results (due 16 Dec 2026) show growth slowing: consensus has revenue of $61.7bn, 13.9% above the August quarter against 31% last quarter. Hyperscaler capex caution after the US midterms and the Taiwan labour dispute keep the stock de-rating from a base of 83% volatility; the multiple stays near 7 times EBIT because earnings are expected to fall. `dossier:figures.117.value` `dossier:figures.21.value` `dossier:figures.102.value` `dossier:expectations.reading`
2. **Mar to Aug 2027.** Contract price growth stalls and then turns negative as Samsung's HBM share (33% in Q2 2026, 40% targeted by Q4) and CXMT (about 10% of DRAM revenue) add supply and Micron's Idaho fab makes its first wafers in mid-2027. The strategic agreements are estimated at over 35% of revenue through 2030, so most sales still follow market prices. Consensus FY2027 EPS of $176.50 is cut and the quarterly operating margin falls from 80.7% into the 60s. `dossier:figures.171.value` `dossier:figures.175.value` `dossier:figures.179.value` `dossier:figures.113.value` `dossier:figures.22.value` `dossier:expectations.what_would_change_it`
3. **Sep 2027 to Mar 2028.** FY2028 starts with capex of about $25bn in the first half of FY2027 already spent into a flattening market. Customers press for price-protection and pricing adjustments (already $4.3bn of consideration payable to customers), receivables of $36.2bn are slow to collect, and a Taiwan wage settlement (a union demand of 15% of operating profit) lifts cost per bit. Operating margin heads to the 2018 peak of 49% and below, and consensus FY2028 revenue of $319.7bn is cut. `dossier:figures.63.value` `dossier:figures.56.value` `dossier:figures.54.value` `dossier:figures.116.value` `dossier:figures.15.value` `dossier:business.cyclicality`
4. **Apr to Nov 2028.** Operating income reaches about $25bn to $34bn, the level at which 14.1 to 10.2 times EV/EBIT equals $345, and the market stops looking through the trough. 2022-23 is the precedent: trailing EBIT fell 81% in three quarters, and memory stocks fell 60-80% from peak to trough in past cycles, which for this stock is 72% below the June 2026 close high. `calc:({valuation.inputs.price_trading}*0.5*{valuation.inputs.shares}+{valuation.inputs.net_debt})/{derived.ev_ebit_history.median}` `calc:({valuation.inputs.price_trading}*0.5*{valuation.inputs.shares}+{valuation.inputs.net_debt})/{derived.ev_ebit_history.p25}` `calc:{derived.ev_ebit_history.quarters.2023-02-28.ttm_ebit}/{derived.ev_ebit_history.quarters.2022-05-31.ttm_ebit}-1` `calc:(1+{market.drawdown_from_peak_close})*0.5-1` [5](https://www.uncoveralpha.com/p/every-memory-cycle-ends-the-same)

**Leading indicators**

- Quarterly operating margin (80.7% in the August 2026 quarter) falls below 70% < 0.7 `dossier:figures.22.value`
- Consensus FY2027 EPS in dollars (176.50 now; 153.87 ninety days ago) cut below 150 < 150 `dossier:figures.113.value`
- Samsung's HBM revenue share in % (33% in Q2 2026; Samsung says about 40% by Q4) reaches 40 while Micron's stays near 18 >= 40 `dossier:figures.171.value` `dossier:figures.172.value`
- DRAM contract price change quarter on quarter in % (one source forecast 0 to +5% for Q4 2026) turns negative < 0 `dossier:expectations.what_would_change_it`
- Sequential revenue growth in % in the November 2026 quarter (13.9% in consensus) comes in below 5 < 5 `calc:{estimates.trend.2026-11-30.revenueEstimateAvg}/{financials_quarterly.2026-08-31.revenue}-1`

## Objections

| Id | Topic | Severity | Objection |
|---|---|---|---|
| R1 | margin | severe | Earnings are a shortage price. FY2026's operating margin of 74.6% followed 26.4% in FY2025 and -37.0% in FY2023, against a previous peak of 49.3%; DRAM ASP rose about 180% and NAND about 200% on DRAM bits up about 25%. The 10-K says AI-driven demand 'may not be sustainable' and the strategic agreements are estimated at over 35% of revenue through 2030, so most revenue floats. A 50% fall needs only an 18.6% margin on flat revenue at the own median multiple. `dossier:figures.12.value` `dossier:figures.13.value` `dossier:figures.14.value` `dossier:figures.15.value` `dossier:figures.34.value` `dossier:figures.36.value` `dossier:figures.179.value` `dossier:business.cyclicality` `calc:({valuation.inputs.price_trading}*0.5*{valuation.inputs.shares}+{valuation.inputs.net_debt})/{derived.ev_ebit_history.median}/{financials_annual.2026-08-31.revenue}` |
| R2 | multiple | moderate | The price is not cheap against the valuation's own lines. At $690 it is 23.0% above the buy-below line of $560.94 and the base-case DCF value is $728.75 (the price is 5.3% under it), with a base-case return of 7.5% a year on the DCF exit; the reverse DCF needs 17.2% growth a year for ten years, a rate at most 5% of 1,375 comparables achieved. Cash is also not all free: $12.75bn of customer deposits are owed back in 2029-2031 and noncurrent tax payables are rising. `facts:valuation.price_lines_trading.buy_below` `facts:valuation.cases.base.dcf_value_per_share_trading` `dossier:figures.136.value` `dossier:figures.123.value` `dossier:figures.126.value` `dossier:figures.127.value` `dossier:figures.41.value` `calc:{valuation.inputs.price_trading}/{valuation.price_lines_trading.buy_below}-1` |
| R3 | competition | moderate | Supply is being added at the top of the cycle by every producer. Micron's capex was $30.7bn in FY2026 and is guided to about $25bn in the first half of FY2027 net of incentives; Samsung's HBM revenue share rose from 21% to 33% in a quarter while Micron's was 18% (SK hynix 50%); CXMT is about 10% of DRAM revenue and state-backed. A review of past cycles finds oversupply tends to arise within two to three years when all three majors expand together. `dossier:figures.59.value` `dossier:figures.63.value` `dossier:figures.173.value` `dossier:figures.171.value` `dossier:figures.172.value` `dossier:figures.170.value` `dossier:figures.175.value` [8](https://www.forbes.com/sites/greatspeculations/2026/05/14/why-micron-stocks-9x-rally-might-just-be-the-start/) |
| R4 | growth | moderate | Demand is concentrated and the Street needs another doubling. About 60% of FY2026 revenue was data centre and about half came from ten customers, both new risk factors; consensus FY2027 revenue of $275.5bn is 2.07 times FY2026's, while consensus for the November quarter is only 13.9% above the August quarter. The 17.5% one-day fall on 5 Nov 2026 was attributed to fears of slower data-centre build-outs. `dossier:figures.37.value` `dossier:figures.38.value` `dossier:figures.115.value` `dossier:figures.0.value` `calc:{estimates.trend.2026-11-30.revenueEstimateAvg}/{financials_quarterly.2026-08-31.revenue}-1` `dossier:figures.167.value` |
| R5 | capital_allocation | moderate | Through-cycle returns are a commodity's, and spending follows the price. ROIC was 1.0% in FY2016, -9.5% in FY2023 and 1.8% in FY2024 against 110.5% in FY2026. In 2017-2025 operating cash flow less capex was only $15.9bn on about $86.4bn of capex; FY2026 alone had $59.0bn, and the next fabs (Idaho, New York, Hiroshima, Singapore, Tongluo) are being committed at today's price level. `dossier:figures.27.value` `dossier:figures.26.value` `dossier:figures.25.value` `dossier:figures.24.value` `dossier:figures.70.value` `dossier:figures.61.value` `calc:{derived.sum_2017_2026.capex}-{derived.ttm.capex}` |
| R6 | other | moderate | Taiwan makes about 60% of Micron's DRAM, and a Taoyuan union held a warning strike on 22 Oct 2026 and demands 15% of operating profit. Bloomberg reported on 5 Nov that Fab 11E construction (up to $4.5bn) was halted, though Micron says Taiwan operations are normal. The 10-K added strike and stoppage risk factors, including liability under the strategic agreements if deliveries stop; a settlement sets a precedent for cost per bit. `dossier:figures.176.value` `dossier:figures.177.value` `dossier:figures.178.value` `dossier:moat.against` |

## Base rates

- Growth: the price implies 17.2% revenue growth a year for ten years with the margin fading to the industry median of 18.0%, and at most 5% of 1,375 comparables (all industries, USD 50bn and above) grew that fast. Micron's own 2016-2026 CAGR of 26.8% starts at a trough and ends in the price spike. `facts:valuation.expectations.implied_growth_10y`
- Margin: FY2026's 74.6% operating margin compares with 49.3% in FY2018, the previous peak; the other eight of the last nine years ran from -37.0% (FY2023) to 31.5% (FY2021). The industry median the valuation fades to is 18.0%. `facts:valuation.inputs.own_margins_10y.1`
- Multiple: EV/EBIT is 7.45 times trailing against an own median of 14.13, a 25th percentile of 10.23 and a minimum of 6.19. A low multiple on peak earnings has not protected the stock: at 7.14 times in May 2022 trailing EBIT was $11.1bn and nine months later it was $2.1bn. `facts:derived.ev_ebit_history.quarters.2022-05-31.ev_ebit`
- Peak-to-trough: Micron fell about 57% from roughly $64 in May 2018 (4.5 times forward earnings) to about $28 at the end of 2018, and a review of memory cycles puts peak-to-trough stock declines at 60-80% over about two years. A further 50% fall from $690 would be 71.6% below the June 2026 high, inside that range. [1](https://www.trefis.com/stock/mu/articles/599100/micron-stock-surged-9x-but-history-suggests-caution/2026-05-12)
- Revenue: it fell 23.0% in FY2019 and 49.5% in FY2023, the two most recent downturns. Consensus FY2027 revenue of $275.5bn is 2.07 times FY2026's, so the Street needs a second doubling. `facts:derived.revenue_growth_by_year.2023`

## Companies like this that failed

**Micron Technology (the 2018 DRAM and NAND peak) (May 2018 to FY2019).** FY2018 revenue rose to $30.4bn and the operating margin to 49.3% on DRAM and NAND shortage prices, and the stock peaked near $64 in May 2018 at about 4.5 times forward earnings, about two quarters before the fundamentals peaked. Cloud customers then cut orders; NAND prices fell about 60% and DRAM about 40%, FY2019 revenue fell 23% and EPS fell 52%, and the stock was near $28 by year end, down about 57%. *Similarity:* Same company and product set at a shortage-driven peak margin, an AI-like customer-capex story (cloud build-out), a three-supplier industry that was supposed to be disciplined, and a low forward multiple that the market read as a peak. Differences: FY2026's margin and revenue jump are far larger, and the 2026 take-or-pay agreements did not exist in 2018. *Lesson:* A forward multiple below 5 times is what the market pays for peak-cycle earnings, not a margin of safety; the stock fell before earnings did and the fall was larger than the first revisions implied. Watch contract pricing and customer inventories, not the trailing multiple. [1](https://www.trefis.com/stock/mu/articles/599100/micron-stock-surged-9x-but-history-suggests-caution/2026-05-12) [2](https://www.uncoveralpha.com/p/every-memory-cycle-ends-the-same) [3](https://www.stocktitan.net/articles/micron-q4-fy2026-earnings-memory-cycle) [4](https://www.forbes.com/sites/greatspeculations/2019/10/30/after-growing-almost-15x-yoy-in-2018-why-did-microns-revenue-drop-23-in-2019/)

**Elpida Memory (2006-07 capacity build to bankruptcy in February 2012).** Elpida, a top-three DRAM maker, invested aggressively in 2006-07 on the bet that the market would keep expanding. DRAM prices fell sharply in 2009 and again in 2011 (the benchmark 2-gigabit DDR3 chip fell 85%); with a strong yen and Thai floods it filed for bankruptcy with liabilities of 448 billion yen ($5.5bn). Micron bought it in 2013. *Similarity:* A DRAM maker with a large capex programme committed at a high point in the price cycle (Micron: $30.7bn in FY2026, about $25bn guided for the first half of FY2027, with fabs in Idaho, New York, Japan, Singapore and Taiwan) in an industry where Chinese state-backed supply is growing. Differences: Elpida was levered and sub-scale at about 15-18% share, while Micron has net cash of about $41bn on the cache basis, so the comparison is about capex timing and price collapse, not about solvency. *Lesson:* Memory capacity bought at peak prices is paid for in the downturn, and a company can be a top-three producer and still not earn its cost of capital through the cycle. For Micron the equivalent loss is not bankruptcy but returns: ROIC was 1.0% in FY2016, -9.5% in FY2023 and 1.8% in FY2024. [1](https://phys.org/news/2012-03-japan-elpida-delisted-tokyo-stock.html) [2](https://www.networkworld.com/article/706324/data-center-elpida-world-s-third-largest-dram-maker-files-for-bankruptcy.html) [3](https://en.wikipedia.org/wiki/Micron_Memory_Japan) `dossier:figures.26.value`

## Flags

- **falling_sharply (falling_sharply, real risk):** The stock is 43.1% below its 25 Jun 2026 closing high of $1,213.56 and fell 17.5% on 5 Nov 2026, with one-year volatility of 83%. Press attributes the fall to the US midterms, data-centre build-out fears, the Fab 11E report and a chip-sector sell-off; none is a reported change in Micron's results, and the August quarter's operating margin was 80.7%, so the fall is not explained by a fundamental event yet. That is the bear's point: in 2018 the stock peaked about two quarters before fundamentals, and the June 2026 high may be the same lead. The guided slowdown in sequential growth supports reading the fall as the market looking ahead, not noise. `facts:market.drawdown_from_peak_close` `dossier:figures.167.value` `dossier:figures.102.value` `dossier:figures.22.value` [5](https://www.uncoveralpha.com/p/every-memory-cycle-ends-the-same)

## Macro exposure

- US10Y (today 4.867): risk if rises above 5.5. The valuation's discount rate of 9.37% is the US 10-year yield plus 4.5 points, so a rise lifts the rate applied to a stream whose value is mostly in later years; it is also the cost of financing hyperscaler data-centre capex, which is the demand for Micron's HBM and server DRAM. The yield rose 0.78 points in 12 months.
- VIX (today 25.64): risk if stays above 30. A stock with 83% one-year volatility and a 17.5% one-day fall is sold first in a risk-off market; the VIX is already 6.1 points higher than a year ago, and AI-capex names fell together on 4-5 Nov 2026.

## Gaps

- Governance test not triggered: facts.governance.events shows no CFO, chief accounting officer, auditor change or non-reliance event in 24 months; the only officer exit is Sumit Sadana (Chief Business Officer, to Senior Advisor, 26 Aug 2026), with no disagreement stated. No trap flag is at yes and the tier is not tagged crowded, so the only flag response is falling_sharply.
- Failure-case facts come from secondary web pages (Trefis, Forbes, Phys.org, Network World, Wikipedia), not company filings; the 2018 forward P/E of 4.5 times and the 57% fall are Trefis's figures. Two of five web searches were used.
- The valuation's base_rates cells give only the share of comparables reaching the implied growth; there is no margin or multiple distribution for the 1,375 comparables, so margin and multiple base rates rest on Micron's own history (about five cached price years for EV/EBIT).
- The price lines and case returns come from code with the caveats in the dossier (reinvestment overstated in years 1-2, 21% tax rate against 14.8% effective, net cash leaving out $30.0bn of long-term investments). Fixing them would raise the DCF value, which is why R2 is moderate, not severe.
- The facts pack's market block is the 30 Oct close ($884.74) while the valuation uses the 6 Nov close ($690); consensus estimates may not yet reflect the 5 Nov sell-off. The 2022-23 EBIT fall is from quarter-end TTM data and the 2018 timing from secondary sources.
- Conversion to avoid: a November-quarter operating margin below 70%, or negative DRAM contract pricing in the first half of 2027, would make R1 decisive.

## Deviations

None.

## Figures

| Figure | Value | Unit | Period | Source |
|---|---|---|---|---|
| Valuation price (6 Nov 2026 close) | 690 | USD | 6 Nov 2026 | `facts:valuation.inputs.price_trading` |
| Price after a 50% fall | 345 | USD | pre-mortem | `calc:{valuation.inputs.price_trading}*0.5` |
| Market value after a 50% fall | 390.3 | USD bn | pre-mortem | `calc:{valuation.inputs.price_trading}*0.5*{valuation.inputs.shares}` |
| Enterprise value after a 50% fall | 349.7 | USD bn | pre-mortem | `calc:({valuation.inputs.price_trading}*0.5*{valuation.inputs.shares}+{valuation.inputs.net_debt})` |
| Operating income that a 50% fall values at the own median multiple | 24.75 | USD bn | pre-mortem | `calc:({valuation.inputs.price_trading}*0.5*{valuation.inputs.shares}+{valuation.inputs.net_debt})/{derived.ev_ebit_history.median}` |
| Operating income at the own 25th percentile multiple | 34.18 | USD bn | pre-mortem | `calc:({valuation.inputs.price_trading}*0.5*{valuation.inputs.shares}+{valuation.inputs.net_debt})/{derived.ev_ebit_history.p25}` |
| That operating income as a share of FY2026's | 24.91 | % | pre-mortem | `calc:({valuation.inputs.price_trading}*0.5*{valuation.inputs.shares}+{valuation.inputs.net_debt})/{derived.ev_ebit_history.median}/{derived.ttm.operating_income}` |
| That operating income as a margin on FY2026 revenue | 18.58 | % | pre-mortem | `calc:({valuation.inputs.price_trading}*0.5*{valuation.inputs.shares}+{valuation.inputs.net_debt})/{derived.ev_ebit_history.median}/{financials_annual.2026-08-31.revenue}` |
| That operating income as a multiple of FY2025's | 2.51 | x | pre-mortem | `calc:({valuation.inputs.price_trading}*0.5*{valuation.inputs.shares}+{valuation.inputs.net_debt})/{derived.ev_ebit_history.median}/{derived.ev_ebit_history.quarters.2025-08-31.ttm_ebit}` |
| Drawdown from peak close today | -43.12 | % | 6 Nov 2026 | `facts:market.drawdown_from_peak_close` |
| Drawdown from peak close after a further 50% fall | -71.56 | % | pre-mortem | `calc:(1+{market.drawdown_from_peak_close})*0.5-1` |
| Own EV/EBIT median | 14.13 | x | 2021-2026 | `facts:derived.ev_ebit_history.median` |
| Own EV/EBIT 25th percentile | 10.23 | x | 2021-2026 | `facts:derived.ev_ebit_history.p25` |
| Own EV/EBIT minimum | 6.19 | x | 2021-2026 | `facts:derived.ev_ebit_history.min` |
| EV/EBIT at the valuation price | 7.45 | x | TTM | `dossier:figures.104.value` |
| EV/EBIT at 31 May 2022 | 7.14 | x | May 2022 | `facts:derived.ev_ebit_history.quarters.2022-05-31.ev_ebit` |
| Trailing EBIT at 31 May 2022 | 11.14 | USD bn | TTM to May 2022 | `facts:derived.ev_ebit_history.quarters.2022-05-31.ttm_ebit` |
| Trailing EBIT at 28 Feb 2023 | 2.11 | USD bn | TTM to Feb 2023 | `facts:derived.ev_ebit_history.quarters.2023-02-28.ttm_ebit` |
| Fall in trailing EBIT, May 2022 to Feb 2023 | -81.05 | % | 3 quarters | `calc:{derived.ev_ebit_history.quarters.2023-02-28.ttm_ebit}/{derived.ev_ebit_history.quarters.2022-05-31.ttm_ebit}-1` |
| Operating margin FY2026 | 74.59 | % | FY2026 | `facts:financials_annual.2026-08-31.operating_margin` |
| Operating margin FY2025 | 26.41 | % | FY2025 | `facts:financials_annual.2025-08-31.operating_margin` |
| Operating margin FY2023 | -36.97 | % | FY2023 | `facts:financials_annual.2023-08-31.operating_margin` |
| Operating margin FY2018 (previous peak) | 49.34 | % | FY2018 | `facts:financials_annual.2018-08-31.operating_margin` |
| Operating margin FY2021 (highest of the other years) | 31.54 | % | FY2021 | `facts:valuation.inputs.own_margins_10y.5` |
| Operating income FY2018 | 14.99 | USD bn | FY2018 | `facts:financials_annual.2018-08-31.operating_income` |
| Operating margin, quarter to 31 Aug 2026 | 80.68 | % | Q4 FY2026 | `facts:financials_quarterly.2026-08-31.operating_margin` |
| Industry mature operating margin (valuation target) | 17.98 | % | valuation | `facts:valuation.inputs.industry_mature_margin` |
| DRAM ASP change FY2026 (approximate) | 180 | % | FY2026 | `dossier:figures.34.value` |
| NAND ASP change FY2026 (approximate) | 200 | % | FY2026 | `dossier:figures.36.value` |
| DRAM bit shipment change FY2026 (approximate) | 25 | % | FY2026 | `dossier:figures.35.value` |
| Strategic agreements, share of revenue through 2030 (estimate) | 35 | % | to 2030 | `dossier:figures.179.value` |
| Revenue FY2026 | 133.2 | USD bn | FY2026 | `facts:financials_annual.2026-08-31.revenue` |
| Revenue growth FY2019 | -22.98 | % | FY2019 | `facts:derived.revenue_growth_by_year.2019` |
| Revenue growth FY2023 | -49.48 | % | FY2023 | `facts:derived.revenue_growth_by_year.2023` |
| Revenue CAGR 2016-2026 | 26.8 | % | 2016-2026 | `facts:derived.revenue_cagr_2016_2026` |
| Implied 10-year revenue growth in the price | 17.22 | % | valuation | `facts:valuation.expectations.implied_growth_10y` |
| Share of comparables achieving that growth (at most) | 5 | % | valuation | `facts:valuation.expectations.share_of_comparables_achieving` |
| Comparables in the base-rate cell | 1,375 | count | valuation | `facts:valuation.expectations.comparables_n` |
| Price line: full size below | 491.5 | USD | valuation | `facts:valuation.price_lines_trading.full_size_below` |
| Price line: buy below | 560.9 | USD | valuation | `facts:valuation.price_lines_trading.buy_below` |
| Price above the buy-below line | 23.01 | % | 6 Nov 2026 | `calc:{valuation.inputs.price_trading}/{valuation.price_lines_trading.buy_below}-1` |
| Base case DCF value per share | 728.8 | per share | valuation | `facts:valuation.cases.base.dcf_value_per_share_trading` |
| Price against the base case DCF value | -5.32 | % | 6 Nov 2026 | `calc:{valuation.inputs.price_trading}/{valuation.cases.base.dcf_value_per_share_trading}-1` |
| Base case implied 5-year annual return, DCF exit | 7.46 | % | valuation | `facts:valuation.cases.base.implied_return_5y` |
| Consensus revenue FY2027 | 275.5 | USD bn | FY2027 | `facts:estimates.trend.2027-08-31.revenueEstimateAvg` |
| Consensus revenue FY2027 over FY2026 | 2.07 | x | FY2027 | `calc:{estimates.trend.2027-08-31.revenueEstimateAvg}/{financials_annual.2026-08-31.revenue}` |
| Consensus revenue FY2028 | 319.7 | USD bn | FY2028 | `facts:estimates.trend.2028-08-31.revenueEstimateAvg` |
| Consensus revenue, November 2026 quarter | 61.74 | USD bn | Q1 FY2027 | `facts:estimates.trend.2026-11-30.revenueEstimateAvg` |
| Revenue, quarter to 31 Aug 2026 | 54.23 | USD bn | Q4 FY2026 | `facts:financials_quarterly.2026-08-31.revenue` |
| Consensus sequential revenue growth, November 2026 quarter | 13.86 | % | Q1 FY2027 | `calc:{estimates.trend.2026-11-30.revenueEstimateAvg}/{financials_quarterly.2026-08-31.revenue}-1` |
| Consensus EPS FY2027 | 176.5 | per share | FY2027 | `facts:estimates.trend.2027-08-31.earningsEstimateAvg` |
| EPS FY2027 consensus 90 days ago | 153.9 | per share | 90 days earlier | `facts:estimates.trend.2027-08-31.epsTrend90daysAgo` |
| Price over FY2027 consensus EPS | 3.91 | x | FY2027 | `dossier:figures.112.value` |
| Capex FY2026 (gross) | 30.71 | USD bn | FY2026 | `facts:financials_annual.2026-08-31.capex` |
| Capex guidance, first half FY2027 (net of incentives) | 25 | USD bn | H1 FY2027 | `dossier:figures.63.value` |
| Capex 2017-2025 | 86.43 | USD bn | 2017-2025 | `calc:{derived.sum_2017_2026.capex}-{derived.ttm.capex}` |
| Operating cash flow less capex 2017-2025 | 15.86 | USD bn | 2017-2025 | `dossier:figures.70.value` |
| Operating cash flow less capex FY2026 | 58.96 | USD bn | FY2026 | `dossier:figures.61.value` |
| ROIC FY2026 | 110.5 | % | FY2026 | `facts:derived.roic_by_year.2026` |
| ROIC FY2024 | 1.76 | % | FY2024 | `facts:derived.roic_by_year.2024` |
| ROIC FY2023 | -9.52 | % | FY2023 | `facts:derived.roic_by_year.2023` |
| ROIC FY2016 | 0.96 | % | FY2016 | `facts:derived.roic_by_year.2016` |
| Customer deposits received FY2026 | 12.75 | USD bn | FY2026 | `dossier:figures.41.value` |
| Remaining performance obligations | 134 | USD bn | 3 Sep 2026 | `dossier:figures.39.value` |
| Consideration payable to customers | 4.32 | USD bn | 3 Sep 2026 | `dossier:figures.56.value` |
| Receivables at 3 Sep 2026 | 36.2 | USD bn | 3 Sep 2026 | `facts:financials_annual.2026-08-31.receivables` |
| Net cash, valuation basis | 40.64 | USD bn | 3 Sep 2026 | `calc:-{valuation.inputs.net_debt}` |
| Samsung HBM revenue share Q2 2026 | 33 | % | Q2 2026 | `dossier:figures.171.value` |
| Samsung HBM revenue share Q1 2026 | 21 | % | Q1 2026 | `dossier:figures.173.value` |
| SK hynix HBM revenue share Q2 2026 | 50 | % | Q2 2026 | `dossier:figures.170.value` |
| Micron HBM revenue share Q2 2026 | 18 | % | Q2 2026 | `dossier:figures.172.value` |
| CXMT share of DRAM revenue | 10 | % | Q2 2026 | `dossier:figures.175.value` |
| Data-centre share of FY2026 revenue (approximate) | 60 | % | FY2026 | `dossier:figures.37.value` |
| Top-ten customers share of revenue (approximate) | 50 | % | FY2026 | `dossier:figures.38.value` |
| One-day share fall, 5 Nov 2026 | -17.46 | % | 5 Nov 2026 | `dossier:figures.167.value` |
| One-year volatility | 82.99 | % | 1y | `facts:market.vol_1y` |
| Peak close, 25 Jun 2026 | 1,214 | USD | 25 Jun 2026 | `dossier:figures.169.value` |
| Taiwan share of Micron DRAM output (approximate) | 60 | % | 2026 | `dossier:figures.176.value` |
| Fab 11E budget, upper end | 4.5 | USD bn | 2026 | `dossier:figures.178.value` |
| Discount rate used in the valuation | 9.37 | % | valuation | `facts:valuation.inputs.discount_rate` |
| US 10-year yield | 4.867 | % | 6 Nov 2026 | `facts:macro.US10Y.latest` |
| US 10-year yield change in 12 months | 0.779 | points | 12m | `facts:macro.US10Y.change_12m` |
| VIX | 25.64 | points | 6 Nov 2026 | `facts:macro.VIX.latest` |
| VIX change in 12 months | 6.14 | points | 12m | `facts:macro.VIX.change_12m` |
| Micron stock fall May to Dec 2018 (Trefis) | 57 | % | 2018 | [1](https://www.trefis.com/stock/mu/articles/599100/micron-stock-surged-9x-but-history-suggests-caution/2026-05-12) |
| Micron peak price May 2018 (Trefis) | 64 | USD | May 2018 | [1](https://www.trefis.com/stock/mu/articles/599100/micron-stock-surged-9x-but-history-suggests-caution/2026-05-12) |
| Micron price at end of 2018 (Trefis) | 28 | USD | Dec 2018 | [1](https://www.trefis.com/stock/mu/articles/599100/micron-stock-surged-9x-but-history-suggests-caution/2026-05-12) |
| Micron forward P/E at the May 2018 peak (Trefis) | 4.5 | x | May 2018 | [1](https://www.trefis.com/stock/mu/articles/599100/micron-stock-surged-9x-but-history-suggests-caution/2026-05-12) |
| Memory stock peak-to-trough fall, low end (uncoveralpha) | 60 | % | past cycles | [1](https://www.uncoveralpha.com/p/every-memory-cycle-ends-the-same) |
| Memory stock peak-to-trough fall, high end (uncoveralpha) | 80 | % | past cycles | [1](https://www.uncoveralpha.com/p/every-memory-cycle-ends-the-same) |
| Elpida liabilities at bankruptcy | 448 | local bn | Feb 2012 | [1](https://phys.org/news/2012-03-japan-elpida-delisted-tokyo-stock.html) |
| Elpida liabilities at bankruptcy in USD (about) | 5.5 | USD bn | Feb 2012 | [1](https://www.networkworld.com/article/706324/data-center-elpida-world-s-third-largest-dram-maker-files-for-bankruptcy.html) |
| Benchmark DDR3 2Gb price fall in 2011 (Wikipedia) | 85 | % | 2011 | [1](https://en.wikipedia.org/wiki/Micron_Memory_Japan) |
