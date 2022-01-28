# Step 1. Form a market view

Establish whether you are bullish, bearish, or neutral on the market direction.

> Don't use PoP for forming a market view, PoP is only a mechanical means to select a better strike price.

## Step 1. Choose the underlying
[...](https://www.youtube.com/watch?v=dHUej1FPbQ0)

When considering an underlying to trade, look for the following key statistics:
1. IV
	- IV tells us the expected move.
	- Compare IV to the overall market and correlated products.
2. IV Ranges
	- Look at the current IV relative to its high and low IV over a period of time.
	- Look for underlyings that are trading high in its IV range to possibly play for an IV mean reversion.
3. Liquidity
	- Look to liquid products as these will offer the most efficiently priced options.
	- Liquidity allows to easily trade in and out of positions, and you give up less edge each time you place a trade.
	- High open interest and tight bid/ask spreads are key indications of liquidity.
4. Earnings/Binary Events
	- These events have a significant impact on IV and theta decay.
	- Being aware of these events and their effect on option pricing is critical in our underlying selection.
5. Price weakness or strength
	- As contrarians you buy into weakness and sell into strength.
	- Look to the price action of an underlying to assist in your underlying selection process.
6. Your existing portfolio
7. Overall market conditions

> In our underlying selection process we look for highly liquid, familiar stocks. We turn to absolute IV and IV percentile for potential trades, governed by high PoP and plausible RoC.
>
> Ultimately trades are triggered by our assumptions, be they directional, IV or otherwise.

# Step 2. Evaluate IV assumptions
[...](https://www.youtube.com/watch?v=iD6Z9m4u08A)

Analyze where you are w.r.t Implied Volatility.

IV drives it all...
- Every thing is designed around some mean reversion of IV.
- The driver behind your directional assumption starts with IV levels.
- Use IV levels to drive the underlying assumptions.
	- If a stock is trading at 100 percentile IV then use this fact to assume its either capitulation or complacency.
	- If a stock is trading at 0 percentile IV level
- Then your underlying assumptions then drives the pot odds (i.e. there is more money to make than there is to lose).
- The driver w.r.t pot odds  starts with IV levels.

[[Option Strategy Builder#Step 3 Make mean reversion assumptions]]

# Step 3. Pick a liquid strike price w/ high PoP

## Step 1. Pick a strike price w/ high PoP

PoP, though useful in strike selection, are not the "holly grail".
- If you short a high probability option with a low IV and you do get the directional move you wanted but IV expands then you still  won't be profitable because IV levels were too low at the time of the trade.
- You should be right on your market view and you must be right on your IV assumptions too.
- Your stock selection generally begins with some assumption with regard to IV levels. And its these assumptions that drive the pot odds as to whether your probabilities (PoP) will get better or worse over time.

The underlying assumptions (directional bias) are based on IV levels.

The strategies are based on what your probabilities are of getting to a certain levels.
- Select a strike with highest OTM probability i.e. 2σ away with approximately 84+% Probability of Profit (PoP)
	- Note that this this standard deviation is derived from the IV itself.
	- The PoP percentage are going to be the same but how much distance away from the stock is based of the IV.
- [[Option Strategies#Short Put]]
	- ![[Option Strategies#^cd7311]]

### Nuances

- Don't use PoP to form a market view. The driver behind your directional assumption must start with IV levels.
- Don't use PoP to drive underlying assumptions.
- Don't use PoP to make the decision to make that trade.
- Use PoP to set stratgies.
- Use PoP to select and be mechanical about continuing to choose the right strike price.
- Use PoP to set reasonal expectations for profit or loss so that we can manage our winning trades.
- Use PoP to set reasonal expectations to our timings i.e. how much duration do we have to extend to get to this number which gives us a reasonable chance of making money.

##### Example

Say ABC has been down for many days straight.
- ABC is trading at 100 IV percentile. At that IV levels you can assume that the stock may go up.
- Its now you use PoP to give yourself a realistic expectation of what level you can get to which will ultimately help you to form your strategies.

## Step 2. Pick a strike price w/ high liquidity
[...](https://www.youtube.com/watch?v=j1Tle-kGzhk)

Liquidity is the king in option trading book.

- Stick to Nifty, Bank Nifty and top 15 F&O stock options for trading.
- Prefer regular monthly options as they are the most liquid options.

###  Narrow Bid/Ask Spreads

Look for tighter bid/ask spreads when selecting a strike sprice.

- A large bid-ask spread is usually a sign of illiquid option.
- Stay away from deep OTM/ITM call/put contracts as their spreads are very wide.

### Higher OI

Look for higher OI when selecting a strike sprice.

- Larger the number of open contracts in the market, higher the probability of it being liquid.
- OI on the ATM as well as not-very-far OTMs  are also important for determining the liquidity.
- When we create strategies with various legs, the OI of OTMs also play an important role. We should be able to adjust strategies at later stages of the trade.

### Higher OI Volume

Look for higher OI volume when selecting a strike sprice.

- Open contracts doesn't mean tradeable contracts!
	- If OI is high but volume is not high then that means it is not tradeable. There are not enough participants trading at that strike price.
	- When these OIs have volumes it displays churning in the said strike.
- Low volumes are sign of illiquid options.

# Step 4. Select the strategy
[...](https://www.youtube.com/watch?v=MOxQqT_s-Eg)

Look for strategies that take advantage of the IV premium, while looking to maximize the PoP & RoC.

- IV is a major component of the underlying selection.
	- IV is a primary factor in strategy selection process.
	- Look to where IV sits in its range and then compare it to the overall market.
	- If the market IV is trading at 25% and we select a stock that is trading at a higher IV say 40% or more, we will choose a strategy that looks to take advantage of the volatility premium by shorting it.
- Probability of Profit (PoP) and Return on Capital (RoC) are other factors to consider when picking a strategy.
	- As a general rule place high PoP trades while attempting to maximize RoC.
	- On a weighted average look to have a portfolio PoP of around 65-75%.
	- Don't sell put if RoC is 1.5%

## High IV Strategies

When volatility is high consider following strategies:
- Short Stangle w/ far OTM strikes
- Short Iron Condors w/ far OTM strikes
- Short Verticals / Credit Spreads
- Covered Calls
- Naked Puts w/ lower strikes that are further OTM

## Low IV Strategies

When volatility is low then strategy selection becomes challenging for an option sellers. However, it is important to stay in the game and stay engaged.
- Do this by widening out your strikes and focusing on underlying that maintain a rich IV.
- Protect against a sudden rise in IV. If IV is low look to place trades that won't be negatively affected by a sudden volatility expansion in the market by deploying following strategies:
	- Bearish Directional Trades (i.e., short stocks)
	- Debit Put Spread (ITM/OTM)
		- Pairs Trade (they give you more time)
		- Diagonals (Directional Diagonal)

# Step 5. Deploy the strategy

# Step 6. Manage the position

Poor Management = Over Adjustments

## Step 1. Do not revisit PoP

Do not look at probability after placing a trade.
- Probabilities are what they are when you place the trade they don't stay that way for the duration of the trade.
- PoP is based on the current snapshot of IV the moment it was captured. And, since IV changes and is mean reverting, it does not remain that way during the life of the trade.
- The PoP is a function of volaitility. If volatility changes, PoP changes with it. If IV's move higher, your short premium probabilities get worse.
	- If you enter a trade at a decent IV level then you are betting on the IV contraction.
	- If you enter a trade at a low IV level then you are still betting on the IV contraction but chances are you will get IV expansion.
