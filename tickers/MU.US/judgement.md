# MU.US judgement

Run 2026-11-07-semis, as of 2026-11-13, claims version 2 (SHA-256 b7049135259f). Rendered from judgement.json by check_judgement.py.

**Verdict: watch. Conviction 2.** Pursue fails. The effective base-case return is 7.46%, below 12%, because no deviation claim is Supported. The severe flag is unresolved, the mispricing does not hold and no claim is Supported. The rule then gives watch: the core claim is Contested, not Unsupported, no kill that applies today is breached, and the business is sound on ROIC (110.54% against a 9.37% discount rate). The next evidence is the November-quarter results due 16 Dec 2026.

Probability the thesis is intact at 12 months: 0.90. All three claims are in scope through their kills, which apply now. No test is due within 12 months (review_by 2028-10-31). Each kill needs two consecutive quarter-ends in breach. The quarters reported by November 2027 run to August 2027, and the TTM figures then include the guided November 2026 quarter and the consensus February 2027 quarter, both at record levels. For C1's TTM margin to fall below 46.28%, C2's TTM operating income below $85bn, or C3's TTM operating cash flow less capex below $26.49bn at two quarter-ends by then, the cycle would have to collapse within about two quarters of a record guide. That is faster than the 2022-23 fall, when TTM EBIT took three quarters to drop 81%. The Red Team's leading indicators would warn first: a quarterly margin under 70%, a cut in FY2027 EPS consensus, or negative DRAM contract prices. Residual risk is a sharp 2027 break plus cash taxes and capex catching up for C3, and measurement noise in the cache's quarterly cash flow. The Red Team was blind, so its case is weighed in full.

## Summary

Watch. Micron is a sound business on the rule (FY2026 ROIC 110.54% against a 9.37% discount rate), but none of the three claims is Supported. C1 (core, mature margin at least the own 27.645% median, tested as TTM operating margin of at least 50% through FY2028) rests on contracted evidence, $134bn of remaining performance obligations at minimum pricing, but those cover a minority of revenue, and a 2019-style first downturn year applied to today's 80.68% quarterly margin lands near 51.5%. That makes it Contested at 0.45. C2 (TTM operating income at least $99.34bn through FY2028) and C3 (TTM operating cash flow less capex at least $52.99bn) are Contested too: guidance and consensus support them near term, but the past cycles turned within two years of a peak. The severe peak-earnings flag stays unresolved. Both macro conditions hold. The mispricing does not hold: the price is 5.3% under the base-case DCF value and the market's fade has history behind it. The effective base case is the code's, at 7.46% a year.

## Rulings

| Claim | Role | Ruling | Reasoning |
|---|---|---|---|
| C1: Micron's mature operating margin is at least 27.645%, the median of its own annual operating margins over FY2017-FY2026. The code's Track B base case instead fades the margin over ten years to 17.98%, the Semiconductors & Semiconductor Equipment median. The own median already includes the FY2023 trough (-36.97%) as well as the FY2026 spike (74.59%). The case for a higher floor than in past cycles rests on contracts that are new this year. The take-or-pay strategic customer agreements carry minimum and maximum price bands. Remaining performance obligations were about $134bn at 3 Sep 2026, measured at committed volumes and minimum pricing (10-K Note 16, Revenue and Customer Contract Liabilities). About one-fourth is due within twelve months and all within five years, secured by $12.75bn of customer deposits and $7bn of letters of credit. The 10-K says gross margins under these agreements, even at floor prices, should be meaningfully above peak quarterly margins in any past cycle; the best past annual gross margin was 58.87% (FY2018). Against the claim, a secondary source estimates the agreements at over 35% of revenue through 2030, so most revenue still follows market prices, and revenue fell in 7 of the last 19 years. Override: margin_target 0.27645. Test: TTM operating margin of at least 50% at every quarter-end through the August 2028 quarter (FY2028). That is above every annual margin before FY2026 (peak 49.34% in FY2018); the code's own path is 68.93% in year 1 and 63.27% in year 2. | core | **Contested** | The evidence row shows TTM operating margin at 74.586% against a 50% test and a 46.28% kill (prep evidence 0): the test passes today and the kill is far off. The guided and consensus November and February quarters keep the TTM above 50% well into 2027. So the claim turns on FY2028, the four quarters to August 2028. The contracted evidence is real: $134bn of remaining performance obligations at committed volumes and minimum pricing, about 25% due within twelve months, backed by $12.75bn of deposits and $7bn of letters of credit. The 10-K says floor-price gross margins should be above any past cycle's peak quarterly margin. But the 10-K also says these obligations are not indicative of future revenue. The company's own estimate, relayed by a secondary source, puts the agreements at over 35% of revenue through 2030, so most revenue still follows market prices, which went to a -9.1% gross margin in FY2023. The base rate argues against a structural change. In the first downturn year after the 2018 peak, the margin kept 64% of its level (49.34% to 31.51%). The same ratio applied to the August 2026 quarter's 80.68% gives about 51.5%, right on the test line. A 2023-style fall (31.54% to -36.97%) breaks it outright. R1 (shortage price) and R3 (supply from Samsung, CXMT and Micron's own Idaho fab from mid-2027, inside the test window) are not answered by the contracts. Depreciation from capex of $30.7bn in FY2026 and about $25bn in the first half of FY2027 alone also weighs on the margin. If FY2028 is not a downturn year the claim passes, and the contracts cushion a mild one. I put that at a little under even. The contracted evidence does not make the claim more likely than not, so it is Contested, not Supported. (weighed R1, R3) `prep:evidence.0.value_now` `prep:evidence.0.test_threshold_base` `prep:evidence.0.kill_threshold_base` `prep:evidence.0.kill_breached_now` `dossier:figures.39.value` `dossier:figures.40.value` `dossier:figures.41.value` `dossier:figures.42.value` `dossier:figures.179.value` `tickers/MU.US/cache/sections/0000723125-26-000023_7.txt` `tickers/MU.US/cache/sections/0000723125-26-000023_8.txt` `facts:financials_quarterly.2026-08-31.operating_margin` `facts:financials_annual.2018-08-31.operating_margin` `facts:valuation.inputs.own_margins_10y.2` `facts:valuation.inputs.own_margins_10y.5` `facts:financials_annual.2023-08-31.operating_margin` `calc:{financials_quarterly.2026-08-31.operating_margin}*{valuation.inputs.own_margins_10y.2}/{valuation.inputs.own_margins_10y.1}` `dossier:business.cyclicality` `dossier:figures.59.value` `dossier:figures.63.value` `redteam:objections.0.statement` `redteam:objections.2.statement` |
| C2: Dossier red flag 0 says earnings and margins are at a shortage peak and price-driven: a 74.59% FY2026 operating margin against a ten-year range of -36.97% to 74.59%. The answer is that FY2026 is not the earnings peak. TTM operating income stays at or above the FY2026 figure of $99.34bn at every quarter-end through the August 2028 quarter. The August 2026 quarter alone earned $43.75bn of operating income on $54.23bn of revenue. The company guided $61.5bn of revenue for the November 2026 quarter (CNBC report of the 30 Sep 2026 release), and in that quarter the November 2025 quarter's $6.14bn drops out of the trailing sum. Consensus revenue is $275.5bn for FY2027 and $319.7bn for FY2028. About one-fourth of the $134bn of remaining performance obligations, measured at minimum pricing, falls in the next twelve months. The test therefore bites in FY2028, when Micron's own Idaho fab (first wafers mid-2027), CXMT and Samsung add supply. | supporting | **Contested** | TTM operating income is $99.34bn, exactly the test line, and the kill is $85bn (prep evidence 1). The near term is firmly for the claim. The November 2025 quarter's $6.14bn drops out next, against consensus November-quarter revenue of $61.74bn and the August quarter's $43.75bn of operating income, so FY2026 is not the trailing peak. Consensus revenue is $275.51bn for FY2027 and $319.68bn for FY2028. The binding test is FY2028, which needs about a quarter of today's run-rate per quarter, roughly $25bn. That threshold is far below consensus, which is why this is more likely than not. History argues against calling it Supported. FY2019 operating income fell to about half of FY2018's, and a similar fall from a FY2027 near consensus lands close to $99bn. The 2022-23 downturn cut TTM EBIT 81% in three quarters (R1's precedent), and that would fail it. R3 (supply arriving 2027-28) and R4 (data-centre concentration, a 17.5% one-day fall on build-out fears) are not answered beyond consensus. R6 (Taiwan labour, about 60% of DRAM output) adds cost and delivery risk. The contracted floor helps but covers a minority of revenue. Evidence on both sides, leaning for: Contested at 0.58. (weighed R1, R3, R4, R6) `prep:evidence.1.value_now` `prep:evidence.1.kill_threshold_base` `facts:financials_quarterly.2025-11-30.operating_income` `facts:financials_quarterly.2026-08-31.operating_income` `facts:estimates.trend.2026-11-30.revenueEstimateAvg` `facts:estimates.trend.2027-08-31.revenueEstimateAvg` `facts:estimates.trend.2028-08-31.revenueEstimateAvg` `dossier:figures.39.value` `dossier:figures.179.value` `redteam:figures.18.value` `redteam:objections.0.statement` `redteam:objections.2.statement` `redteam:objections.3.statement` `redteam:objections.5.statement` `dossier:red_flags.0` |
| C3: The code's base case charges reinvestment at a sales-to-capital ratio of 0.852 on revenue growth that is mostly price. Its free cash flow to the firm, $26.49bn in year 1 and $26.76bn in year 2, is therefore far below what the business will produce. TTM operating cash flow less capex stays at or above $52.99bn, twice the code's year-1 figure, at every quarter-end through the August 2028 quarter. In FY2026 Micron added $95.81bn of revenue on $30.71bn of capex and produced $58.96bn of operating cash flow less capex. For year 1's added revenue the code charges $85.79bn of reinvestment. Against the claim: capex is guided at about $25bn, net of incentives, in the first half of FY2027 and higher in the second half. FY2026 cash taxes of $1.25bn ran far below the $14.76bn provision and will catch up. Receivables rose $25.2bn in the year. | supporting | **Contested** | TTM operating cash flow less capex is $58.963bn against a $52.99bn test and a $26.49bn kill (prep evidence 2). The claim's point is right for the near term. Price-driven revenue needed little capital in FY2026: revenue up $95.8bn on $30.71bn of capex. So the code's year-1 free cash flow to the firm of $26.495bn understates cash generation while prices hold. The test runs to August 2028, though, and three things in the dossier work against it. Capex is guided at about $25bn net of incentives in the first half of FY2027 alone and higher after. Cash taxes of $1.25bn against a $14.8bn provision will catch up. Receivables rose $25.2bn. So FY2028 needs operating cash flow of roughly twice FY2026's capex, and that probably needs operating income near C2's line. That makes C3 at least as hard as C2. R5 points the same way: in 2017-2025 operating cash flow less capex was only $15.9bn, and spending follows price. A downturn would release working capital and capex can be cut, as in 2023, which keeps this near even. Contested at 0.45. (weighed R5) `prep:evidence.2.value_now` `prep:evidence.2.test_threshold_base` `prep:evidence.2.kill_threshold_base` `facts:derived.ttm.capex` `facts:valuation.cases.base.path.0.fcff` `dossier:figures.63.value` `dossier:financial_quality.earnings_quality` `dossier:expectations.case_comments` `redteam:objections.4.statement` |

## Effective base case (computed in code)

Total 61.65; base-case 5-year return 7.5%; no deviation claim Supported, so the code's base case stands.

| Line | Price |
|---|---|

No price zone: the high case's year-5 value is 3.6x the base case's (over 2.5x), so the zone depends on which case holds. Base weight 0.0% of the stock sleeve (track B).

## Red flags

- Flag 0: **unresolved**. The flag says earnings and margins are at a shortage peak and price-driven. Its only rebuttal claim, C2, is Contested, not Supported, so the flag stands. The evidence says FY2026 is not the trailing peak, since the November quarter is guided higher. It does not show that the shortage price will survive the supply arriving in 2027-28. `dossier:red_flags.0` `prep:red_flags.0.rebuttal_claims` `prep:evidence.1.value_now`

## Macro conditions

- M1: holds today.
- M2: holds today.

## Mispricing

Does not hold. The market view's facts check out. The price implies 17.22% growth a year on the code's fade, and EV is 7.45 times TTM EBIT. But the claim that the market is wrong rests on C1, which I put at 0.45, with C2 and C3 Contested too. On the effective base case the price of $690 is only 5.3% under the DCF value of $728.75, for 7.46% a year. Pricing a margin collapse is what the market did correctly in 2018 and 2022, when low trailing multiples came before falls in earnings. The new contracts are real but cover a minority of revenue. So the evidence does not show a mispricing.

## Independence and recomputation

Red Team: blind (no claims.json at the Red Team's commit); bear verdict caution.

- TTM revenue: recomputed 1.33188e+11 against 1.33188e+11 (gap 0.00%)
- Base-case year-5 value per share: recomputed 988.57 against 988.57 (gap 0.00%)
- Implied 10-year growth: recomputed 0.1722 against 0.1722 (gap 0.00%)

## Kill criteria

- TTM operating margin below 46.28% at two consecutive quarter-ends before the August 2028 quarter's results: the margin would be fading faster than the code's own path and the price-band contracts would not have changed the cycle. (C1)
- TTM operating income below $85bn at two consecutive quarter-ends: FY2026's earnings would have been the peak and the cyclical fall not stopped by the contracts. (C2)
- TTM operating cash flow less capex below $26.49bn, the code's year-1 free cash flow to the firm, at two consecutive quarter-ends: the code's reinvestment charge would be right. (C3)

Next review: 2026-12-18.

## Deviations

- No base_rate_deviation claim is Supported, so the base case is the code's (7.46% a year) and no override is applied.
- judge_prep.json was read as written on 2026-11-07 (run.yaml judge_prep: keep) and not rebuilt today. Its recompute, macro values and price (6 Nov close of $690) are as of then. Logged in runs/2026-11-07-semis/judge/issues.tsv.
- The Red Team was blind (no claims.json at its commit), so no blindness caveat applies.

## Figures

| Figure | Value | Unit | Period | Source |
|---|---|---|---|---|
| TTM operating margin | 74.59 | % | TTM to Aug 2026 | `facts:derived.ttm.operating_margin` |
| C1 test threshold | 50 | % | each quarter-end to Aug 2028 | `prep:evidence.0.test_threshold_base` |
| C1 kill threshold | 46.28 | % | two consecutive quarter-ends | `prep:evidence.0.kill_threshold_base` |
| Operating margin, quarter to 31 Aug 2026 | 80.68 | % | Q4 FY2026 | `facts:financials_quarterly.2026-08-31.operating_margin` |
| Operating margin FY2018 (previous peak) | 49.34 | % | FY2018 | `facts:financials_annual.2018-08-31.operating_margin` |
| Operating margin FY2019 | 31.51 | % | FY2019 | `facts:valuation.inputs.own_margins_10y.2` |
| Operating margin FY2022 | 31.54 | % | FY2022 | `facts:valuation.inputs.own_margins_10y.5` |
| Operating margin FY2023 | -36.97 | % | FY2023 | `facts:financials_annual.2023-08-31.operating_margin` |
| FY2019 margin as a share of FY2018's | 0.6386 | ratio | FY2018-FY2019 | `calc:{valuation.inputs.own_margins_10y.2}/{valuation.inputs.own_margins_10y.1}` |
| August 2026 quarter margin after a 2019-style first downturn year | 51.52 | % | illustrative | `calc:{financials_quarterly.2026-08-31.operating_margin}*{valuation.inputs.own_margins_10y.2}/{valuation.inputs.own_margins_10y.1}` |
| Remaining performance obligations at minimum pricing | 134 | USD bn | 3 Sep 2026 | `dossier:figures.39.value` |
| Share of remaining obligations due within 12 months | 25 | % | 3 Sep 2026 | `dossier:figures.40.value` |
| Customer deposits under strategic agreements | 12.75 | USD bn | FY2026 | `dossier:figures.41.value` |
| Letters of credit backing strategic agreements | 7 | USD bn | 3 Sep 2026 | `dossier:figures.42.value` |
| Strategic agreements, share of revenue through 2030 (over, estimate) | 35 | % | to 2030 | `dossier:figures.179.value` |
| TTM operating income | 99.34 | USD bn | TTM to Aug 2026 | `facts:derived.ttm.operating_income` |
| C2 test threshold | 99.34 | USD bn | each quarter-end to Aug 2028 | `prep:evidence.1.test_threshold_base` |
| C2 kill threshold | 85 | USD bn | two consecutive quarter-ends | `prep:evidence.1.kill_threshold_base` |
| Operating income, quarter to 30 Nov 2025 | 6.136 | USD bn | Q1 FY2026 | `facts:financials_quarterly.2025-11-30.operating_income` |
| Operating income, quarter to 31 Aug 2026 | 43.75 | USD bn | Q4 FY2026 | `facts:financials_quarterly.2026-08-31.operating_income` |
| Consensus revenue, November 2026 quarter | 61.74 | USD bn | Q1 FY2027 | `facts:estimates.trend.2026-11-30.revenueEstimateAvg` |
| Consensus revenue FY2027 | 275.5 | USD bn | FY2027 | `facts:estimates.trend.2027-08-31.revenueEstimateAvg` |
| Consensus revenue FY2028 | 319.7 | USD bn | FY2028 | `facts:estimates.trend.2028-08-31.revenueEstimateAvg` |
| Fall in trailing EBIT, May 2022 to Feb 2023 | -81.05 | % | 3 quarters | `calc:{derived.ev_ebit_history.quarters.2023-02-28.ttm_ebit}/{derived.ev_ebit_history.quarters.2022-05-31.ttm_ebit}-1` |
| TTM operating cash flow less capex | 58.96 | USD bn | TTM to Aug 2026 | `calc:{derived.ttm.ocf}-{derived.ttm.capex}` |
| C3 test threshold | 52.99 | USD bn | each quarter-end to Aug 2028 | `prep:evidence.2.test_threshold_base` |
| C3 kill threshold | 26.49 | USD bn | two consecutive quarter-ends | `prep:evidence.2.kill_threshold_base` |
| TTM capex | 30.71 | USD bn | TTM to Aug 2026 | `facts:derived.ttm.capex` |
| Capex guidance, first half FY2027 (net of incentives) | 25 | USD bn | H1 FY2027 | `dossier:figures.63.value` |
| Base case free cash flow to the firm, year 1 | 26.5 | USD bn | year 1 | `facts:valuation.cases.base.path.0.fcff` |
| ROIC FY2026 | 110.5 | % | FY2026 | `prep:sound_business.roic_latest` |
| Discount rate | 9.37 | % | valuation | `prep:sound_business.discount_rate` |
| Base case implied 5-year annual return, DCF exit | 7.46 | % | 5y | `facts:valuation.cases.base.implied_return_5y` |
| Valuation price (6 Nov 2026 close) | 690 | USD | 6 Nov 2026 | `facts:valuation.inputs.price_trading` |
| Base case DCF value per share | 728.8 | per share | valuation | `facts:valuation.cases.base.dcf_value_per_share_trading` |
| Price against the base case DCF value | -5.32 | % | 6 Nov 2026 | `calc:{valuation.inputs.price_trading}/{valuation.cases.base.dcf_value_per_share_trading}-1` |
| Implied 10-year revenue growth (Track B) | 17.22 | % | 10y | `facts:valuation.expectations.implied_growth_10y` |
| EV/EBIT at the valuation price on TTM operating income | 7.45 | x | TTM | `calc:{valuation.inputs.enterprise_value}/{derived.ttm.operating_income}` |
| US 10-year yield (M1, threshold 5.5) | 4.867 | % | as of judge_prep | `prep:macro.0.value_today` |
| CMDI investment grade (M2, threshold 0.5) | 0.25 | points | as of judge_prep | `prep:macro.1.value_today` |
