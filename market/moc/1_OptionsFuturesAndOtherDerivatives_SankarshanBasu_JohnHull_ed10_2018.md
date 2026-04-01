1_OptionsFuturesAndOtherDerivatives_SankarshanBasu_JohnHull_ed10_2018.pdf

This book's goal:

- Unifying framework for valuation of all types of derivatives.

# Derivatives Market (1-2, 8)

## Derivatives Market and How it is changing (1)

## How it works? (2)

## What are the different ways of transferring risks? (8)
- Forward Contract
- Futures Contract
- Option Contract
- Swap
- ==Securitization (8)==

---

# Interest Rates (4, 28-29,31-33)

## Interest Rate Derivatives (28-29)

### Valuation (28)

## Interest Rate Term Structure (31-33)

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


## LIBOR for Fixed Interest Rates

# Forward Contracts (5)

# Futures (3, 6)

## Hedging Strategies (3)

```mermaid
graph LR;
	f(Futures)
	f-->f_s(Strategies)
		f_s-->fs_h(3. Hedging)
	f-->v(5. Valuation)
	f-->f_t(Types)
	f_t-->ft_s(Stocks)
	f_t-->ft_c(Commodities)
	f_t-->ft_i(Indices)
	f_t-->ft_f(Foreign Currencies)
	f_t-->ft_irf(6. Interest Rate Futures)
		ft_irf-->ftirf_tb(6. Treasury Bonds)
		ft_irf-->ftirf_ed(6. Eurodollar Futures)
```


# Swaps (7, 34)

Vanilla Swaps
Compounding Swaps
Currency Swaps
Equity Swaps

# Options (10-24,26-27,30,36)

These are `vanilla` Option Contracts for Financial Assets

## Various Types & Inner Workings (10-18,20-21,23,26-27,30,36)

```mermaid
graph LR;
	so(10. Spot Options)
	subgraph " "
		so-->so_me(10. Mechanics)
		so-->so_s(12. Strategies)
		so-->so_v(Valuation)
		so_v-.-|in|sov_ad(American-style)
			sov_ad-->sovad_wp(w/ Process)
				sovad_wp-->sovadwp_s(14. Stochastic Process)
					sovadwp_s-.-|based on|sovadwps_s(Sampling)
						sovadwps_s-->sovadwpss_rpo(Random Process Outcomes)
					sovadwp_s-.-|based on|sovadwps_t(Time)
						sovadwps_t-->sovadwpst_d(Discrete)
						sovadwps_t-->sovadwpst_c(Continuous)
							sovadwpst_c-->sovadwpstc_dr(Drift Rate)
							sovadwpst_c-->sovadwpstc_vr(Variance Rate)
					sovadwp_s-.-|based on|sovadwps_v(Variable)
						sovadwps_v-->sovadwpsv_d(Discrete)
						sovadwps_v-->sovadwpsv_c(Continuous)
					sovadwp_s==>sovadwp_mp(Markov Process)
					sovadwp_s==>sovadwp_wp(Wiener Process)
					sovadwp_mp-.->sovadwp_wp
					sovadwp_wp-.-sovadwpst_c
					sovadwp_s==>sovadwp_ip(Itô process)
					sovadwp_wp-.->sovadwp_ip
					sovadwp_ip-.-sovadwpst_c
					sovadwp_s==>sovadwp_mcs(Monte Carlo Simulation)
					sovadwp_mcs-.-sovadwpss_rpo
			sov_ad-->sov_wtm(w/ Models)
				sov_wtm-->sovwtm_gmm("Geometric Motion Model (GMM)")
					sovwtm_gmm-->sovwtmgmm_bsm(15. Black-Scholes-Merton)
					sovwtm_gmm-->sovwtmgmm_bnp(21. Basic Numerical Proedures)
						sovwtmgmm_bnp-->sovwtmgmmbnp_bt(13. Binomial Trees)
				sov_wtm-->sovwtm_gmma(27. Alternatives to GMM)
			sov_ad-->sovad_v(w/ Volatility)
				sovad_v-->sovadv_vs(20. Volatility Smile)
				sovad_v-->sovadv_ev(23. Estimating Volatilities & Correlations)
		so_v-.-|in|sov_ed(30. European-style)
			sov_ed-->soved_ca(Convexity Adjustments)
				soved_ca-->sovedca_ir(Interest Rates)
				soved_ca-->sovedca_sr(Swap Rates)
			sov_ed-->soved_ta(Timing Adjustments)
			sov_ed-->soved_q(Quantos)
				soved_q-->sovedq_nbm(Numeraire-based Measures)
				soved_q-->sovedq_trn(Traditional Risk-Neutral Measures)
		so-->so_t(Types)
		so_t-->sot_so(Stock Options)
			sot_so-->sotso_p(11. Properties)
		so_t-->sot_es(16. Employee Stock Options)
		so_t-->sot_i(17. Indices Options)
		so_t-->sot_c(17. Commodities Options)
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
	r-->r_d("19. Dimensions (Greeks)")
		r_d-->rd_v(Vega)
		r_d-->rd_g(Gamma)
		r_d-->rd_d(Delta)
		r_d-->rd_t(Theta)
		r_d-->rd_vix(VIX/VI)
	r-->r_tr("22. Total Risk (for Banks)")
		r_tr-->rtr_var("Value at Risk (VaR)")
		r_tr-->rtr_es("Expected Shortfall (ES)")
	r_cr(24. Credit Risks)
		r_cr-->rcr_cc2007(8. 2007 Credit Crisis)
		r_cr-->rcr_pa("9. Derivatives Price Adjustments (XVAs)")
			rcr_pa-->rcrpa_cva(CVA)
			rcr_pa-->rcrpa_dva(DVA)
			rcr_pa-->rcrpa_fva(FVA)
			rcr_pa-->rcrpa_mva(MVA)
			rcr_pa-->rcrpa_kva(KVA)
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