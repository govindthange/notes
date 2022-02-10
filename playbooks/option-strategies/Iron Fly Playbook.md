[...](https://www.youtube.com/watch?v=9IodHBgG8Z8) | [...](https://youtu.be/dhEPY7DUBwI?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=592)

# Step 1. Find range
[[Strategy Builder Playbook#Step 1 Find range]]

# Step 2. Cover range
[...](https://youtu.be/9IodHBgG8Z8?t=595)

[[Strategy Builder Playbook#Step 2 Cover range]]

Make straddle exactly at the middle of the range.
- You need not short call and put at the exact same strike. Its fine to go slightly diagonal i.e. shorting at slightly different strikes.
- You may also short ATM instead of middle of the range.

# Step 3. Define risk
[...](https://youtu.be/9IodHBgG8Z8?t=811)

Hedge naked straddle using Iron Fly.

1. Define risk with 1:1 Risk/Reward ratio.
	- If you receive 10k in credit, then only debit 10k for hedging.
	- Its fine to pay slightly extra.
2. Use one of the following 2 approaches to hedge:
	1. Either use `breakevens` to pick strikes for hedging.
		- Use the received credit to buy put and call at the breakeven (approx).
		- By buying PE & CE options at the breakeven will reduce the breakeven range.
	2. Or pick the strikes corresponding to the credit received from the sold options.
3. By buying PE & CE options will increase breakeven range.

# Step 4. Deploy

- Deploy monthly strategy on Thursday @ 10:20

# Step 5. Monitor position
[[Strategy Builder Playbook#Step 4 Monitor position]]

# Step 6. Adjust position
[...](https://youtu.be/9IodHBgG8Z8?t=1291)

The only reason you do adjustments in Iron Fly is because when the back turn happens you can benefit from it.

## Stage 1. Start w/ outside hedges
[...](https://youtu.be/9IodHBgG8Z8?t=911)

Start with a defined risk straddle.
- You do not need a proper Iron Fly right in the beginning.
- Cut cost by not putting hedges around breakeven right from the start.
- Just define risk by putting hedges ar outside of breakevens and trade it like a straddle.
- This will increase your breakeven range.
- This will also increase your Prob. of Profit.

## Stage 2. Convert to Iron Fly
[...](https://youtu.be/9IodHBgG8Z8?t=1056)

1. Wait for 3-5 days in monthly trade.
2. Move hedges inwards to breakeven.
	- This will convert straddle to a proper Iron Fly.
	- This will reduce the breakeven range.
	- This will reduce max. loss by few points.
4. Start following the market.

## Stage 3. Shift hedges upon directional moves
[...](https://youtu.be/9IodHBgG8Z8?t=1200)

As a guideline 1.5% move in any one direction in nifty is bothersome and requires adjustments.

### Case 1. When price approaches call side breakeven

#### Stage 3.1 Price moves impulsively

1. Wait for 1.5% impulsive move towards upside. This is 180-200 points move in nifty.
2. Slide down the call side hedge by few points.
	1. Exit the call side long position and book the profit.
	2. Buy a new call with strike inwards by 0.75% points (i.e. 100 points inside in nifty).
		- This will reduce the loss on the call side.
		- The blue t+0 line in opstra will become flat on the call side.
		- It will further reduce the breakeven range.
		- It is best to do this just once. This was your first turn.

==Do not touch the put side hedge!==

#### Stage 3.2 Price approaches call side breakeven

1. Wait for price to come close to the call side breakeven.
2. Again slide down the call side hedge by 0.75% points.
	1. Exit the call side long position and book the profit.
	2. Buy a new call with strike inwards by 0.75% points (i.e. 100 points inside in nifty).
		- This was your second turn. It is best to shift call side hedge only once.
		- Do not do this more than twice.
3. Next slide up the put side hedge by 0.75% points.
	1. Exit the put side long position and book the loss.
	2. Buy a new put with strike inwards by 0.75% points (i.e. increase strike by 100 points in nifty)
		- This will reduce losses on the put side.
		- This would reduce the breakeven range even more.

### Case 2. When price approaches put side breakeven

## Stage 4. Price breaches breakeven
[...](https://youtu.be/9IodHBgG8Z8?t=1362)

Once price breaches the breakeven point the entire goal of doing adjustment is to comfortably manage the trade till expiry and close it with a minimum possible loss.

1. Sell a 1 lot option from breakeven on the non tested side. [...](https://youtu.be/9IodHBgG8Z8?t=1792)
	1. Pick a strike at or close to the breakeven on the non tested side.
	2. Now short an option with this selected strike.
2. Wait for this option premium to reduce to ₹20 and then exit it.
3. If market moves further in the same direction then again short a new option.
4. Short another option.
	- If premiums are high enough then
		- `Either` select a strike with premium ₹20 lesser than the one you shorted earlier.
		- `Or` select a strike with premium same as earlier one when you shorted it.
		- `Or` select a strike that is far enough (say 7-8% or 1000 points in nifty).
	- Ensure that the strike price is safe as per your analysis.
		- Keep analyzing the chart for support region.
		- If the short put strike distance from the spot is 7-8% (say 1000 points in nifty) then it can be considered a safe distance.
		- If the market has shown a straight impulsive move towards upside and only few days are left for the monthly expiry then you can even short options till the strike distance from the spot is 3.5-4% (i.e. 500 points in nifty).
5. Repeat step 2 through 4 as market moves further in the direction.
	- Never cut your Iron Fly trade if you can bear the loss shown on the right side.
	- As you short options and come closer from the left side you will no more see a triangle/cone in payoff chart.
	- Be warned about shifting put too deep inside to reduce losses on the right side of payoff chart.
		- The loss shown on the right side of payoff chart has been fixed.
		- New short puts created with strikes too deep inside will pose risk if market reverses.
		- Once market reverses the short put will quickly become ITM.
		- Say you created a straddle at 13300 then go inside by just 300 to 400 points only.
			- This will reduce your max profit potentially substantially.
			- Say current lot size is of 50 quantity.
			- If you move inside by 300 points then you lose profit by ₹15,000 (300 x 50).
			- If market reverses your final profit will be reduced by ₹15,000.