Directional heroes generally lose lot of money because the market is in conslidation phase 70% of the time.

Short Strangle is when you have a neutral view of the market and so you sell `OTM Call` and `OTM Put`.
- Extremely risk due to unlimited loss.
- Decent profit but limited.
- Trade management is the key to success in this strategy.

Only use this strategy for `Nifty` and `Bank Nifty` as the indices, although expensive, are likely to absorb volatility better than stocks.
- Nifty is safer.
- Bank Nifty is little riskier.
- Stocks are the most riskiest due to high volatility.

Use `Weekly Expiry` over Monthly Expiry due to following reasons:
- Better % returns
- Adjustment can be made quickly at weekly expiry

Determine the `Strike Price` for OTM Call and OTM Put by using one of the following methods:

1. `Observe Price Action` to find a range.
2. Use `Support & Resistance` to determine the range.
3. Use `Option Chain` to determine the strike price with the highest Open Interest.
	-  The strike price with the highest OI change on the Call side is to be considered as resistance and a Call at that strike price should be shorted.
	-  The strike price with the highest OI change on the Put side is to be considered as support and a Put at that strike price should be shorted.
4. Use a predecided `Delta`.
5. Use a predecided `Strike Price`.


## Managing the Strangle Mechanics

Once you take the position its all about managing the mechanics of the Strangle position. You may have to frequently do so based on the volatility. Generally you would rollup the untested side of the position if the price attempts to test one side of the strangle.
- If the price drops you bring the `Call` down and rollout; i.e. add a new `Call`.
- If the price soars you bring the `Put` down and rollout; i.e. add a new `Put`

## Rules
([Ref.](https://youtu.be/Eqzmq_RkBaY?t=758))

- Be convervative and keep the position size down. It is the most important thing!
	- Keeping the size down is the only defence you have against the bad trades. Size is when Genius fails.
	- There are only 2 kind of trades viz: `Good Trades` and `Bad Trades`.
	- You need not worry about Good Trades.
	- With Bad Trades, if you have the buying power, and you give your self a little time and manage those then you only have Good Trades.
- Ensure that 50% of your buying power is free just so that you can freely roleover and re-adjust your strangle position.
- Take profits at around 50%.
- If there is an Earning Declaration by companies then you skew your strangle position to the upside.
	- These days when earnings are declared, if its good you know the price will shoot to 30% but if its not good, then it may not crash by 30%.
	- So, you can select a `Put` with 15 δ.
	- If the earnings are not great then you can go aggressive on the call side by keeping δ high.
- If there is high volatility create a super wide strangle position.

# Fixed Strike Price Method

1. Pick a fixed strike price like so:
	- For Bank Nifty select `CE @ 115 Rs.` and `PE @ 115 Rs.` premiums with `Take Profit` at Rs. 4,000 level.
	- For Nifty select `CE @ ? 25` and `PE @ ? 25` premiums wiht `Take Profit` at Rs. 3,000 level.

2. Hedge your strangle by buying `Heldge Legs` as follow:
	1. For `Bank Nifty` go `Long` on `CE @ 25 Rs.` and `PE @ 25 Rs.`
	2. For `Nifty` go `Long` on ???

3. Exit when current week's premium falls below 80%.
	- You may exit anywhere between the 75% to 85% range.
	- If the premium does not fall below 80% then exit the current week contract on the thursday morning as soon as market opens.

> Note that if you wait for the premium to become 0 then the profit will go down. There is no point in holding a position beyond a certain time.

```
Example:

You go `Short` on `CE @ 100 Rs.` and `PE @ 100 Rs.` @ `Current Week Expiry`

During the week whenever the premium starts trading close to 20 Points you should exit the trade. It may not be exactly 20. It could be anwhere between 18 to 22.
```

4. Immediately after exiting the position, take entry into the coming week expiry contract.

## Adjusting Position

5 Rules of adjusting the premium.

`Rule 1.` Exit the trade as soon you make Rs 4,000/- in profits in Bank Nifty or Rs 3,000/- in profits in Nifty.

`Rule 2.` Adjust your position only when one side of the premium falls below 50% of the higher trading premium.

`Rule 3.` The premium of the adjusted position has to be between 80% to 95% of the higher side premium.

`Rule 4.` Difference between the `Call` and `Put` premiums should not go below 80% during the market closing hours. When this happens adjust the position by exiting the lower premium Call or Put and Shorting a new Call/Put which is at a price that keeps the difference between 80% to 95% range.

`Rule 5.` Exit the trade when you reach a point where both `Call` and `Put` both are at the same `Strike Price`.

References:
- [The Strategy](https://www.youtube.com/watch?v=_t-vfmCG3Mo)
- [The Backtesting](https://www.youtube.com/watch?v=GCCWnE-Cu7A)

# Δ Method

High Δ value implies:
- High risk due to high probability of ITM.
- High rewards due to high premium.
- Tighter strangle range which means smaller room for price to consolidate.
- Experienced traders can choose 16-20 δ value. 30-35 δ is an aggressive value for advanced traders.
- Requires frequent managing of positions. Generally you would rollup the untested side of the position if the price attempts to test one side of the strangle.

Low Δ value implies:
- Low risk due to low probability of ITM.
- Low rewards due to low premium.
- Wider strangle range so price has more to consolidate and attempt small trends.
- Generally 5 δ is a low delta value good for beginners.
- Position need not be managed frequently.

- [Choosing Delta by Sasha Evdakov](https://www.youtube.com/watch?v=ZPKqHhHyPfs)

> You can start with 5 to 10 delta value and as you master the mechanics of managing strangle then you can graduate to using 20 delta and beyond.

## 5-10 δ Strangle
https://www.youtube.com/watch?v=Eqzmq_RkBaY

If you are beginner choose 5-10 δ value to create strangle.

5 minute trade.

![[Short Strangle#Rules]]

### Adjusting Position

## 16 δ Strangle with 1 SD
https://www.youtube.com/watch?v=AEwaxiliR-M

Experienced traders can choose 16-20 δ value.

### Adjusting Position

## 20-35 δ Strangle
https://www.youtube.com/watch?v=9TEN6Q2BzGc

30-35 δ is an aggressive value for a more advanced traders.

Note that volatility and fear is overstated in the long run (30-45 days).

Usually go with 20 Delta Strangle. You may select 30-35 Delta when you have confidence and feel more aggressive.

You can take 10 to 20 simulataneous positions in `uncorrelated` assets like equity, commodity, bonds etc. and manage them.

Monthly contracts which goes from 30 days to 45 days.

### Adjusting Position

When 20 δ reduces to 10-12 δ then continue holding the position without adjusting.

Adjust when position becomes breakeven by rolling over to the untested side of the position.

### Exiting Position

When 20 δ reduces to 5 δ then exit the position.


