1_OptionsFuturesAndOtherDerivatives_SankarshanBasu_JohnHull_ed10_2018.pdf

# Derivative Market (1-2, 8)

## How derivative market works? (1-2)

## What are different ways of transferring risks? (8)
- Forward Contract
- Futures Contract
- Option Contract
- Swap
- ==Securitization (8)==

### 2007 Credit Crisis (8)

## What are various price adjustments important in derivative market? (9)

Derivatives are valued using following XVAs:

- Credit Valuation Adjustment (CVA)
- Debit Valuation Adjustment (DVA)
- Funding Valuation Adjustment (FVA)
- Margin Valuation Adjustment (MVA)
- Capital Valuation Adjustment (KVA)

---

# Interest Rates (4, 28-29)

## Interest Rate Derivatives (28-29)

### Valuation (28)

```mermaid
graph LR;
	ts(Term Structure)
		ts-->ts_srm(Short Rate)
			ts_srm-->tssrm_em(31. Equilibrium Model)
				tssrm_em-->tssrmem_1fmm(One-Factor Markov Models)
					tssrmem_1fmm-->tssrmem1fmm_vm(Vasicek Model)
					tssrmem_1fmm-->tssrmem1fmm_c(Cox, Ingersoll & Ross Model)
				tssrm_em-->tssrmem_2fmm(Two-Factor Markov Models)
			ts_srm-->tssrm_nam(32. Non-Arbitrage Model)
		ts-->irrfn_frm(33. Forward Rate)
```

# Forward Contracts (5)

# Futures (3, 6)

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


# Swaps (7, 34)

## LIBOR for Fixed Interest Rates


Vanilla Swaps
Compounding Swaps
Currency Swaps
Equity Swaps

# Options (10-24,26-27,30,36)

These are `vanilla` Option Contracts for Financial Assets
## LIBOR for Fixed Interest Rates
## Various Types & Inner Workings (10-18,20-21,23,26-27,30,36)

```mermaid
graph LR;
	so(10. Spot Options)
	subgraph " "
		so-->so_me(10. Mechanics)
		so-->so_p(11. Properties)
		so-->so_s(12. Strategies)
		so-->so_v(Valuation)
		so_v-.-|of|sov_ad(American-style Derivatives)
			sov_ad-->sov_wtm(w/ Models)
				sov_wtm-->sovwtm_bt(13. Binomial Trees)
				sov_wtm-->sovwtm_pp(14. Various Pricing Processes)
					sovwtm_pp-->sovwtm_wp(Wiener Processes)
					sovwtm_pp-->sovwtm_mcs(Monte Carlo Simulation)
				sov_wtm-->sovwtm_bsm(15. Black-Scholes-Merton)
			sov_ad-->sov_wom(w/o Models)
				sov_wom-->sovwom_bnp(21,27. Numerical Procedures)
			sov_ad-->sovad_v(w/ Volatility)
				sovad_v-->sovadv_vs(20. Volatility Smile)
				sovad_v-->sovadv_ev(23. Estimating Volatilities & Correlations)
		so_v-.-|of|sov_ed(30. European-style Derivatives)
			sov_ed-->soved_ca(Convexity Adjustments)
			sov_ed-->soved_ta(Timing Adjustments)
			sov_ed-->soved_q(Quantos)
		so-->so_t(Types)
		so_t-->sot_es(16. Employee Stocks)
		so_t-->sot_i(17. Indices)
		so_t-->sot_c(17. Commodities)
    end
	
	fo(18. Future Options)
	subgraph " "
    end
	
	eo(26. Exotic Options)
	subgraph " "
    end
	
	ro(36. Real Options)
	subgraph " "
    end
```


> `Exotic Options` (aka Exotics) are `Over The Counter (OTC)` derivative products for financial assets.

> `Real Options` are option contracts for real assets like land, buildings, plant and equipiments.

## Risks (19,20,22,24)

```mermaid
graph LR;
	r(Market Risks)
	r-->r_d(19. Different Dimensions)
	r-->r_tr(22. Total Risk)
		r_tr-->rtr_var("Value at Risk (VaR)")
		r_tr-->rtr_es("Expected Shortfall (ES)")
	r_cr(24. Credit Risks)
```

# Credit Derivatives (25)

```mermaid
graph LR;
	cd(25. Credit Derivatives)
```

# Energy & Commodity Derivatives (35)

---

Pending:
- Chapter 37