[...](https://www.youtube.com/watch?v=KN4lNB-B2l8)

# Intraday Option Chain

- Option Chain works very well with `Top 10 Nifty 50 Stocks` due to their high liquidity.
- Option Chain data provides lot of insights on the day of expiry (Thursday).
- Option Chain data is not very useful soon after the day of expiry (i.e. Friday). For example data on Friday is not useful so one must wait till Monday or Tuesday and then analyze it.

# Open Interest Analysis

`Open Interest (OI)` is the number of Call (or Put) contracts at a strike.

Usually `Smart Money or Big Institutions` are `Option Sellers`.
- If there is a huge OI at a call strike above then it means someone big is selling calls thinking market won't go above a certin resistance level.
- If there is a huge OI at a put strike below then it means someone big is selling puts thinking market won't go below a certain support level.

A high `Call OI` above current price usually means a `Resistance`. A huge OI in 2 or more close call strikes indicates a `Resistance Zone` around those strikes. So if there is significant `Call OI` around a strike, you can sell calls of that zone.

A high `Put OI` below current price usually means a `Support`. A huge OI in 2 or more close put strikes indicates a `Support Zone` around those strikes. So if there is significant `Put OI` around a strike, you can sell puts of that zone.

> For better results use OI Analysis along with Volume, Price Action, Technical Charts and Indicators.

- Open Interest does not work all the time on all the stocks. Using it incorrectly can land you in lot of trouble.
- The Open Interest (OI) must be a big number like in following cases:
	- Bank Nifty Weekly Options
	- Nifty Weekly Options
	- Nifty Monthly Options near the middle of the month. (Not in the beginning of the month!)
	- Heavily Traded Liquid Stocks.

OI Analysis would not work for the following:
- Far away expiry contracts
- Contracts at the beginning of the expiry month
- Smaller stocks with low market cap.
- Illiquid stocks/options.
- When there are events (like Stock Results) do not rely on Open Interest to base your trades.

- Look for Strike Prices that see more activity.
	- With Bank Nifty almost all the activity happens with Strike Prices that are multiple of 500. So look for Bank Nifty Strike Price with gap of ₹500.
	- Look for Nifty Strike Prices with gap of ₹100.

## Change in OI / Guessing Direction
[...](https://www.youtube.com/watch?v=CEAR2wmznL8)

Change in OI tells market momentum and direction.

Have a `Bullish View` when...
- `Put OI` is increasing at a given strike.
	- Strong support is about to build up at strike.
	- Smart money is gaining confidence in Support at strike below the spot.
- `Call OI` is decreasing at a given strike
	- Smart money is losing confidence in Resistance at strike above the spot.

Have a `Bearish View` when...
- `Put OI` is decreasing at a given strike.
	- Smart money is loosing confidence in Support at strike below the spot.
- `Call OI` is increasing at a given strike
	- Strong resistance is about to build up at strike.
	- Smart money is gaining confidence in Resistance at strike above the spot.

> OI by itself is just a snapshot. You cant tell market direction by looking at just one OI value. To understand where market is going you need to see OI value in relation to its previous value i.e. `Change in OI`.

```
When `Call OI is increasing` at or above current price (resistance level)
=> People are selling `Calls`
=> Market is ==bearish==

When `Call OI is decreasing` at or above current price
=> People are unwinding/getting out of sold `Calls`
=> Market is ==bullish==

When `Put OI is increasing` at or below current price (support level)
=> People are selling `Puts`
=> Market is ==bullish==

When `Put OI is decreasing` at or below current price
=> People are unwinding/getting out of sold `Puts`
=> Market is ==bearish==
```

## Multi-Strike OI Analysis
## Pay-Off Diagram
## Basket Orders

# Put Call Ratio (PCR)

Stick to PCR on the nearest coming expiry.

Very Low PCR (< 0.3) is a Bullish Possibility
- Market is Oversold

Low PCR (< 0.5) is Bearish
- More Calls than Puts
- (Big) Sellers are willing to sell calls, more than puts.
- It means Smart Money / Insitutions are scared of market falling `market won't rise much`.

PCR = 0.7 (approx) is neutral
- Wait and watch!

High PCR (> 1) is Bullish
- More Puts than Calls
- (Big) Sellers are willing to sell puts, more than calls.
- It means Smart Money / Insitutions think `market won't go down much`.

Very High PCR > 1.3 is a Bearish Possibility
- Market is Overbought

# Max Pain

`Max Pain Point` is a point at which the sellers will have least loss.

`Max Pain Theory:` The expiry of the stock will happen at the `Max Pain` point.

Example:

If currently Nifty is @ ₹11883.85 and its `Max Pain` = 11800 then as per `Max Pain Theory` this week's expiry will likely happen at around 11800 (approx) because it is the point at which both `Call` and `Put` sellers will face least amount of losses.

Expiry happening at the strike price causes least damage to the seller. This theory is not scientific; there are loose evidence of this working well.

# ITM Probability

We should consider selling those Strikes that have lowest probability of going ITM.