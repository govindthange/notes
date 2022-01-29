# Analysis & Strategies

## Buy Low Sell High

`v1.0`

| If your view is   | but definitely NOT | then to profit | how?       | when?     | with     |
|-------------------|--------------------|----------------|------------|-----------|----------|
| bullish today     | in future          | buy            | @ discount | today     | Short PE |
| bullish in future | today              | buy            | @ discount | in future | Long CE  |
| bearish today     | in future          | sell           | @ premium  | today     | Short CE |
| bearish in future | today              | sell           | @ premium  | in future | Long PE  |

`v2.0`

| If your view is | when?     | but definitely NOT | when      | then to profit | how?       | when?     | with     |
|-----------------|-----------|--------------------|-----------|----------------|------------|-----------|----------|
| bullish         | today     | bullish            | in future | buy shares     | @ discount | today     | SHORT PE |
| bullish         | in future | bullish            | today     | buy shares     | @ discount | in future | LONG CE  |
| bearish         | today     | bearish            | in future | sell shares    | @ premium  | today     | SHORT CE |
| bearish         | in future | bearish            | today     | sell shares    | @ premium  | in future | LONG PE  |


`v3.0`

| If your view is | when?     | i.e. the market will          | but definitely NOT | when?     | then to profit | how?       | when?     | with     |
|-----------------|-----------|-------------------------------|--------------------|-----------|----------------|------------|-----------|----------|
| NOT bearish     | today     | be sideways to little bullish | bullish            | in future | buy shares     | @ discount | today     | SHORT PE |
| bullish         | in future | start trending up             | bullish            | today     | buy shares     | @ discount | in future | LONG CE  |
| NOT bullish     | today     | be sideways to little bearish | bearish            | in future | sell shares    | @ premium  | today     | SHORT CE |
| bearish         | in future | start trending down           | bearish            | today     | sell shares    | @ premium  | in future | LONG PE  |

# Rules

[[Trading Commandments]]

- Be conservative and keep the position size down. It is the most important thing!
	- Keeping the size down is the only defence you have against the bad trades. Size is where Genius fails.
	- There are only 2 kind of trades viz: `Good Trades` and `Bad Trades`.
	- You need not worry about Good Trades.
	- With Bad Trades, if you have the buying power, and you give your self a little time and manage those then you only have Good Trades.
- Make sure you enter 45 day contract. [...](https://youtu.be/Cm2gkiT5bV8?t=765)
- Take profits at around 50%.
- See where the IV is.
- Never close your position unless you do atleast rolls. Give your positoin a little time.

# Guidelines

## Small Account Traders
[...](https://www.youtube.com/watch?v=HaoM4nqxYhU)

- If you have a small account `avoid trading naked options`.
- If you have a small account `avoid trading directional trades`.
- If you have a small account `keep the variety of strategies to a minimum`.

# Tools
1. [Option Opstra](https://opstra.definedge.com/options-simulator)
2. Option Oracle
3. Sensibull

# The Tasty Trade Strategies
[...](https://youtu.be/T6uA_XHunRc?t=86)

## Short Strangle or Naked Strangle
[...](https://youtu.be/T6uA_XHunRc?t=118)

> Simultaneous sale of an OTM put and OTM call.

- You pick this strategy for smaller underlyings. For larger underlyings you choose Iron Condor.
- It has high probability of success (70% to 90%).

### Playbook

- Pick a high IV ranking stock with high liquidity.
- Choose 30 delta strangle. [...](https://youtu.be/T6uA_XHunRc?t=411)
	- A 40Δ strangle gives over 40% chances of being whipsawed.
	- A 30Δ strangle gives only 8% chances of being whipsawed. You collect less premium.
	- A 20Δ strangle 1% chance of whipsaw. You collect even lesser premium.
	- A 10Δ strangle < 1% chance of whipsaw.
- Management mechanics:
	- Exit at 50% of the credit received or 21 DTE.
- Defence mechanics:
	- Roll the untested side when the strike is breached or delta becomes too big.
		- If the stocks is going higher, roll up the puts.
		- If the stock is going lower, roll down the calls.
	- Roll the position out in time.
		- 21 DTE hasn't come up yet, we take the position from the the front month (current) and move it to the back month (next). You may do it for the same strike.
		- This gives you more credit, more time, higher probability of success, and does not use any more buying power.
	- Go inverted.
		- The stock goes too low. Your put is being tested. You move your call below your put.
		- The stock goes too high. Your call is being tested. you move your put over your call.
		- This reduces your delta. Look to reduce your delta by 25% to 50% whenever you do any adjustments.

### Trade

Naked Strangle Trade:
	=> (1 x `Short PE @ OTM`) + (1 x `Short CE @ OTM`)
	=> (1 x `35 DTE`  `30Δ`  `Short PE @ Support`) + (1 x `35 DTE`  `30Δ`   `Short CE @ Resistance`)

- Use `20Δ` strangles if you want to be less aggressive.
- Use volatility pops to gauge how aggressive you want to get.

### Trade Adjustment

- Don't make the mistake of not re-eststablishing the position in the last 5-10 days to expiration.
	- The mistake of not rolling out that delta when you go into the last 5-10 DTE and re-establishing the position out in another 30 days.
- One approach when position moves against you is to not do anything until you reach the breakeven point i.e. when the price attempts to test one side of the strangle.
- Another approach, even when breakeven isn't breached, is to wait for your original 20 δ to go over 30 δ or 35 δ.
- For adjustment you would rollup the untested side of the position if.
- Exit upon 5 to 10 DTE or 50% of the max profit.

[[Short Strangle]]

## Iron Condors
[...](https://youtu.be/T6uA_XHunRc?t=458)

> Simulatenou sale of an OTM put spread and OTM call spread.

- You basically take a short strangle and define risk by buying CE and PE around it.
- You pick this strategy for larger underlyings. For smaller underlyings you choose short strangle.
- It has 70% to 90% probability of success (same as strangle).
- You make far less compared to a short strangle.
- You use a lot less buying power.
- You have a limited risk.

### Trade

Iron Condor Trade:
	=> (1 x `Short Strangle`) + (2 x `Long Wings`)
OR  => (1 x `Short Call Spread`) + (1 x `Short Put Spread`)
	=> (`35 DTE`  `25Δ`  `Short PE @ Support` + `Long PE @ OTM`) + (`35 DTE`  `25Δ`  `Short CE @ Resistance` + `Long CE @ OTM`)

## Credit Spread
[...](https://youtu.be/T6uA_XHunRc?t=549)

- Its a directional strategy and like any directional strategy you have 50% chances.
- If you short at 30Δ strike you will have 70% chance of winning.
- Management mechanics:
	- Exit at 50% of the credit received or 21 DTE.
- Defence mechanics:
	- No defence.
	- Limited risk.

## Ratio Spread
[...](https://youtu.be/T6uA_XHunRc?t=631)

- It has high probability of success (80% to 90%).
- Volaitity should be not very low or not very high.
- Where to place our short strikes?
	- If stocks moved lower in a 45-day period, they moved an average of -4.5% and landed around the 25Δ PE strike.
	- If stocks moved higher ina 45-day period, they moved an average of +3.7% and landed around the 30Δ CE strike.
	- Use regular monthly options as they are the most liquid.
- Management mechanics:
	- 30% of max profit.
- Defence mechanics:
	- Close spread.
	- Roll out in time 1 of the short options.
	- Turn it into a strangle w/o any extra buying power.

### Trade

Ratio Spread Trade:
	=> (1 x `Long Call Spread`) + (1 x `Short Call`)
OR  => (1 x `Long CE @ ATM`) + (2 x `Short CE @ OTM`)
	=> (1 x `35 DTE`  `40Δ`  `Long CE @ ATM`) + (2 x `35 DTE`  `30Δ`   `Short CE @ OTM`)

## Naked Options

If you short an option that is 1σ away from the spot price, it has 84% probability of finishing OTM.

### Trade

Short Put Trade:
	=> (1 x `Short PE @ OTM`)
	=> (1 x `35 DTE`  `35Δ`  `Short PE @ OTM`)

Short Call Trade:
	=> (1 x `Short CE @ OTM`)
	=> (1 x `35 DTE`  `35Δ`  `Short CE @ OTM`)

## Broken Wing Butterfly (BWB)
[...](https://youtu.be/T6uA_XHunRc?t=832) | [...](https://www.youtube.com/watch?v=sjCWOmn4OgA) | [...](https://www.youtube.com/watch?v=ZCcs2CgY-mI) | [...](https://www.youtube.com/watch?v=r5GvQgbChJQ)

> Simultaneous purchase of a long butterfly combined with a short credit spread.

- It has 70% to 80% probability of success.
- Management mechanics:
	- 25% of max profit.
- Defence mechanics:
	- Generally no defence since limited risk.

## Diagonal Spread
[...](https://youtu.be/T6uA_XHunRc?t=941)

> Simultaneous purchase of a long calendar combined with a vertical spread.

- It is the least popular strategies.
- It has 50% to 60% probability of success.
- Management mechanics:
	- 25% to 50% of max profit.
- Defence mechanics:
	- Roll forward the near month.

## Reverse Jade Lizard

### Trade

Jade Lizard Trade:
	=> (1 x `Short Put Spread`) + (1 x `Short Call`)
OR  => (1 x `Short Strangle`) + (1 x `Long PE @ OTM`)
	=> (1 x `35 DTE`  `30Δ`  `Short OTM Strangle`) + (1 x `35 DTE`  `Long PE @ OTM`)

# Catalog

[[Option Strategy Catalog]]

# Popular Strategies

## Short Put
[...](https://www.youtube.com/watch?v=RMRWlwcKmJA)

If you short a put 1σ below the spot price, it has 84% probability of finishing OTM! ^cd7311

## Poor Man's Covered Call

## Covered Strangle

## [[Vertical Spread]]

## [[Iron Fly]]

# Comparisons

Covered Call = Short CE + Long Stocks

## Strangles vs Iron Condors
https://www.youtube.com/watch?v=D0I-VXz3FcI

Iron Condor = Strangle + Hedges

## Iron Butterfly vs Regular Butterfly Spread
[...](https://www.youtube.com/watch?v=gQIIcktL5I8)

### Iron Butterfly

- Uses combinations of CEs and PEs
- Uses OTM
- Credit Strategy

### Regular Butterfly Spread

- Uses just CEs (or just PEs)
- Uses ATM & ITM
- Debit Strategy

### Similarities

- Both strategies are very similar in terms of Risk Profile and Risk to Reward Ratios.
- If the stock is very liquid then it doesn't matter which of the 2 strategies you use.

### Differences

If the stock is illiquid and [[Trade#Bid-Ask Spread]] is wide the `Bid-Ask` becomes even more wider for `ITM` options. In such cases use `Iron Butterfly` over `Regular Butterfly Spread` as Iron Butterfly Strategy uses `OTM` options as its component.