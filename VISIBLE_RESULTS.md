# eBay — decision evidence and visible results

**WATCH / DEFER. Provisional scenario range; material evidence gaps prevent initiation.**

Valuation: 2026-09-16 close. USD millions except per-share values. Five rolling years ending September 16, 2027–2031; these are not corporate fiscal years.
Information cutoff: September 16; sources retrieved October 19. No later operating evidence is used. Latest balance sheet is June 30; the September opening is a disclosed synthetic bridge, not a reported balance sheet.

Conditional DCF range: **31–81 USD/share**; base 53.17. Market quote: 109.17 on September 16. Rounded endpoints are presentation, not confidence bounds.
Price-only entry gate: <= 24.46 (20% below low case), AND verified bridge/PPA, intact thesis, and analyst adoption of assumptions. The price gate alone never authorizes initiation.

## Cases and named stresses
| Case | GMV growth path | EV | Equity | USD/share | PV terminal / EV | Status |
| --- | --- | --- | --- | --- | --- | --- |
| Low | 0.0%, 1.0%, 2.0%, 2.0%, 2.0% | 17,548.28 | 13,913.68 | 30.58 | 64.0% | provisional |
| Base | 4.0%, 4.0%, 3.5%, 3.0%, 3.0% | 27,825.10 | 24,190.50 | 53.17 | 70.6% | provisional |
| High | 8.0%, 7.0%, 6.0%, 5.0%, 4.0% | 40,286.81 | 36,652.22 | 80.55 | 75.4% | provisional |
| Flat GMV / no more monetization | 0.0%, 0.0%, 0.0%, 0.0%, 0.0% | 23,938.39 | 20,303.79 | 44.62 | 68.8% | provisional |
| Service cost and fraud squeeze | 4.0%, 4.0%, 3.5%, 3.0%, 3.0% | 19,607.87 | 15,973.27 | 35.11 | 71.3% | provisional |
| Depop integration failure | 4.0%, 4.0%, 3.5%, 3.0%, 3.0% | 26,877.74 | 23,243.14 | 51.08 | 70.7% | provisional |
| Severe marketplace contraction | -15.0%, -10.0%, -5.0%, 0.0%, 0.0% | 6,133.16 | 2,498.57 | 5.49 | 64.9% | provisional |

## Decision-changing downside
Flat GMV and service-cost pressures lower the admissible entry value. Persistent severe contraction or failure to fund losses changes WATCH/DEFER to DO NOT INITIATE until an explicit recovery/funding case is supported. No negative cash flow is clipped.
## WACC
| Component | Value |
| --- | --- |
| market_equity | 48,580.65 |
| debt | 6,735.00 |
| equity_weight | 87.8244% |
| cost_equity | 10.0100% |
| pretax_cost_debt | 6.0100% |
| wacc | 9.3766% |

Risk-free 5.01% is sourced; beta 1.0 and ERP 5% are judgments. New debt cost 6.01% is risk-free plus a judgment 100 bp spread, not the old 5.125% bond coupon presented as market yield. Debt weights use carrying value as market-value proxy.
## EV-to-equity bridge
| Adjustment | USD millions |
| --- | --- |
| cash_less_required_reserve | -97.65 |
| liquid_investments | 2,541.00 |
| equity_investments_after_haircut | 657.05 |
| debt | -6,735.00 |
| other_claims | 0.00 |
| Proxy diluted shares, millions | 455.00 |

Cash less reserve can be negative: the model deducts any reserve shortfall rather than ignoring required funding. Customer funds are excluded. Investment income is outside operating profit; investments are added once. Operating leases remain operating costs; no second lease-debt deduction.
## Terminal convention
| Component | Value |
| --- | --- |
| terminal_roic | 0.15 |
| terminal_nopat | 2,537.18 |
| terminal_reinvestment | 422.86 |
| terminal_fcff | 2,114.32 |
| pv_explicit | 8,183.72 |
| terminal_value | 30,746.43 |
| pv_terminal | 19,641.39 |

End-year discounting. Terminal NOPAT grows at g; reinvestment = NOPAT × g/ROIC. The terminal ROIC is an explicit judgment, not the final-year PP&E ratio. This avoids perpetuating transitional D&A/capex distortions.
## WACC / growth sensitivity, USD/share
| WACC | g 1.5% | g 2.5% | g 3.5% |
| --- | --- | --- | --- |
| 8.377% | 58.83 | 63.38 | 69.70 |
| 9.377% | 50.30 | 53.17 | 56.92 |
| 10.377% | 43.70 | 45.54 | 47.84 |

## Reverse DCF
{
  "status": "solved",
  "constant_annual_gmv_growth": 0.2007587312720716,
  "check_price": 109.16999999778305,
  "target": 109.17,
  "held_fixed": "Base ad/market yields, costs, Depop, WACC, terminal growth/ROIC, bridge and shares."
}

Solved variable is a constant five-year legacy GMV growth rate; base monetization and all other assumptions remain fixed. This is one conditional explanation of the market price, not a forecast.
## Comparable-company diagnostics
| Metric | Value |
| --- | --- |
| method | H1-2026 annualized continuing earnings; common market equity / net income |
| peer_count | 1.00 |
| peer | ETSY (qualified) |
| etsy_market_equity | 6,742.29 |
| etsy_adjusted_cash | 2,682.95 |
| etsy_debt_including_finance_leases | 3,082.21 |
| etsy_ev | 7,141.54 |
| etsy_pe | 15.39 |
| etsy_ev_ebit | 14.57 |
| etsy_ev_sales | 2.75 |
| ebay_pe | 22.83 |
| ebay_ev | 51,099.30 |
| ebay_legacy_ev_cost_allocation | 49,699.30 |
| ebay_legacy_ev_ebit_cost_allocation | 19.31 |
| ebay_ev_ebit_unallocated | 19.85 |
| ebay_ev_sales_unallocated | 4.11 |
| pe_anchor | 71.99 |
| ev_ebit_anchor | 77.50 |
| warning | Single-peer diagnostics, not fair-value bounds. EBAY observed EV includes Depop while historical operating denominators do not; unallocated ratios are NOT directly comparable. Applied EV anchor uses a separately disclosed Depop COST proxy. P/E anchor is historical-earnings diagnostic with post-acquisition scope mismatch. Costs/capitalization and unreported bridge changes remain qualified. |

The historical Lab 8 P/E band used 2025 total EPS and Depop/Reverb scope; the new diagnostic uses H1-2026 continuing earnings annualized for both firms. Neither is a probability interval.
DCF versus multiples: a current market earnings multiple embeds different growth, capital returns, and risk expectations; it does not establish sustainable cash conversion. Etsy cost capitalization, convertibles, DST benefit and post-sale cash make direct transfer weak. Use these anchors to challenge the DCF, not average them into its range.
## Material evidence still needed
See ../../DATA_QUALITY_AND_MISSING_DATA.md. Most consequential: September net cash/share changes, Depop closing cash/PPA and recurring losses, validated market beta/spread or a defended discount-rate judgment, and your review of scenarios.

## Human review and monitoring
Quarterly: verify comparable GMV, separate ad yield, service/fraud costs, operating cash conversion and Depop losses. Two quarters of nonpositive FX-neutral GMV with falling ad yield, or inability to fund losses without forced dilution, triggers renewed underwriting and a DO NOT INITIATE thesis assessment. Initiation requires a new verified bridge, price below the conditional gate and evidence that the downside remains fundable. Thresholds are proposed analyst judgments, not company guidance.

## Low — linked annual statements

Cause: Marketplace volume stalls, ad yield saturates, service costs rise, Depop fails to scale profitably.

### Income statement
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| marketplace_revenue | 10,002.81 | 10,102.84 | 10,304.89 | 10,510.99 | 10,721.21 |
| advertising_revenue | 2,354.00 | 2,377.54 | 2,425.09 | 2,473.59 | 2,523.06 |
| depop_revenue | 285.92 | 300.22 | 315.23 | 330.99 | 347.54 |
| revenue | 12,642.73 | 12,780.60 | 13,045.21 | 13,315.58 | 13,591.82 |
| legacy_cogs | 3,429.93 | 3,464.23 | 3,533.52 | 3,604.19 | 3,676.27 |
| sales | 2,782.15 | 2,809.97 | 2,866.17 | 2,923.49 | 2,981.96 |
| product | 1,854.61 | 1,873.16 | 1,910.62 | 1,948.84 | 1,987.81 |
| ga | 1,421.74 | 1,435.96 | 1,464.67 | 1,493.97 | 1,523.85 |
| transaction_losses | 599.90 | 605.90 | 618.02 | 630.38 | 642.98 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| depop_operating_cost | 357.40 | 360.26 | 362.51 | 364.09 | 364.92 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| ebit | 2,147.45 | 2,181.57 | 2,240.16 | 2,301.08 | 2,364.48 |
| interest | 336.75 | 336.75 | 336.75 | 336.75 | 336.75 |
| pretax | 1,810.70 | 1,844.82 | 1,903.41 | 1,964.33 | 2,027.73 |
| tax | 362.14 | 368.96 | 380.68 | 392.87 | 405.55 |
| net_income | 1,448.56 | 1,475.86 | 1,522.72 | 1,571.46 | 1,622.18 |

### Balance sheet
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| cash | 1,626.02 | 2,431.67 | 3,317.74 | 4,277.25 | 5,304.93 |
| investments | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 |
| customer_receivable | 1,589.00 | 1,604.89 | 1,636.99 | 1,669.73 | 1,703.12 |
| ppe | 1,555.11 | 1,723.48 | 1,857.03 | 1,965.83 | 2,057.12 |
| goodwill | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 |
| acquired_intangibles | 247.90 | 220.36 | 192.81 | 165.27 | 137.72 |
| other_assets | 4,941.00 | 4,920.38 | 4,901.02 | 4,881.73 | 4,862.49 |
| assets | 18,769.82 | 19,711.56 | 20,716.39 | 21,770.59 | 22,876.17 |
| debt | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 |
| revolver | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| customer_payable | 1,589.00 | 1,604.89 | 1,636.99 | 1,669.73 | 1,703.12 |
| other_liabilities | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 |
| liabilities | 13,344.20 | 13,360.09 | 13,392.19 | 13,424.93 | 13,458.33 |
| equity | 5,425.61 | 6,351.47 | 7,324.19 | 8,345.66 | 9,417.84 |

### Cash flow and FCFF
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| net_income | 1,448.56 | 1,475.86 | 1,522.72 | 1,571.46 | 1,622.18 |
| depreciation | 374.13 | 437.49 | 484.85 | 522.42 | 553.03 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| working_capital | -0.76 | 1.38 | 2.65 | 2.70 | 2.76 |
| customer_asset_cf | 0.00 | -15.89 | -32.10 | -32.74 | -33.39 |
| customer_liability_cf | 0.00 | 15.89 | 32.10 | 32.74 | 33.39 |
| cfo | 1,873.00 | 1,961.51 | 2,054.48 | 2,140.73 | 2,222.00 |
| cfi | -599.33 | -605.86 | -618.41 | -631.22 | -644.32 |
| repayment | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| distributions | 550.00 | 550.00 | 550.00 | 550.00 | 550.00 |
| revolver_cf | -0.00 | -0.00 | -0.00 | -0.00 | -0.00 |
| cff | -550.00 | -550.00 | -550.00 | -550.00 | -550.00 |
| cash | 1,626.02 | 2,431.67 | 3,317.74 | 4,277.25 | 5,304.93 |
| nopat | 1,717.96 | 1,745.26 | 1,792.12 | 1,840.86 | 1,891.58 |
| fcff | 1,543.07 | 1,625.05 | 1,705.47 | 1,778.91 | 1,847.08 |

Accounting checks: balance sheet, cash, equity, PP&E, acquired intangibles, debt, customer funds and FCFF financing exclusion all passed at 0.000001 million absolute tolerance.

## Base — linked annual statements

Cause: GMV normalizes from recent acceleration; limited ad monetization; stable costs; gradual Depop breakeven.

### Income statement
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| marketplace_revenue | 10,495.68 | 10,915.51 | 11,297.55 | 11,636.48 | 11,985.57 |
| advertising_revenue | 2,475.99 | 2,594.32 | 2,695.11 | 2,775.96 | 2,859.24 |
| depop_revenue | 326.77 | 375.78 | 413.36 | 446.43 | 473.22 |
| revenue | 13,298.43 | 13,885.61 | 14,406.02 | 14,858.86 | 15,318.02 |
| legacy_cogs | 3,406.03 | 3,547.33 | 3,674.11 | 3,784.34 | 3,897.87 |
| sales | 2,855.73 | 2,974.20 | 3,080.50 | 3,172.91 | 3,268.10 |
| product | 1,946.90 | 2,027.67 | 2,100.14 | 2,163.14 | 2,228.03 |
| ga | 1,492.48 | 1,554.40 | 1,609.95 | 1,658.25 | 1,708.00 |
| transaction_losses | 564.89 | 588.33 | 609.35 | 627.63 | 646.46 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| depop_operating_cost | 375.78 | 394.57 | 413.36 | 424.11 | 425.89 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| ebit | 2,607.08 | 2,749.56 | 2,869.06 | 2,978.94 | 3,094.12 |
| interest | 336.75 | 336.75 | 336.75 | 336.75 | 336.75 |
| pretax | 2,270.33 | 2,412.81 | 2,532.31 | 2,642.19 | 2,757.37 |
| tax | 454.07 | 482.56 | 506.46 | 528.44 | 551.47 |
| net_income | 1,816.27 | 1,930.25 | 2,025.85 | 2,113.75 | 2,205.90 |

### Balance sheet
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| cash | 1,956.09 | 3,168.00 | 4,511.14 | 5,971.21 | 7,543.43 |
| investments | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 |
| customer_receivable | 1,652.56 | 1,718.66 | 1,778.82 | 1,832.18 | 1,887.15 |
| ppe | 1,586.19 | 1,798.20 | 1,975.24 | 2,123.95 | 2,252.58 |
| goodwill | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 |
| acquired_intangibles | 247.90 | 220.36 | 192.81 | 165.27 | 137.72 |
| other_assets | 4,947.56 | 4,931.43 | 4,914.63 | 4,897.16 | 4,879.75 |
| assets | 19,201.08 | 20,647.43 | 22,183.43 | 23,800.55 | 25,511.41 |
| debt | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 |
| revolver | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| customer_payable | 1,652.56 | 1,718.66 | 1,778.82 | 1,832.18 | 1,887.15 |
| other_liabilities | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 |
| liabilities | 13,407.76 | 13,473.87 | 13,534.02 | 13,587.39 | 13,642.35 |
| equity | 5,793.32 | 7,173.57 | 8,649.41 | 10,213.16 | 11,869.06 |

### Cash flow and FCFF
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| net_income | 1,816.27 | 1,930.25 | 2,025.85 | 2,113.75 | 2,205.90 |
| depreciation | 374.13 | 446.23 | 505.87 | 555.68 | 597.51 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| working_capital | 5.80 | 5.87 | 5.20 | 4.53 | 4.59 |
| customer_asset_cf | -63.56 | -66.10 | -60.15 | -53.36 | -54.97 |
| customer_liability_cf | 63.56 | 66.10 | 60.15 | 53.36 | 54.97 |
| cfo | 2,234.15 | 2,420.15 | 2,576.06 | 2,714.45 | 2,848.36 |
| cfi | -630.41 | -658.24 | -682.91 | -704.38 | -726.15 |
| repayment | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| distributions | 550.00 | 550.00 | 550.00 | 550.00 | 550.00 |
| revolver_cf | -0.00 | -0.00 | -0.00 | -0.00 | -0.00 |
| cff | -550.00 | -550.00 | -550.00 | -550.00 | -550.00 |
| cash | 1,956.09 | 3,168.00 | 4,511.14 | 5,971.21 | 7,543.43 |
| nopat | 2,085.67 | 2,199.65 | 2,295.25 | 2,383.15 | 2,475.30 |
| fcff | 1,873.14 | 2,031.31 | 2,162.55 | 2,279.47 | 2,391.62 |

Accounting checks: balance sheet, cash, equity, PP&E, acquired intangibles, debt, customer funds and FCFF financing exclusion all passed at 0.000001 million absolute tolerance.

## High — linked annual statements

Cause: Focus categories sustain volume; ads monetize without seller churn; cost leverage; successful Depop integration.

### Income statement
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| marketplace_revenue | 10,899.36 | 11,662.32 | 12,362.05 | 12,980.16 | 13,499.36 |
| advertising_revenue | 2,590.48 | 2,813.04 | 3,014.60 | 3,188.27 | 3,327.74 |
| depop_revenue | 354.00 | 442.50 | 531.00 | 610.65 | 671.71 |
| revenue | 13,843.84 | 14,917.86 | 15,907.65 | 16,779.08 | 17,498.81 |
| legacy_cogs | 3,407.19 | 3,656.10 | 3,883.75 | 4,083.73 | 4,250.09 |
| sales | 2,902.35 | 3,114.39 | 3,308.30 | 3,478.66 | 3,620.37 |
| product | 2,024.67 | 2,172.58 | 2,307.86 | 2,426.69 | 2,525.55 |
| ga | 1,552.10 | 1,665.49 | 1,769.19 | 1,860.29 | 1,936.08 |
| transaction_losses | 546.99 | 586.95 | 623.49 | 655.60 | 682.31 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| depop_operating_cost | 371.70 | 442.50 | 477.90 | 519.05 | 537.37 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| ebit | 2,989.30 | 3,230.30 | 3,487.61 | 3,705.51 | 3,897.50 |
| interest | 336.75 | 336.75 | 336.75 | 336.75 | 336.75 |
| pretax | 2,652.55 | 2,893.55 | 3,150.86 | 3,368.76 | 3,560.75 |
| tax | 530.51 | 578.71 | 630.17 | 673.75 | 712.15 |
| net_income | 2,122.04 | 2,314.84 | 2,520.69 | 2,695.01 | 2,848.60 |

### Balance sheet
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| cash | 2,230.55 | 3,780.52 | 5,561.63 | 7,541.41 | 9,700.16 |
| investments | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 |
| customer_receivable | 1,716.12 | 1,836.25 | 1,946.42 | 2,043.74 | 2,125.49 |
| ppe | 1,612.05 | 1,865.72 | 2,094.95 | 2,301.00 | 2,483.21 |
| goodwill | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 |
| acquired_intangibles | 247.90 | 220.36 | 192.81 | 165.27 | 137.72 |
| other_assets | 4,953.01 | 4,941.75 | 4,929.65 | 4,916.36 | 4,901.56 |
| assets | 19,570.41 | 21,455.38 | 23,536.25 | 25,778.58 | 28,158.93 |
| debt | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 |
| revolver | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| customer_payable | 1,716.12 | 1,836.25 | 1,946.42 | 2,043.74 | 2,125.49 |
| other_liabilities | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 |
| liabilities | 13,471.33 | 13,591.45 | 13,701.63 | 13,798.95 | 13,880.70 |
| equity | 6,099.09 | 7,863.93 | 9,834.62 | 11,979.63 | 14,278.23 |

### Cash flow and FCFF
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| net_income | 2,122.04 | 2,314.84 | 2,520.69 | 2,695.01 | 2,848.60 |
| depreciation | 374.13 | 453.50 | 524.87 | 589.36 | 647.32 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| working_capital | 11.26 | 10.74 | 9.90 | 8.71 | 7.20 |
| customer_asset_cf | -127.12 | -120.13 | -110.17 | -97.32 | -81.75 |
| customer_liability_cf | 127.12 | 120.13 | 110.17 | 97.32 | 81.75 |
| cfo | 2,534.46 | 2,807.15 | 3,085.21 | 3,325.20 | 3,538.27 |
| cfi | -656.26 | -707.18 | -754.10 | -795.41 | -829.53 |
| repayment | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| distributions | 550.00 | 550.00 | 550.00 | 550.00 | 550.00 |
| revolver_cf | -0.00 | -0.00 | -0.00 | -0.00 | -0.00 |
| cff | -550.00 | -550.00 | -550.00 | -550.00 | -550.00 |
| cash | 2,230.55 | 3,780.52 | 5,561.63 | 7,541.41 | 9,700.16 |
| nopat | 2,391.44 | 2,584.24 | 2,790.09 | 2,964.41 | 3,118.00 |
| fcff | 2,147.60 | 2,369.37 | 2,600.51 | 2,799.19 | 2,978.14 |

Accounting checks: balance sheet, cash, equity, PP&E, acquired intangibles, debt, customer funds and FCFF financing exclusion all passed at 0.000001 million absolute tolerance.

## Flat GMV / no more monetization — linked annual statements

Cause: GMV normalizes from recent acceleration; limited ad monetization; stable costs; gradual Depop breakeven.

### Income statement
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| marketplace_revenue | 10,092.00 | 10,092.00 | 10,092.00 | 10,092.00 | 10,092.00 |
| advertising_revenue | 2,354.00 | 2,354.00 | 2,354.00 | 2,354.00 | 2,354.00 |
| depop_revenue | 326.77 | 375.78 | 413.36 | 446.43 | 473.22 |
| revenue | 12,772.77 | 12,821.78 | 12,859.36 | 12,892.43 | 12,919.22 |
| legacy_cogs | 3,268.00 | 3,268.00 | 3,268.00 | 3,268.00 | 3,268.00 |
| sales | 2,740.00 | 2,740.00 | 2,740.00 | 2,740.00 | 2,740.00 |
| product | 1,868.00 | 1,868.00 | 1,868.00 | 1,868.00 | 1,868.00 |
| ga | 1,432.00 | 1,432.00 | 1,432.00 | 1,432.00 | 1,432.00 |
| transaction_losses | 542.00 | 542.00 | 542.00 | 542.00 | 542.00 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| depop_operating_cost | 375.78 | 394.57 | 413.36 | 424.11 | 425.89 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| ebit | 2,497.44 | 2,527.67 | 2,546.46 | 2,568.78 | 2,593.78 |
| interest | 336.75 | 336.75 | 336.75 | 336.75 | 336.75 |
| pretax | 2,160.69 | 2,190.92 | 2,209.71 | 2,232.03 | 2,257.03 |
| tax | 432.14 | 438.18 | 441.94 | 446.41 | 451.41 |
| net_income | 1,728.55 | 1,752.73 | 1,767.76 | 1,785.62 | 1,805.62 |

### Balance sheet
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| cash | 1,898.55 | 2,981.74 | 4,125.73 | 5,320.64 | 6,559.64 |
| investments | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 |
| customer_receivable | 1,589.00 | 1,589.00 | 1,589.00 | 1,589.00 | 1,589.00 |
| ppe | 1,561.27 | 1,729.87 | 1,852.81 | 1,942.74 | 2,008.64 |
| goodwill | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 |
| acquired_intangibles | 247.90 | 220.36 | 192.81 | 165.27 | 137.72 |
| other_assets | 4,942.30 | 4,920.79 | 4,899.16 | 4,877.50 | 4,855.76 |
| assets | 19,049.81 | 20,252.54 | 21,470.30 | 22,705.93 | 23,961.55 |
| debt | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 |
| revolver | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| customer_payable | 1,589.00 | 1,589.00 | 1,589.00 | 1,589.00 | 1,589.00 |
| other_liabilities | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 |
| liabilities | 13,344.20 | 13,344.20 | 13,344.20 | 13,344.20 | 13,344.20 |
| equity | 5,705.60 | 6,908.34 | 8,126.10 | 9,361.72 | 10,617.34 |

### Cash flow and FCFF
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| net_income | 1,728.55 | 1,752.73 | 1,767.76 | 1,785.62 | 1,805.62 |
| depreciation | 374.13 | 439.22 | 486.65 | 521.24 | 546.53 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| working_capital | 0.54 | 0.49 | 0.38 | 0.33 | 0.27 |
| customer_asset_cf | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| customer_liability_cf | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| cfo | 2,151.69 | 2,241.01 | 2,303.58 | 2,356.07 | 2,401.43 |
| cfi | -605.49 | -607.81 | -609.60 | -611.16 | -612.43 |
| repayment | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| distributions | 550.00 | 550.00 | 550.00 | 550.00 | 550.00 |
| revolver_cf | -0.00 | -0.00 | -0.00 | -0.00 | -0.00 |
| cff | -550.00 | -550.00 | -550.00 | -550.00 | -550.00 |
| cash | 1,898.55 | 2,981.74 | 4,125.73 | 5,320.64 | 6,559.64 |
| nopat | 1,997.95 | 2,022.13 | 2,037.16 | 2,055.02 | 2,075.02 |
| fcff | 1,815.60 | 1,902.59 | 1,963.39 | 2,014.31 | 2,058.40 |

Accounting checks: balance sheet, cash, equity, PP&E, acquired intangibles, debt, customer funds and FCFF financing exclusion all passed at 0.000001 million absolute tolerance.

## Service cost and fraud squeeze — linked annual statements

Cause: GMV normalizes from recent acceleration; limited ad monetization; stable costs; gradual Depop breakeven.

### Income statement
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| marketplace_revenue | 10,495.68 | 10,915.51 | 11,297.55 | 11,636.48 | 11,985.57 |
| advertising_revenue | 2,475.99 | 2,594.32 | 2,695.11 | 2,775.96 | 2,859.24 |
| depop_revenue | 326.77 | 375.78 | 413.36 | 446.43 | 473.22 |
| revenue | 13,298.43 | 13,885.61 | 14,406.02 | 14,858.86 | 15,318.02 |
| legacy_cogs | 3,924.89 | 4,087.73 | 4,233.82 | 4,360.83 | 4,491.66 |
| sales | 2,855.73 | 2,974.20 | 3,080.50 | 3,172.91 | 3,268.10 |
| product | 1,946.90 | 2,027.67 | 2,100.14 | 2,163.14 | 2,228.03 |
| ga | 1,492.48 | 1,554.40 | 1,609.95 | 1,658.25 | 1,708.00 |
| transaction_losses | 824.33 | 858.52 | 889.21 | 915.88 | 943.36 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| depop_operating_cost | 375.78 | 394.57 | 413.36 | 424.11 | 425.89 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| ebit | 1,828.78 | 1,938.97 | 2,029.50 | 2,114.19 | 2,203.43 |
| interest | 336.75 | 336.75 | 336.75 | 336.75 | 336.75 |
| pretax | 1,492.03 | 1,602.22 | 1,692.75 | 1,777.44 | 1,866.68 |
| tax | 298.41 | 320.44 | 338.55 | 355.49 | 373.34 |
| net_income | 1,193.63 | 1,281.78 | 1,354.20 | 1,421.95 | 1,493.35 |

### Balance sheet
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| cash | 1,333.45 | 1,896.88 | 2,568.38 | 3,336.65 | 4,196.32 |
| investments | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 |
| customer_receivable | 1,652.56 | 1,718.66 | 1,778.82 | 1,832.18 | 1,887.15 |
| ppe | 1,586.19 | 1,798.20 | 1,975.24 | 2,123.95 | 2,252.58 |
| goodwill | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 |
| acquired_intangibles | 247.90 | 220.36 | 192.81 | 165.27 | 137.72 |
| other_assets | 4,947.56 | 4,931.43 | 4,914.63 | 4,897.16 | 4,879.75 |
| assets | 18,578.44 | 19,376.32 | 20,240.67 | 21,165.99 | 22,164.30 |
| debt | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 |
| revolver | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| customer_payable | 1,652.56 | 1,718.66 | 1,778.82 | 1,832.18 | 1,887.15 |
| other_liabilities | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 |
| liabilities | 13,407.76 | 13,473.87 | 13,534.02 | 13,587.39 | 13,642.35 |
| equity | 5,170.68 | 5,902.45 | 6,706.65 | 7,578.61 | 8,521.95 |

### Cash flow and FCFF
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| net_income | 1,193.63 | 1,281.78 | 1,354.20 | 1,421.95 | 1,493.35 |
| depreciation | 374.13 | 446.23 | 505.87 | 555.68 | 597.51 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| working_capital | 5.80 | 5.87 | 5.20 | 4.53 | 4.59 |
| customer_asset_cf | -63.56 | -66.10 | -60.15 | -53.36 | -54.97 |
| customer_liability_cf | 63.56 | 66.10 | 60.15 | 53.36 | 54.97 |
| cfo | 1,611.51 | 1,771.68 | 1,904.41 | 2,022.65 | 2,135.81 |
| cfi | -630.41 | -658.24 | -682.91 | -704.38 | -726.15 |
| repayment | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| distributions | 550.00 | 550.00 | 550.00 | 550.00 | 550.00 |
| revolver_cf | -0.00 | -0.00 | -0.00 | -0.00 | -0.00 |
| cff | -550.00 | -550.00 | -550.00 | -550.00 | -550.00 |
| cash | 1,333.45 | 1,896.88 | 2,568.38 | 3,336.65 | 4,196.32 |
| nopat | 1,463.03 | 1,551.18 | 1,623.60 | 1,691.35 | 1,762.75 |
| fcff | 1,250.50 | 1,382.84 | 1,490.90 | 1,587.67 | 1,679.07 |

Accounting checks: balance sheet, cash, equity, PP&E, acquired intangibles, debt, customer funds and FCFF financing exclusion all passed at 0.000001 million absolute tolerance.

## Depop integration failure — linked annual statements

Cause: GMV normalizes from recent acceleration; limited ad monetization; stable costs; gradual Depop breakeven.

### Income statement
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| marketplace_revenue | 10,495.68 | 10,915.51 | 11,297.55 | 11,636.48 | 11,985.57 |
| advertising_revenue | 2,475.99 | 2,594.32 | 2,695.11 | 2,775.96 | 2,859.24 |
| depop_revenue | 272.31 | 272.31 | 272.31 | 272.31 | 272.31 |
| revenue | 13,243.97 | 13,782.13 | 14,264.96 | 14,684.74 | 15,117.11 |
| legacy_cogs | 3,406.03 | 3,547.33 | 3,674.11 | 3,784.34 | 3,897.87 |
| sales | 2,855.73 | 2,974.20 | 3,080.50 | 3,172.91 | 3,268.10 |
| product | 1,946.90 | 2,027.67 | 2,100.14 | 2,163.14 | 2,228.03 |
| ga | 1,492.48 | 1,554.40 | 1,609.95 | 1,658.25 | 1,708.00 |
| transaction_losses | 564.89 | 588.33 | 609.35 | 627.63 | 646.46 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| depop_operating_cost | 408.46 | 408.46 | 381.23 | 354.00 | 326.77 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| ebit | 2,519.95 | 2,632.20 | 2,760.14 | 2,874.92 | 2,992.34 |
| interest | 336.75 | 336.75 | 336.75 | 336.75 | 336.75 |
| pretax | 2,183.20 | 2,295.45 | 2,423.39 | 2,538.17 | 2,655.59 |
| tax | 436.64 | 459.09 | 484.68 | 507.63 | 531.12 |
| net_income | 1,746.56 | 1,836.36 | 1,938.71 | 2,030.54 | 2,124.47 |

### Balance sheet
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| cash | 1,889.50 | 3,012.19 | 4,273.36 | 5,655.55 | 7,151.48 |
| investments | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 |
| customer_receivable | 1,652.56 | 1,718.66 | 1,778.82 | 1,832.18 | 1,887.15 |
| ppe | 1,583.61 | 1,791.44 | 1,963.70 | 2,107.39 | 2,231.16 |
| goodwill | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 |
| acquired_intangibles | 247.90 | 220.36 | 192.81 | 165.27 | 137.72 |
| other_assets | 4,947.01 | 4,930.39 | 4,913.22 | 4,895.42 | 4,877.74 |
| assets | 19,131.37 | 20,483.83 | 21,932.69 | 23,466.60 | 25,096.04 |
| debt | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 |
| revolver | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| customer_payable | 1,652.56 | 1,718.66 | 1,778.82 | 1,832.18 | 1,887.15 |
| other_liabilities | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 |
| liabilities | 13,407.76 | 13,473.87 | 13,534.02 | 13,587.39 | 13,642.35 |
| equity | 5,723.61 | 7,009.96 | 8,398.67 | 9,879.21 | 11,453.69 |

### Cash flow and FCFF
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| net_income | 1,746.56 | 1,836.36 | 1,938.71 | 2,030.54 | 2,124.47 |
| depreciation | 374.13 | 445.50 | 503.97 | 552.43 | 592.86 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| working_capital | 5.26 | 5.38 | 4.83 | 4.20 | 4.32 |
| customer_asset_cf | -63.56 | -66.10 | -60.15 | -53.36 | -54.97 |
| customer_liability_cf | 63.56 | 66.10 | 60.15 | 53.36 | 54.97 |
| cfo | 2,164.98 | 2,326.02 | 2,487.40 | 2,628.32 | 2,762.55 |
| cfi | -627.83 | -653.34 | -676.23 | -696.13 | -716.62 |
| repayment | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| distributions | 550.00 | 550.00 | 550.00 | 550.00 | 550.00 |
| revolver_cf | -0.00 | -0.00 | -0.00 | -0.00 | -0.00 |
| cff | -550.00 | -550.00 | -550.00 | -550.00 | -550.00 |
| cash | 1,889.50 | 3,012.19 | 4,273.36 | 5,655.55 | 7,151.48 |
| nopat | 2,015.96 | 2,105.76 | 2,208.11 | 2,299.94 | 2,393.87 |
| fcff | 1,806.55 | 1,942.09 | 2,080.57 | 2,201.59 | 2,315.33 |

Accounting checks: balance sheet, cash, equity, PP&E, acquired intangibles, debt, customer funds and FCFF financing exclusion all passed at 0.000001 million absolute tolerance.

## Severe marketplace contraction — linked annual statements

Cause: GMV normalizes from recent acceleration; limited ad monetization; stable costs; gradual Depop breakeven.

### Income statement
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| marketplace_revenue | 8,578.20 | 7,720.38 | 7,334.36 | 7,334.36 | 7,334.36 |
| advertising_revenue | 2,023.64 | 1,834.93 | 1,749.66 | 1,749.66 | 1,749.66 |
| depop_revenue | 326.77 | 375.78 | 413.36 | 446.43 | 473.22 |
| revenue | 10,928.61 | 9,931.09 | 9,497.38 | 9,530.45 | 9,557.24 |
| legacy_cogs | 3,843.96 | 3,464.51 | 3,293.63 | 3,293.63 | 3,293.63 |
| sales | 2,334.01 | 2,103.61 | 1,999.86 | 1,999.86 | 1,999.86 |
| product | 1,591.21 | 1,434.14 | 1,363.41 | 1,363.41 | 1,363.41 |
| ga | 1,219.82 | 1,099.41 | 1,045.18 | 1,045.18 | 1,045.18 |
| transaction_losses | 779.75 | 702.77 | 668.11 | 668.11 | 668.11 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| depop_operating_cost | 375.78 | 394.57 | 413.36 | 424.11 | 425.89 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| ebit | 734.54 | 682.53 | 664.29 | 686.61 | 711.61 |
| interest | 336.75 | 365.16 | 385.66 | 406.17 | 426.62 |
| pretax | 397.79 | 317.37 | 278.63 | 280.44 | 284.99 |
| tax | 79.56 | 63.47 | 55.73 | 56.09 | 57.00 |
| net_income | 318.24 | 253.90 | 222.91 | 224.35 | 227.99 |

### Balance sheet
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| cash | 1,000.00 | 1,000.00 | 1,000.00 | 1,000.00 | 1,000.00 |
| investments | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 | 3,314.00 |
| customer_receivable | 1,350.65 | 1,215.58 | 1,154.81 | 1,154.81 | 1,154.81 |
| ppe | 1,473.85 | 1,530.00 | 1,549.80 | 1,565.60 | 1,578.22 |
| goodwill | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 | 5,496.79 |
| acquired_intangibles | 247.90 | 220.36 | 192.81 | 165.27 | 137.72 |
| other_assets | 4,923.86 | 4,891.88 | 4,865.54 | 4,843.88 | 4,822.14 |
| assets | 17,807.05 | 17,668.61 | 17,573.75 | 17,540.33 | 17,503.68 |
| debt | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 | 6,735.00 |
| revolver | 405.90 | 698.64 | 991.65 | 1,283.88 | 1,569.24 |
| customer_payable | 1,350.65 | 1,215.58 | 1,154.81 | 1,154.81 | 1,154.81 |
| other_liabilities | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 | 5,020.20 |
| liabilities | 13,511.76 | 13,669.43 | 13,901.66 | 14,193.89 | 14,479.25 |
| equity | 4,295.29 | 3,999.18 | 3,672.09 | 3,346.44 | 3,024.43 |

### Cash flow and FCFF
| Line | 2027 | 2028 | 2029 | 2030 | 2031 |
| --- | --- | --- | --- | --- | --- |
| net_income | 318.24 | 253.90 | 222.91 | 224.35 | 227.99 |
| depreciation | 374.13 | 414.63 | 430.42 | 435.99 | 440.44 |
| legacy_amortization | 22.00 | 22.00 | 22.00 | 22.00 | 22.00 |
| acquired_amortization | 27.54 | 27.54 | 27.54 | 27.54 | 27.54 |
| working_capital | -17.90 | -9.98 | -4.34 | 0.33 | 0.27 |
| customer_asset_cf | 238.35 | 135.07 | 60.78 | -0.00 | -0.00 |
| customer_liability_cf | -238.35 | -135.07 | -60.78 | 0.00 | 0.00 |
| cfo | 759.81 | 728.04 | 707.21 | 709.56 | 717.70 |
| cfi | -518.07 | -470.78 | -450.22 | -451.79 | -453.06 |
| repayment | 0.00 | 0.00 | 0.00 | 0.00 | 0.00 |
| distributions | 550.00 | 550.00 | 550.00 | 550.00 | 550.00 |
| revolver_cf | 405.90 | 292.74 | 293.01 | 292.23 | 285.36 |
| cff | -144.10 | -257.26 | -256.99 | -257.77 | -264.64 |
| cash | 1,000.00 | 1,000.00 | 1,000.00 | 1,000.00 | 1,000.00 |
| nopat | 587.64 | 546.03 | 531.43 | 549.29 | 569.29 |
| fcff | 511.14 | 549.39 | 565.51 | 582.71 | 605.94 |

Accounting checks: balance sheet, cash, equity, PP&E, acquired intangibles, debt, customer funds and FCFF financing exclusion all passed at 0.000001 million absolute tolerance.

## Automated validation
| Test | Status | Detail |
| --- | --- | --- |
| Filing and accounting-basis reconciliation | PASS | {'FY2025 reported income': 0, 'FY2025 CFO reconciliation': 0, 'FY2025 cash definition reconciliation': 0, 'FY2025 full cash flow tie': 0, 'FY2025 reported balance': 0, '2025 recast PP&E': 0, '2025 recast assets': 0, '2025 recast liabilities': 0, '2025 recast equity': 0, 'June assets': 0, 'June liabilities': 0, 'June balance': 0, 'H1 revenue components': 0, 'H1 EBIT filing tie': 0} |
| Five-year statements articulate | PASS | True |
| Synthetic closed-form known answer using actual DCF kernel | PASS | {'expected': 1000.0, 'actual': 999.9999999999997, 'units': 'synthetic currency units', 'limitation': 'Synthetic independent known answer; published weekly starter answer key still needed.'} |
| Legacy training answer reproduced through final discount kernel | PASS | {'expected_from_lab_notes': 27.4974, 'actual': 27.49737039819684, 'status': 'Reproduces supplied lab-note training answer; instructor answer-key authentication pending.'} |
| WACC/g monotonicity with positive terminal economics | PASS | {'wacc_lower_price': 63.379689902889204, 'base_price': 53.16594423347071, 'wacc_higher_price': 45.53511609032838, 'g_low': 50.30333446236393, 'g_high': 56.92393929896758} |
| Reject WACC <= terminal growth | PASS | Invalid WACC/growth/ROIC boundary |
| Reject terminal ROIC <= growth | PASS | Invalid WACC/growth/ROIC boundary |
| Highest-risk: typed cash must stop valuation | PASS | 2027 asset sum: actual=19201.082571075043, expected=19301.082571075043, gap=-100.0 |
| Broken CFO link refuses | PASS | 2027 cash: actual=1053.7362185666477, expected=1063.7362185666477, gap=-10.0 |
| NaN input refuses | PASS | inputs.assumptions.beta: invalid finite numeric input |
| Liquidity exhaustion refuses | PASS | 2027 liquidity failure: revolver exhausted |
| FCFF excludes financing; no double debt subtraction | PASS | Distributions/paydown alter cash/debt, not operating FCFF or opening EV bridge. |
| Negative FCFF retained; no invented recovery | PASS | {'signed_present_value': -10989.543102581994, 'incorrect_clipped_value': 0.0, 'terminal_rejection': 'Nonpositive terminal operating profit: explicit recovery required'} |
| Peer/multiple definition arithmetic | PASS | Common-equity numerator; continuing H1 denominators; debt not added to P/E. |
| Reverse DCF reprices target | PASS | {'status': 'solved', 'constant_annual_gmv_growth': 0.2007587312720716, 'check_price': 109.16999999778305, 'target': 109.17, 'held_fixed': 'Base ad/market yields, costs, Depop, WACC, terminal growth/ROIC, bridge and shares.'} |

These are AI-assisted software/source checks. They do not establish a human AI-off precommit, a published weekly training-key reconciliation, a partner review, or a recorded student cold run.
## Material input ledger
| ID | Value | Units | Period | Source/locator | Label |
| --- | --- | --- | --- | --- | --- |
| fy25_revenue | 11,100.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_gross | 7,931.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_sales | 2,394.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_ga | 1,198.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_product | 1,642.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_losses | 396.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_amort | 24.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_ebit | 2,277.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_net | 2,031.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_cfo | 2,009.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_da | 407.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_capex | 525.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_assets | 17,610.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_liabilities | 12,995.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_equity | 4,615.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_ppe | 1,338.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_legal | 61.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| fy25_transitions | 91.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Consolidated IS/BS/CF pp.61–66 and MD&A p.44 | fact |
| cash | 2,310.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| short_investments | 997.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| long_investments | 2,317.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| customer_receivable | 1,589.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| other_current_assets | 1,107.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| ppe | 1,301.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| goodwill | 4,471.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| rou | 394.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| dta | 2,929.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| other_assets | 518.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| short_debt | 1,593.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| ap | 353.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| customer_payable | 1,589.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| accrued | 2,334.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| tax_payable | 23.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| lease_liabilities | 278.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| dtl | 1,446.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| long_debt | 5,142.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| other_liabilities | 510.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| equity | 4,665.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| assets | 17,933.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| liabilities | 13,268.00 | USD millions | 2026-06-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Balance sheet p.6 | fact |
| h1_revenue | 6,223.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| h1_market | 5,046.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| h1_ads | 1,177.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| h1_gmv | 44,595.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| h1_cogs | 1,634.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| h1_sales | 1,370.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| h1_product | 934.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| h1_ga | 716.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| h1_losses | 271.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| h1_amort | 11.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| h1_ebit | 1,287.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| h1_net_cont | 1,064.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| h1_da | 194.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| h1_capex | 295.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| equity_investments | 773.00 | USD millions | H1 2026 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) IS p.7; CF p.10; Notes 4/5; MD&A metrics | fact |
| recast_ppe | 1,165.00 | USD millions | 2025-12-31 adjusted basis | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Note 1 ASU 2025-06 retrospective adoption | fact |
| ppe_reduction | 173.00 | USD millions | 2025-12-31 adjusted basis | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Note 1 ASU 2025-06 retrospective adoption | fact |
| dtl_reduction | 41.00 | USD millions | 2025-12-31 adjusted basis | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Note 1 ASU 2025-06 retrospective adoption | fact |
| equity_reduction | 132.00 | USD millions | 2025-12-31 adjusted basis | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Note 1 ASU 2025-06 retrospective adoption | fact |
| recast_assets | 17,437.00 | USD millions | 2025-12-31 adjusted basis | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Note 1 ASU 2025-06 retrospective adoption | fact |
| recast_liabilities | 12,954.00 | USD millions | 2025-12-31 adjusted basis | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Note 1 ASU 2025-06 retrospective adoption | fact |
| recast_equity | 4,483.00 | USD millions | 2025-12-31 adjusted basis | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Note 1 ASU 2025-06 retrospective adoption | fact |
| basic_shares | 445.00 | million shares | 2026-07-31 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Cover page; Note 2 Q2 dilutive effect | fact |
| award_increment | 10.00 | million shares | 2026-07-31 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Cover page; Note 2 Q2 dilutive effect | fact |
| depop_paid | 1,400.00 | USD millions | 2026-07-30 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Note 3 goodwill/acquisition and MD&A | fact |
| dividend_per_share | 0.31 | USD/share | 2026-09-11 | [Q26](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000177/ebay-20260630.htm) Note 11 declared dividend, $0.31 paid September 11 | fact |
| depop_h1_revenue | 136.15 | USD millions | H1 2026 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Note 2 Depop discontinued operations, thousands /1000 | fact |
| depop_h1_ebit | -196.61 | USD millions | H1 2026 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Note 2 Depop discontinued operations, thousands /1000 | fact |
| depop_cash | 130.30 | USD millions | 2026-06-30 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Note 2 Depop assets/liabilities, thousands /1000 | fact |
| depop_other_current | 15.08 | USD millions | 2026-06-30 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Note 2 Depop assets/liabilities, thousands /1000 | fact |
| depop_ppe | 28.92 | USD millions | 2026-06-30 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Note 2 Depop assets/liabilities, thousands /1000 | fact |
| depop_intangibles | 275.45 | USD millions | 2026-06-30 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Note 2 Depop assets/liabilities, thousands /1000 | fact |
| depop_other_assets | 0.67 | USD millions | 2026-06-30 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Note 2 Depop assets/liabilities, thousands /1000 | fact |
| depop_assets | 450.42 | USD millions | 2026-06-30 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Note 2 Depop assets/liabilities, thousands /1000 | fact |
| depop_liabilities | 76.20 | USD millions | 2026-06-30 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Note 2 Depop assets/liabilities, thousands /1000 | fact |
| etsy_h1_revenue | 1,299.59 | USD millions | H1 2026 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Continuing IS, thousands /1000 | fact |
| etsy_h1_ebit | 245.11 | USD millions | H1 2026 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Continuing IS, thousands /1000 | fact |
| etsy_h1_net | 219.00 | USD millions | H1 2026 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Continuing IS, thousands /1000 | fact |
| etsy_cash | 901.28 | USD millions | 2026-06-30 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Continuing BS; Note 9; thousands /1000 | fact |
| etsy_st_investments | 221.01 | USD millions | 2026-06-30 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Continuing BS; Note 9; thousands /1000 | fact |
| etsy_lt_investments | 160.66 | USD millions | 2026-06-30 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Continuing BS; Note 9; thousands /1000 | fact |
| etsy_debt | 2,985.51 | USD millions | 2026-06-30 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Continuing BS; Note 9; thousands /1000 | fact |
| etsy_finance_lease_noncurrent | 90.30 | USD millions | 2026-06-30 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Continuing BS; Note 9; thousands /1000 | fact |
| etsy_shares | 91.78 | million shares | 2026-07-31 | [ET26](https://investors.etsy.com/sec-filings/all-sec-filings/content/0001370637-26-000080/etsy-20260630.htm) Cover common shares, shares /1e6 | fact |
| market_price | 109.17 | USD/share | 2026-09-16 | [PRICE_EB](https://www.quiverquant.com/stock/EBAY/historical-prices/) Regular-session Close; corroborated Investing.com/Yahoo | fact |
| etsy_price | 73.46 | USD/share | 2026-09-16 | [PRICE_ET](https://stockanalysis.com/stocks/etsy/history/) Regular-session Close; corroborated Investing.com/Yahoo | fact |
| risk_free | 0.05 | decimal annual rate | 2026-09-16 | [RF](https://home.treasury.gov/resource-center/data-chart-center/interest-rates/TextView?field_tdr_date_value=2026&type=daily_treasury_yield_curve) 10-year column; independent FRED corroboration | fact |
| fy25_cf_discontinued_adjustment | -35.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_sbc | 607.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_cf_investment_adjustment | -17.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_cf_deferred_tax | 44.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_cf_warrant | 5.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_cf_other_current | -153.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_cf_other_noncurrent | 48.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_cf_ap | -4.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_cf_accrued | -335.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_cf_tax | -985.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_corporate_cash | 1,867.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_customer_cash | 1,017.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_restricted_cash | 171.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_total_cash | 3,055.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_begin_cash | 3,286.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_discontinued_cfo | -50.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_cfi | 1,420.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_cff | -3,661.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
| fy25_fx | 51.00 | USD millions | FY2025 original basis | [K25](https://www.sec.gov/Archives/edgar/data/1065088/000106508826000027/ebay-20251231.htm) Cash flow statement pp.65–66 and cash-definition reconciliation; MD&A cash | fact |
