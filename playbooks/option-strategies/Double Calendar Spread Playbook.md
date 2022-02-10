[...](https://www.youtube.com/watch?v=zMwFaIqWYhs)

# Step 1. Wait for setup
[...](https://youtu.be/9JFVkhbOZIw?list=PLOggP3CmSaMDKsajRrNOECS4U94v4xvxc&t=1048)

Wait for a defined event.

- Take advantage of upcoming high volatility.
	- You need current volatility to be low/medium and expect it to go up from here.
	- Calendar based strategies can only benefit during the times of increasing IV.
	- If there is no increase in IV then the long calendar options (the hedges) of next/far expiry will rapidly fall after 2 days.
	- Note that the middle of the payoff chart is always close to 0 line i.e. close to no profit if price doesn't move.
- Deploy calendars based on what might happen in the near future that may cause volatility to go up.
	- Calendar based strategies works best for the upcoming known events.
	- Await news, budget, ellection, announcement, or some result/earning event etc.
	- Your technical analysis or bullish/bearish view has little role to play in calendar strategies.

# Step 2. Define risk

Hedge naked strangle with the credit received from selling a Double DCS.

1. Define risk with 1:1 Risk/Reward ratio.
	- If you receive ₹10,000 in credit, then only debit ₹10,000 for hedging.
	- Its fine to pay slightly extra.
2. Hedge the short position by buying an option with the same lot size.
	- Skip the near expiry (front week/month) i.e. expiry of the option used for strangle and go to the subsequent expiry (AKA next expiry or back week/month expiry).
	- Pick the strike corresponding to the credit received from the sold options.
		- You may pay slightly extra because you will close this position in the near expiry (i.e. front week/month).
		- It is best to pick strike which is atleast ₹10 higher than the credit received.
	- The profit in the middle of the payoff chart should be at least 1.5% of the margin.
	- By buying PE & CE options will increase breakeven range.

# 3. Deploy strategy

- Deploy strategy on Tuesday @ 03:00 PM.
- Exit strategy by Wednesday @ 3:00 PM or by Thursday @ 9:20 AM.
- Exit as soon you see profit. As days pass by, Probability of Profit falls sharply.

## Position Size

1. Look at the blue t+0 line in opstra.
2. Move your cursor over the t+0 line at the lowermost breakeven point.
3. Note down the loss.
4. If this `loss` is ≤ `2% of total trading capital` only then deploy the strategy.
5. If `loss` > `2% of the total trading capital` then skip and wait for the next opportunity.

## Stop Loss

1. Find stop loss on the futures chart using previous swing-low/high, S/R levels, or ATR indicator.
2. Find the distance between current price and the stop loss. Lets say this distance is `r` (r := Spot - SL)
3. Multiply `r` with the option's `delta` (typically 20Δ or 0.20 in decimals). Lets say this value is `s` (s := r * 0.20)
4. Keep the S.L. on the option's price `s` distance away.

# Step 4. Monitor position
[[Strategy Builder Playbook#Step 4 Monitor position]]

# Step 5. Adjust position
