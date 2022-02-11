[Weekly Iron Fly](https://www.youtube.com/watch?v=REA-YxpS14c) | [Monthly Iron Fly](https://www.youtube.com/watch?v=9IodHBgG8Z8) | [...](https://youtu.be/dhEPY7DUBwI?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=592)

# Step 1. Wait for the setup

- VIX is above 18.
- Theta Gainer prefers Bank Nifty for Iron Fly.

# Step 2. Find range
[[Strategy Builder Playbook#Step 1 Find range]]

# Step 3. Cover range
[...](https://youtu.be/9IodHBgG8Z8?t=595)

[[Strategy Builder Playbook#Step 2 Cover range]]

Make straddle exactly at the middle of the range.
- You need not sell call & put at the exact same strike.
	- Its fine to go slightly diagonal i.e. selling at slightly different strikes.
- You may also short ATM instead of middle of the range.

# Step 4. Define risk
[...](https://youtu.be/9IodHBgG8Z8?t=811)

Hedge naked straddle using Iron Fly.

1. Define risk with 1:1 Risk/Reward ratio.
	- If you receive 10k in credit, then only debit 10k for hedging.
	- Its fine to pay slightly extra.
2. Use one of the following 2 approaches to hedge:
	1. `Either` use `breakevens` to pick strikes for hedging.
		- Use the received credit to buy call & put at the breakeven (approx).
	2. `Or` pick the strikes corresponding to the credit received from the sold options.
3. By buying call & put at the breakeven will decrease the breakeven range.

# Step 5. Deploy

- Deploy Monthly Iron Fly like so:
	- Have 45 DTE strategy.
	- Enter trade on the 3rd week, Thursday @ 10:20 AM of current month.
	- Exit trade on last thursday of next month.
- Deploy Weekly Iron Fly like so:
	- Enter trade on Wednesday @ 10:30 AM or 01:20 PM.
	- Exit trade next week on Wednesday @ 3:00 PM or by Thursday @ 9:20 AM.

# Step 6. Monitor position
[[Strategy Builder Playbook#Step 4 Monitor position]]

Monitory daily @ 10:30 AM.

# Step 7. Adjust position
[...](https://youtu.be/9IodHBgG8Z8?t=1291)

The only reason you do adjustments in Iron Fly is because when the back turn happens you can benefit from it.

## Stage 1. Start w/ outside hedges
[...](https://youtu.be/9IodHBgG8Z8?t=911)

Start with a defined risk straddle.
- You do not need a proper Iron Fly right in the beginning.
- Cut cost by not putting hedges around breakeven right from the start.
- For weekly, directly deploy a straddle at 9:20 AM without any hedges but with a stop loss.
- For monthly, define risk by putting hedges far outside of breakevens and trade it like a straddle.
	- This will increase your breakeven range compared to hedges right at breakevens.
	- This will also increase your Prob. of Profit.

## Stage 2. Wait for 11% of DTE

- In `weekly` trades, after deploying a naked straddle at 9:20 AM, `wait till 3 PM` before proceeding to next stage.
- In `monthly` trades, after deploying a defined risk straddle, `wait for 3-5 days` before proceeding to next stage.

Once your staddle is successful after recommended waiting, you not only have MTM profit, the cost of buying hedges would also decrease. You can then convert this straddle into an `Iron Fly` or a `Loss Less Iron Fly`. [...](https://youtu.be/REA-YxpS14c?&t=281)

## 3. Convert to Iron Fly
[...](https://youtu.be/9IodHBgG8Z8?t=1056)

1. Move hedges inwards to breakeven.
	- This will convert straddle to a proper Iron Fly.
	- This will reduce the breakeven range.
	- This will reduce max. loss by few points.
2. Start following the market.

### Make a Loss Less Iron Fly
[...](https://youtu.be/REA-YxpS14c?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=276) | [...](https://youtu.be/REA-YxpS14c?t=167)

You can only make an Iron Fly loss less after you see some MTM profit.

1. Do not attempt to make Iron Fly loss less right in the beginning.
	- If you make an Iron Fly loss less right from the beginning then you will not get enough range to ride the trade.
	- The cone in the payoff chart will become very narrow and thin.
2. Wait to accumulate some MTM profit.
3. Create an Iron Fly with hedges inside its breakeven points.
	- Create hedges 1% to 1.2% inside.
	- This is typically 400 points inside breakevens in Bank Nifty.
4. Analyze payoff chart to confirm Loss Less Iron Fly.
	- Note that you sacrificed your Max Profit potential in order to make it loss less.

> Do not make completely loss less. Leave enough on table so that you are not fearful and at the same time you can be in trade for long.  [...](https://youtu.be/REA-YxpS14c?t=1085)

## Stage 4. Shift hedges upon directional move
[...](https://youtu.be/9IodHBgG8Z8?t=1200)

As a guideline 1.5% move in any one direction in Nifty is bothersome and requires adjustments.

### Case 1. When price approaches call side breakeven

#### Stage 3.1 Price moves impulsively

1. Wait for 1.5% impulsive move towards upside. This is 180-200 points move in Nifty.
2. Slide down the call side hedge by few points.
	1. Exit the call side long position and book the profit.
	2. Buy a new call with strike inwards by 0.55% to 0.75% points.
		- It is best to do this just once. This was your first turn.
		- 0.75% is 100 points inside breakeven in Nifty.
		- 0.55% is 200 points inside breakeven in Bank Nifty.
3. Observe the payoff chart.
		- The losses on the call side will go down.
		- This losses on the put side will slightly rise.
		- The blue t+0 line in opstra will become flatter on the call side.
		- The breakeven range will reduce.

==Do not touch the put side hedge yet!==

You can only do few shift on the put side. So save this for later.

#### Stage 3.2 Price approaches call side breakeven

1. Wait for price to come close to the call side breakeven.
2. Again slide down the call side hedge by 0.55% to 0.75% points.
	1. Exit the call side long position and book the profit.
		- You may not be able to book profit if many days have passed and the call side was incurred theta decay. [...](https://youtu.be/REA-YxpS14c?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=821)
	2. Buy a new call with strike inwards by 0.55% to 0.75% points.
		- This was your second turn. It is best to shift call side hedge only once.
		- Do not do this more than twice.
		- 0.75% is 100 points inside breakeven in Nifty.
		- 0.55% is 200 points inside breakeven in Bank Nifty.
3. Observe the payoff chart again.
		- The losses on the call side will further go down.
		- This losses on the put side will slightly rise.
		- The blue t+0 line in opstra will become flatter on the call side.
		- The breakeven range will further reduce.
4. Next slide up the put side hedge by 0.75% points for safety from the gap downs.
	1. Exit the put side long position and book the loss.
	2. Buy a new put with strike inwards by 0.75% points (i.e. increase strike by 100 points in Nifty)
		- This will reduce losses on the put side.
		- This would reduce the breakeven range even more.

### Case 2. When price approaches put side breakeven

## Stage 5. Price breaches breakeven
[...](https://youtu.be/9IodHBgG8Z8?t=1362)

Once price breaches the breakeven point the entire goal of doing adjustment is to gradually reduce losses caused by the directional move of the market. We can comfortably manage the trade till expiry and close it with a minimum possible loss.

Iron Fly can be managed till the day of expiry.
- [V Shape Recovery | 18 March 2021 to 29 April 2021](https://youtu.be/IaEjcuBNPgg?t=163)
	- We safely managed a directional move of 4000 points (12% drop) to the down side w/ max. loss of ₹9,000.
	- We then sustained the complete recovery of 12.9% withoug exceeding loss of ₹9,000.
	- We managed trade to convert a ₹19,000 loss into profit.
	- We closed trade in profit of ₹14,000 by giving margin of ₹2,00,000.
- [Strong Trend | 12 April 2021 to 29 April 2021](https://youtu.be/IaEjcuBNPgg?t=1365)
	- We created Iron Fly with very low premium.
	- Market trends 7.35% (2500 points) after breaching the range of 2,250 points.
	- We managed trade to reduce drawdown from ₹14,377 to ₹4,136.

1. Sell a 1 lot option from breakeven on the non tested side. [...](https://youtu.be/9IodHBgG8Z8?t=1792)
	1. Pick a strike at or close to the breakeven on the non tested side.
	2. Now short an option with this selected strike.
2. Wait for this option premium to reduce to ₹20 (₹30 in Bank Nifty) and then exit it.
3. If market moves further in the same direction then again short an option on the non tested side.
	- If premiums are high enough then
		- `Either` select a strike with premium ₹20 lesser (₹30 in Bank Nifty) than the one you shorted earlier.
		- `Or` select a strike with premium same as earlier one when you shorted it.
		- `Or` select a strike that is far enough (say 7% to 8% or 1000 points in Nifty).
	- Ensure that the strike price is safe as per your analysis.
		- Keep analyzing the chart for support region.
		- If the short put strike distance from the spot is 7% to 8% (say 1000 points in Nifty) then it can be considered a safe distance.
		- If the market has shown a straight impulsive move towards upside and only few days are left for the monthly expiry then you can even short options till the strike distance from the spot is 3.5% to 4% (i.e. 500 points in Nifty).
4. Exit when the strike price of put crosses the middle of payoff chart i.e. the middle of original straddle cone (green zone).
5. Repeat step 2 through 4 as market moves further in the direction.
	- Never cut your Iron Fly trade if you can bear the loss shown on the right side.
	- Although selling option on the non tested side pose undefined risk, but before causing  this loss it will first come inside the straddle range to incur Max Profit. Your staddle is the first primary protection from the undefined loss.
	- As you keep selling options and come inwards from the left side you will no more see a triangle/cone in payoff chart. It will become flat on the top. [...](https://youtu.be/IaEjcuBNPgg?t=1193)
	- Be warned about shifting put too deep inside on the non tested side.
		- The loss shown on the right side of payoff chart has been fixed.
		- New short puts created with strikes too deep inside will pose risk if market reverses.
		- Once market reverses the short put will quickly become ITM.
		- Say you created a straddle at 13,300 then go inside by just 300 to 400 points only.
			- This will reduce your max profit potentially substantially.
			- Say current lot size is of 50 quantity.
			- If you move inside by 300 points then you lose profit by ₹15,000 (300 x 50).
			- If market reverses your final profit will be reduced by ₹15,000.

## Stage 6. Iron Fly fails

- `Either` exit with the lowest drawdown, cost to cost, or at the current MTM profit.
- `Or` create new Iron Fly in the direction of the market.

# Step 8. Exit

- Exit when the Monthly Iron Fly delivers 2% profit.
- Exit when the Weekly Iron Fly delivers 1% profit.
- If Iron Fly fails then exit with the lowest drawdown, cost to cost, or at the current MTM profit.