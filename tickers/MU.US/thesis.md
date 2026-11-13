# MU.US thesis

Run 2026-11-07-semis, as of 2026-11-07, claims version 2. The bull's case; the Judge sets the verdict. Rendered from thesis.json and claims.json by check_thesis.py; edit those, not this file.

## Summary

Pursue cannot be reached: the high case's year-5 value is 3.57 times the base case's, over the 2.5 limit, so no buy line or zone is published, and no claim clears that. The code's total is 61.65 against 70 (maximum reachable 65.15). The 10-K's single-supplier disclosure costs 15 moat points. Valuation decides how near the total gets: it scores 0 on a 7.46% base-case return, after -20 for rare growth and -10 for the low case. Core claim C1: the mature operating margin is at least Micron's own ten-year median of 27.645%, not the 17.98% industry median the code fades it to. If C1 is supported, the code's base case returns 14.05% a year with a buy line of $755.67, above the $690 price, and the total is 66.15. C2 rebuts the severe peak-earnings flag (TTM operating income at or above $99.34bn through FY2028). C3 says the code overcharges reinvestment. Both macro conditions hold today (US 10-year 4.867% below 5.5; CMDI_IG 0.25 below 0.5).

## Thesis in three sentences

At $690 the market pays 7.45 times TTM EBIT, below Micron's own 25th percentile of 10.23, because it prices FY2026's 74.59% operating margin as a peak that will fall back to industry levels. Take-or-pay contracts with price floors, $134bn of them at minimum pricing, make Micron's own ten-year median margin of 27.645% the right end point rather than the 17.98% industry median (C1); on that margin the code's base case returns 14.05% a year. The case is wrong if TTM operating margin falls below 46.28% or TTM operating income below $85bn at two consecutive quarter-ends before the August 2028 quarter.

## Score (computed in code)

| Dimension | Points |
|---|---|
| quality | 100 |
| growth | 87 |
| moat | 35 |
| management | 70 |
| valuation | 0 |
| **Total** | **61.65** (maximum reachable 65.15; pursue needs 70) |

Pursue is blocked: maximum reachable total 65.15 is below 70; base-case implied 5-year return 7.5% is below the 12% hurdle; the high case's year-5 value is 3.6x the base case's (over 2.5x), so no buy line or zone is published.

## Claims

| Id | Role | Claim | Test | Kill | Review by | Share of gap |
|---|---|---|---|---|---|---|
| C1 | core | Micron's mature operating margin is at least 27.645%, the median of its own annual operating margins over FY2017-FY2026. The code's Track B base case instead fades the margin over ten years to 17.98%, the Semiconductors & Semiconductor Equipment median. The own median already includes the FY2023 trough (-36.97%) as well as the FY2026 spike (74.59%). The case for a higher floor than in past cycles rests on contracts that are new this year. The take-or-pay strategic customer agreements carry minimum and maximum price bands. Remaining performance obligations were about $134bn at 3 Sep 2026, measured at committed volumes and minimum pricing (10-K Note 16, Revenue and Customer Contract Liabilities). About one-fourth is due within twelve months and all within five years, secured by $12.75bn of customer deposits and $7bn of letters of credit. The 10-K says gross margins under these agreements, even at floor prices, should be meaningfully above peak quarterly margins in any past cycle; the best past annual gross margin was 58.87% (FY2018). Against the claim, a secondary source estimates the agreements at over 35% of revenue through 2030, so most revenue still follows market prices, and revenue fell in 7 of the last 19 years. Override: margin_target 0.27645. Test: TTM operating margin of at least 50% at every quarter-end through the August 2028 quarter (FY2028). That is above every annual margin before FY2026 (peak 49.34% in FY2018); the code's own path is 68.93% in year 1 and 63.27% in year 2. | Trailing-12-month operating margin >= 50 (each quarter-end to the August 2028 quarter (FY2028)) | TTM operating margin below 46.28% at two consecutive quarter-ends before the review. That is the code's own year-5 base margin reached within two years and below the FY2018 peak of 49.34%: margins fading more than twice as fast as the code's path, so the price-band contracts did not change the cycle. | 2028-10-31 | 1.000 (measured) |
| C2 | supporting | Dossier red flag 0 says earnings and margins are at a shortage peak and price-driven: a 74.59% FY2026 operating margin against a ten-year range of -36.97% to 74.59%. The answer is that FY2026 is not the earnings peak. TTM operating income stays at or above the FY2026 figure of $99.34bn at every quarter-end through the August 2028 quarter. The August 2026 quarter alone earned $43.75bn of operating income on $54.23bn of revenue. The company guided $61.5bn of revenue for the November 2026 quarter (CNBC report of the 30 Sep 2026 release), and in that quarter the November 2025 quarter's $6.14bn drops out of the trailing sum. Consensus revenue is $275.5bn for FY2027 and $319.7bn for FY2028. About one-fourth of the $134bn of remaining performance obligations, measured at minimum pricing, falls in the next twelve months. The test therefore bites in FY2028, when Micron's own Idaho fab (first wafers mid-2027), CXMT and Samsung add supply. | Trailing-12-month operating income >= 99.34 (each quarter-end to the August 2028 quarter (FY2028)) | TTM operating income below $85bn at two consecutive quarter-ends. Quarterly operating income would then be averaging under about $21bn against $43.75bn in the August 2026 quarter: a cyclical fall the contracts did not stop, so FY2026 was the peak. | 2028-10-31 | 0.050 (estimate) |
| C3 | supporting | The code's base case charges reinvestment at a sales-to-capital ratio of 0.852 on revenue growth that is mostly price. Its free cash flow to the firm, $26.49bn in year 1 and $26.76bn in year 2, is therefore far below what the business will produce. TTM operating cash flow less capex stays at or above $52.99bn, twice the code's year-1 figure, at every quarter-end through the August 2028 quarter. In FY2026 Micron added $95.81bn of revenue on $30.71bn of capex and produced $58.96bn of operating cash flow less capex. For year 1's added revenue the code charges $85.79bn of reinvestment. Against the claim: capex is guided at about $25bn, net of incentives, in the first half of FY2027 and higher in the second half. FY2026 cash taxes of $1.25bn ran far below the $14.76bn provision and will catch up. Receivables rose $25.2bn in the year. | TTM operating cash flow less TTM capex >= 52.99 (each quarter-end to the August 2028 quarter (FY2028)) | TTM operating cash flow less capex below $26.49bn, the code's own year-1 free cash flow to the firm, at two consecutive quarter-ends. The code's reinvestment charge would then be right, and the extra value the Analyst's case comments describe would not exist. | 2028-10-31 | 0.150 (estimate) |

If C1 is supported, the base case returns 14.1% a year (49.3% at the industry exit), against 7.5% today.

**Macro conditions**

- M1: US10Y < 5.5 (today 4.867). The code's discount rate is the US 10-year yield (4.867% today) plus 4.5%, and the DCF cap on the exit multiple, which sets the base case's 4.54x exit, comes from it. A yield above 5.5% would raise the discount rate by more than 60 basis points and cut the value of the margins C1 says will last.
- M2: CMDI_IG < 0.5 (today 0.25). About 60% of FY2026 revenue was data centre, and the take-or-pay volumes behind C1 and C2 depend on hyperscale customers funding their AI data-centre builds; the 10-K added data-centre build-out delays as a risk factor. CMDI_IG (0.25 today) above 0.5 would mean investment-grade corporate credit is impaired, which threatens that funding and the customers' purchase commitments.

## Mispricing

**Market view.** On the code's Track B rule (margin fading from 74.59% to the 17.98% industry median over ten years), the $690 price needs 17.22% revenue growth a year for ten years, which at most 5% of 1,375 comparables achieved. If today's margin were simply held, it needs revenue to shrink 4.16% a year. Enterprise value is 7.45 times TTM EBIT, against an own median of 14.13 and a minimum of 6.19. The market is pricing a margin collapse, not a growth path.

**Our view.** The fade's end point is too low for the business Micron has become. Its own ten-year median operating margin of 27.645%, a span that includes the FY2023 trough, is the better base rate, and the contracts signed in FY2026 put a floor under part of the volume (C1). FY2026 is not the earnings peak: the August 2026 quarter alone earned $43.75bn of operating income (C2). Cash generation is far above the code's free cash flow to the firm (C3). On C1 alone, the code's base case returns 14.05% a year and the buy line rises to $755.67.

**Catalyst (2027-09-01 to 2027-12-31, C1).** The FY2027 results and 10-K (fiscal year to early September 2027; the FY2026 release came on 30 Sep 2026) and the first-quarter FY2028 results. This is the first full fiscal year under the strategic customer agreements and the first period in which the Idaho fab's first wafers (mid-2027) add supply. TTM operating margin at or above 50% through those results would show that the fade the price assumes is not happening (C1).

## Supply-chain position

The map places Micron in the memory-and-storage tier with high AI-capex exposure: about 60% of FY2026 revenue was data centre. Nvidia's and Qualcomm's 10-Ks name Micron as a memory supplier. Lam Research, Rambus and Silicon Motion name it as a customer. The 10-K names Samsung, SK hynix, Sandisk, CXMT and YMTC as competitors. The map proposes no chokepoint and the dossier records none, so the moat score gets no chokepoint points. The tier is not crowded; XSD had a 4-week outflow of 7.76% of assets and XLK an inflow of 1.38%.

## Valuation

The code's base case takes consensus growth of 54.88% a year for two years, then base rates, with the margin fading to 17.98% (46.28% in year 5). Its exit is the DCF cap of 4.54 times EBIT, against 32.26 for the industry. That gives 7.46% a year (46.45% at the industry exit), a DCF value of $728.75 and a buy line of $560.94 against the $690 price. The low case returns -20.92% and the high case 38.63%; the high case is 3.57 times the base at year 5, so no zone is published. C1's what-if (margin_target 27.645%, priced after the claims were pushed) gives an exit of 6.25 times, 14.05% a year, a DCF value of $968.33 and a buy line of $755.67, a measured share of the gap of 1.0. The thesis makes no exit-multiple claim: the own EV/EBIT history covers 15 quarter-ends from November 2021 (median 14.13, 25th percentile 10.23, 75th 18.85), and its 85.51 maximum was set on trough earnings. The Analyst's caveats (overstated reinvestment, a 21.04% tax rate, net cash leaving out $30.0bn of long-term investments) all point to a higher value.

## Bull case

Operating income was $43.75bn in the August 2026 quarter, at an 80.68% margin. Remaining performance obligations under take-or-pay agreements are $134bn, measured at minimum pricing, and are backed by $12.75bn of deposits and $7bn of letters of credit. Net cash on the broad basis is about $68.3bn. Consensus revenue rises to $319.7bn in FY2028. At 7.45 times TTM EBIT, the earnings yield stays high even if the margin halves, and the code's own base case returns 14.05% if the margin settles at Micron's own median.

## Bear case

FY2026 was price, not volume: DRAM prices rose about 180% on bit growth in the mid-20% range. Operating margins over ten years ran from -36.97% to 74.59%, and revenue fell in 7 of 19 years, including -49.48% in FY2023. Micron, Samsung, SK hynix and CXMT are all adding capacity, and Micron guides about $25bn of capex in the first half of FY2027 alone. The agreements are estimated at only over 35% of revenue, and a Taiwan labour dispute affects about 60% of DRAM output. Insiders sold $338.53m and bought $7.82m.

## Peers

- **Samsung Electronics**: The largest memory maker and a named competitor. The dossier cites Counterpoint (via a secondary source) for Samsung's HBM revenue share rising from 21% to 33% between Q1 and Q2 2026, against Micron's 18%.
- **SK hynix**: A named competitor and HBM leader, with a 50% HBM revenue share in Q2 2026 (Counterpoint, secondary). The cache holds no SK hynix figures.
- **Sandisk**: A NAND competitor, deep-dived in this run, that has signed similar multi-year agreements with floor prices. Unlike Micron it has no DRAM and no fabs of its own.
- **CXMT**: State-backed Chinese DRAM maker named in the 10-K, about 10% of DRAM revenue (Counterpoint, per industry reports). The main new supply risk to C1 and C2.

## Kill criteria

- TTM operating margin below 46.28%, the code's year-5 base margin, at two consecutive quarter-ends before the August 2028 quarter. That is below the FY2018 peak of 49.34%, and would mean the price-band contracts have not changed the cycle. (C1)
- TTM operating income below $85bn at two consecutive quarter-ends, meaning quarterly operating income averaging under about $21bn against $43.75bn in the August 2026 quarter. FY2026 would then have been the peak. (C2)
- TTM operating cash flow less capex below $26.49bn, the code's year-1 free cash flow to the firm, at two consecutive quarter-ends. The code's reinvestment charge would then be right. (C3)

## Reopen conditions

- A later valuation run in which the high case's year-5 value is at most 2.5 times the base case's, so a buy line and zone are published. This is the blocker no claim can clear today.
- The price at or below the code's base-case buy line of $560.94, or at or below $755.67 if the Judge supports C1.
- TTM operating margin at or above 50% and TTM operating income above $99.34bn at the August 2027 quarter, the first full fiscal year under the strategic customer agreements (C1 and C2 holding).
- The FY2026 proxy, when filed, showing executive pay tied to per-share or return metrics, plus a guidance record in the cache. Those inputs are worth up to 3.5 points of total, and are null today.

Next review: 2026-12-18.

## Gaps

- Guidance record: no history of guided against actual results is in the cache, so the guidance input is null (0 points).
- Pay: the FY2026 proxy is not filed and no proxy rows are in the cache; CEO pay comes only from a secondary summary of the FY2025 proxy, so pay_tied_to_returns is null (0 points).
- Remaining performance obligations ($134bn) and the strategic agreements' share of revenue (over 35%, secondary) are not cache series, so no claim uses them as a metric_ref; C1 and C2 test their effect through TTM margin and operating income.
- HBM shares and CXMT's DRAM share come from secondary pages relaying Counterpoint; the November-quarter guidance comes from CNBC's report, not the release.
- The 10-K's floor-price gross margin statement compares with 'peak quarterly margins in any past cycle'; the cache's quarterly history starts in November 2023, so FY2018's annual gross margin of 58.87% is used as a lower bound on that peak.

## Deviations

- Pursue is blocked, so every section except the claims, kill criteria and reopen conditions is kept to a few sentences (step 2 of the instructions).

## Figures

| Figure | Value | Unit | Period | Source |
|---|---|---|---|---|
| Valuation price (6 Nov 2026 close) | 690 | USD | 6 Nov 2026 | `facts:valuation.inputs.price_trading` |
| High case year-5 value over base case year-5 value | 3.57 | x | year 5 | `facts:valuation.high_to_base_year5` |
| Limit above which no zone is published | 2.5 | x | valuation | `facts:valuation.high_to_base_limit` |
| Thesis total (computed in code) | 61.65 | points | as of | `scores:total` |
| Maximum reachable total | 65.15 | points | as of | `scores:max_reachable_total` |
| Valuation dimension points | 0 | points | as of | `scores:dimensions.valuation` |
| Moat dimension points | 35 | points | as of | `scores:dimensions.moat` |
| Base case implied 5-year annual return, DCF exit | 7.46 | % | 5y | `facts:valuation.cases.base.implied_return_5y` |
| Base case implied 5-year annual return, industry exit | 46.45 | % | 5y | `facts:valuation.cases.base.implied_return_5y_industry_exit` |
| Base case DCF exit multiple | 4.54 | x | year 5 | `facts:valuation.cases.base.exit_ev_ebit` |
| Industry exit multiple | 32.26 | x | year 5 | `facts:valuation.cases.base.exit_ev_ebit_industry` |
| Base case DCF value per share | 728.8 | per share | valuation | `facts:valuation.cases.base.dcf_value_per_share_trading` |
| Base case buy line | 560.9 | USD | valuation | `facts:valuation.price_lines_trading.buy_below` |
| Consensus growth a year for the first two years | 54.88 | % | 2y | `facts:valuation.cases.base.growth_first_years` |
| Base case year-5 operating margin | 46.28 | % | year 5 | `facts:valuation.cases.base.path.4.margin` |
| Base case year-1 operating margin | 68.93 | % | year 1 | `facts:valuation.cases.base.path.0.margin` |
| Base case year-2 operating margin | 63.27 | % | year 2 | `facts:valuation.cases.base.path.1.margin` |
| Low case implied 5-year annual return | -20.92 | % | 5y | `facts:valuation.cases.low.implied_return_5y` |
| High case implied 5-year annual return | 38.63 | % | 5y | `facts:valuation.cases.high.implied_return_5y` |
| C1 what-if: base case 5-year annual return | 14.05 | % | 5y | `scores:what_if.C1.implied_return_5y` |
| C1 what-if: buy line | 755.7 | USD | valuation | `scores:what_if.C1.price_lines_trading.buy_below` |
| C1 what-if: exit multiple | 6.25 | x | year 5 | `scores:what_if.C1.exit_ev_ebit` |
| C1 what-if: DCF value per share | 968.3 | per share | valuation | `scores:what_if.C1.dcf_value_per_share_trading` |
| C1 measured share of the gap | 1 | ratio | valuation | `scores:what_if.C1.share_of_gap_measured` |
| Total if C1 is supported | 66.15 | points | as of | `scores:what_if.C1.total_if_supported` |
| TTM operating margin | 74.59 | % | TTM to Aug 2026 | `facts:derived.ttm.operating_margin` |
| Own median annual operating margin FY2017-FY2026 | 27.64 | % | FY2017-FY2026 | `calc:({valuation.inputs.own_margins_10y.8}+{valuation.inputs.own_margins_10y.0})/2` |
| Industry mature operating margin (Track B target) | 17.98 | % | valuation | `facts:valuation.inputs.industry_mature_margin` |
| Operating margin FY2018 (previous peak) | 49.34 | % | FY2018 | `facts:financials_annual.2018-08-31.operating_margin` |
| Gross margin FY2018 | 58.87 | % | FY2018 | `facts:financials_annual.2018-08-31.gross_margin` |
| Operating margin FY2023 (trough) | -36.97 | % | FY2023 | `facts:financials_annual.2023-08-31.operating_margin` |
| Revenue growth FY2023 | -49.48 | % | FY2023 | `facts:derived.revenue_growth_by_year.2023` |
| Implied 10-year revenue growth (Track B) | 17.22 | % | 10y | `facts:valuation.expectations.implied_growth_10y` |
| Implied growth with today's margin held | -4.16 | % | 10y | `facts:valuation.expectations.implied_growth_10y_track_a` |
| Share of comparables achieving the implied growth (at most) | 5 | % | 10y | `facts:valuation.expectations.share_of_comparables_achieving` |
| Comparables in the base-rate cell | 1,375 | count | 10y | `facts:valuation.expectations.comparables_n` |
| EV/EBIT at the valuation price on TTM operating income | 7.45 | x | TTM | `calc:{valuation.inputs.enterprise_value}/{derived.ttm.operating_income}` |
| Own EV/EBIT median | 14.13 | x | Nov 2021 to Aug 2026 | `facts:derived.ev_ebit_history.median` |
| Own EV/EBIT 25th percentile | 10.23 | x | Nov 2021 to Aug 2026 | `facts:derived.ev_ebit_history.p25` |
| Own EV/EBIT 75th percentile | 18.85 | x | Nov 2021 to Aug 2026 | `facts:derived.ev_ebit_history.p75` |
| Own EV/EBIT minimum | 6.19 | x | Nov 2021 to Aug 2026 | `facts:derived.ev_ebit_history.min` |
| Own EV/EBIT maximum (trough earnings) | 85.51 | x | Nov 2021 to Aug 2026 | `facts:derived.ev_ebit_history.max` |
| Own EV/EBIT quarter-ends in the history | 15 | count | Nov 2021 to Aug 2026 | `facts:derived.ev_ebit_history.n` |
| TTM operating income | 99.34 | USD bn | TTM to Aug 2026 | `facts:derived.ttm.operating_income` |
| Operating income, quarter to 31 Aug 2026 | 43.75 | USD bn | Q4 FY2026 | `facts:financials_quarterly.2026-08-31.operating_income` |
| Operating margin, quarter to 31 Aug 2026 | 80.68 | % | Q4 FY2026 | `facts:financials_quarterly.2026-08-31.operating_margin` |
| Consensus revenue FY2028 | 319.7 | USD bn | FY2028 | `facts:estimates.trend.2028-08-31.revenueEstimateAvg` |
| TTM operating cash flow less capex | 58.96 | USD bn | TTM to Aug 2026 | `calc:{derived.ttm.ocf}-{derived.ttm.capex}` |
| Base case free cash flow to the firm, year 1 | 26.5 | USD bn | year 1 | `facts:valuation.cases.base.path.0.fcff` |
| Tax rate in the valuation | 21.04 | % | valuation | `facts:valuation.inputs.tax_rate` |
| Long-term marketable investments left out of net cash | 30.02 | USD bn | 3 Sep 2026 | `tickers/MU.US/cache/sections/0000723125-26-000023_8.txt` |
| Remaining performance obligations at minimum pricing | 134 | USD bn | 3 Sep 2026 | `tickers/MU.US/cache/sections/0000723125-26-000023_8.txt` |
| Customer deposits under strategic agreements | 12.75 | USD bn | FY2026 | `tickers/MU.US/cache/sections/0000723125-26-000023_7.txt` |
| Letters of credit backing strategic agreements | 7 | USD bn | 3 Sep 2026 | `tickers/MU.US/cache/sections/0000723125-26-000023_7.txt` |
| Net cash, all marketable investments less all debt incl. leases (approximate) | 68.27 | USD bn | 3 Sep 2026 | `dossier:figures.66.value` |
| Capex guidance, first half FY2027 (net of incentives) | 25 | USD bn | H1 FY2027 | `tickers/MU.US/cache/sections/0000723125-26-000023_7.txt` |
| Insider sale value in 12 months | 338.5 | USD m | 12m | `facts:ownership.insiders.sale_value_12m` |
| Insider purchase value in 12 months | 7.822 | USD m | 12m | `facts:ownership.insiders.purchase_value_12m` |
| US 10-year yield (M1) | 4.867 | % | 6 Nov 2026 | `facts:macro.US10Y.latest` |
| CMDI investment grade (M2) | 0.25 | points | 23 Oct 2026 | `facts:macro.CMDI_IG.latest` |
| XSD 4-week flow | -7.76 | % | 4 weeks to 30 Oct 2026 | `facts:map.tier.overlay.baskets.1.flow_4w_pct_aum` |
| XLK 4-week flow | 1.38 | % | 4 weeks to 30 Oct 2026 | `facts:map.tier.overlay.baskets.0.flow_4w_pct_aum` |
