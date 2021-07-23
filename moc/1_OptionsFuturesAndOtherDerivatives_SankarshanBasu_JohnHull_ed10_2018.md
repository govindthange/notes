1_OptionsFuturesAndOtherDerivatives_SankarshanBasu_JohnHull_ed10_2018.pdf

# Derivative Market (1-2, 8)

## How derivative market works? (1-2)

## What are different ways of transferring risks? (8)
- Forward Contract
- Futures Contract
- Option Contract
- Swap
- ==Securiization (8)==

### 2007 Credit Crisis (8)

## What are various price adjustments important in derivative market? (9)

Derivatives are valued using following XVAs:

- Credit Valuation Adjustment (CVA)
- Debit Valuation Adjustment (DVA)
- Funding Valuation Adjustment (FVA)
- Margin Valuation Adjustment (MVA)
- Capital Valuation Adjustment (KVA)

---

# Interest Rates (4)

# Forward Contract (5)

# Futures Contract (3, 6)

## Hedging (3)

## Types (6)

```mermaid
graph LR;
	s(Stocks)
	c(Commodities)
	i(Indices)
	f(Foreign Currencies)
	ir(4. Interest Rates)
	ir-->ir_tb(6. Treasury Bonds)
	ir-->ir_ed(6. Eurodollar Futures)
```


# Swaps (7)

# Vanilla Option Contract for Financial Assets (10-24,27,30)

## Various Types & Inner Workings (10-18,21,27,30)

```mermaid
graph LR;
	so(10. Spot Options)
	subgraph " "
		so-->so_me(10. Mechanics)
		so-->so_p(11. Properties)
		so-->so_s(12. Strategies)
		so-->so_v(Valuation)
		so_v-->sov_ad(Valuing American Derivatives)
			sov_ad-->sov_wtm(w/ Models)
				sov_wtm-->sovwtm_bt(13. Binomial Trees)
				sov_wtm-->sovwtm_pp(14. Various Pricing Processes)
					sovwtm_pp-->sovwtm_wp(Wiener Processes)
					sovwtm_pp-->sovwtm_mcs(Montel Carlo Simulation)
				sov_wtm-->sovwtm_bsm(15. Black-Scholes-Merton)
			sov_ad-->sov_wom(w/o Models)
				sov_wom-->sovwom_bnp(21,27. Numerical Procedures)
		so_v-->sov_ed(30. Valuing European-style Derivatives)
			sov_ed-->soved_ca(Convexity Adjustments)
			sov_ed-->soved_ta(Timing Adjustments)
			sov_ed-->soved_q(Quantos)
		so-->so_mo(15. Model)
		so-->so_t(Types)
		so_t-->sot_es(16. Employee Stocks)
		so_t-->sot_i(17. Indices)
		so_t-->sot_c(17. Commodities)
    end
	
	fo(18. Future Options)
	subgraph " "
    end
```

## Risks (19,20,22-24)

```mermaid
graph LR;
	r(Market Risks)
	r-->r_d(19. Different Dimensions)
	r-->r_tr(22. Total Risk)
		r_tr-->rtr_var("Value at Risk (VaR)")
		r_tr-->rtr_es("Expected Shortfall (ES)")
	r-->r_v(20. Volatility)
	r_v-->rv_ev(23. Estimating Volatilities & Correlations)

	r_cr(24. Credit Risks)
```

# Credit Derivatives (25)

```mermaid
graph LR;
	cd(25. Credit Derivatives)
```

# Exotic Option Contract (26)

Exotic Options (aka Exotics) are `Over The Counter (OTC)` derivative product for financial assets.


```mermaid
graph LR;
	cd(26. Exotic Options)
```

# Interest Rate Derivatives (28-29)

### Valuation (28)

# Swaps (34)

# Energy & Commodity Derivatives (35)

# Real Option Contract for Real Assets (36)
Options for real assets like land, buildings, plant and equipiments.