[Weekly Iron Fly](https://www.youtube.com/watch?v=REA-YxpS14c) | [Monthly Iron Fly](https://www.youtube.com/watch?v=9IodHBgG8Z8) | [...](https://youtu.be/dhEPY7DUBwI?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=592)


Iron Fly (Straddle) loss is less than the Iron Condor (Strangle) loss.

# Step 1. Wait for the setup

- VIX is above 18.
- Theta Gainer prefers Bank Nifty for Iron Fly.

# Step 2. Find range
[[Strategy Builder Playbook#Step 1 Find range]]

# Step 3. Cover range
[...](https://youtu.be/9IodHBgG8Z8?t=595)

[[Strategy Builder Playbook#Step 2 Cover range]]

Make straddle like so:
1. Mark [[Support & Resistance#S R in a Range]] on a 1 hour Nifty chart.
2. Analyze the [[Option Chain]] to select a strike that satisfies following conditions:
	1. The selected strike should give higher credit from call & put premiums.
		- By collecting higher credit gives better breakeven range for doing future adjustments.
	2. The selected strike lies within the middle zone of overhead resistance & underlying support range.
		- Its possible to receive better premiums for strikes in the middle of S/R range compared to ATM strike premiums.
	3. The gap between the breakeven may favor trend depicted by SuperTrend indicator.
		- The gap between the `selected strike` and the `call side breakeven` should be `≥ 50%` for bullish trend.
		- The gap between the `selected strike` and the `put side breakeven` should be `≥ 50%` for bearish trend.
	4. The selected strike should not be too far away from ATM.
3. You need not sell call & put at the exact same strike.
	- Its fine to go slightly diagonal i.e. selling at slightly different strikes.

> In monthly trades, for first 10 days use future spot price for picking strikes. Later towards the end of month you can use normal spot price for picking strikes. [...](https://youtu.be/A-zpeOlgtOY?t=1697)

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
	- Enter trade on the 3rd week, Wednesday @ 10:20 AM of current month.
	- Exit trade on last thursday of next month.
- Deploy Weekly Iron Fly like so:
	- Enter trade on Wednesday @ 10:20 AM or 01:20 PM.
	- Exit trade next week on Wednesday @ 3:00 PM or by Thursday @ 10:20 AM.

# Step 6. Monitor position
[[Strategy Builder Playbook#Step 4 Monitor position]]

Monitory daily @ 10:30 AM.

# Step 7 (A). Adjust position w/ breakevens
[...](https://youtu.be/9IodHBgG8Z8?t=1291)

The only reason you do adjustments in Iron Fly is because when the back turn happens you can benefit from it.

> If in the beginning spot price is closer to one side of the breakeven point because you chose strike in the middle of S/R range then for that side skip the steps in Stage 1 to 3.
	- For the side which is now close to breakeven follow Stage 4.1 steps right away (as 1st step).
		- I.E. bring the hedge 0.55% to 0.75% inside on that side of the breakeven.
	- For the other side, which is far away from the spot, follow all the steps from Stage 1 to Stage 4.

## Stage 1. Risk defined straddle

##### Action: Start w/ outside hedges
[...](https://youtu.be/9IodHBgG8Z8?t=911)

Start with a defined risk straddle.
- You do not need a proper Iron Fly right in the beginning.
- Cut cost by not putting hedges around breakeven right from the start.
- For `weekly`, directly deploy a straddle at 10:20 AM `with stop loss but without hedges`.
- For `monthly`, define risk by putting hedges far outside of breakevens and trade it like a straddle.
	- Put `hedges 12% outside of breakeven`. It is 200 points in Nifty.
	- The breakeven range will decrease after deploying the hedges.
		- This breakeven range would be far less if you hedged right at the breakevens.
	- This will also increase your Prob. of Profit.

## Stage 2. Waiting

##### Action: Wait till 11% of DTE

- Wait for 11% of DTE
	- In `weekly` trades, after deploying a naked straddle at 10:20 AM, `wait till 03:20 PM` before proceeding to next stage.
	- In `monthly` trades, after deploying a defined risk straddle, `wait for 3-5 days` before proceeding to next stage.
- Wait for 1.5% impulsive move in any one direction. <== GovindThange Approach

Waiting may lead to some MTM profit. Also the cost of buying hedges may go down. You can then convert this straddle into an `Iron Fly` or a `Loss Less Iron Fly`. [...](https://youtu.be/REA-YxpS14c?&t=281)

## Stage 3.  Iron Fly launch

##### Action: Convert to Iron Fly
[...](https://youtu.be/9IodHBgG8Z8?t=1056)

1. Move hedges inwards to breakeven.
	- Close hedges deployed 12% out side of breakevens.
	- Deploy new `hedges at the 2 breakevens`.
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
	- Create `hedges 1% to 1.2% inside breakevens`.
	- This is typically 400 points inside breakevens in Bank Nifty.
4. Analyze payoff chart to confirm Loss Less Iron Fly.
	- Note that you sacrificed your Max Profit potential in order to make it loss less.

> Do not make Iron Fly completely loss less. Leave enough on table so that you are not fearful and at the same time have enough room to be in the trade (do adjustments) till expiry. [...](https://youtu.be/REA-YxpS14c?t=1085)

## Stage 4. Directional move
[...](https://youtu.be/9IodHBgG8Z8?t=1200)

As a guideline 1.5% move in any one direction in Nifty is bothersome and requires adjustments.

> Shifting hedges decreases the breakeven range so do this step only if the breakeven range is over 7.5% (i.e. 100 x range/spot). We need a good breakeven range to do adjustments.

### Case 1. When price approaches call side breakeven

#### Stage 4.1 Price moves impulsively

##### Action: Roll down the hedged long call

1. Wait for 1.5% to 1.7% impulsive move towards upside. This is 180-200 points move in Nifty.
2. Slide down the `call side hedge 0.55% to 0.75% inside breakeven`.
	1. Exit the call side long position and book the profit.
		- You may not be able to book profit if many days have passed and the call side incurred some theta decay. [...](https://youtu.be/REA-YxpS14c?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=821)
	2. Buy a new call with strike 0.55% to 0.75% inwards from the breakeven.
		- It is best to do this just once. This was your first turn.
		- 0.75% is 100 points in Nifty.
		- 0.55% is 200 points in Bank Nifty.
3. Observe the payoff chart.
		- The losses on the call side will go down.
		- This losses on the put side will slightly rise.
		- The blue t+0 line in opstra will become flatter on the call side.
		- The breakeven range will reduce which is bad for future adjustment.

==Do not touch the put side hedge yet!==

You can only do few shifts on the put side. So save this for later.

#### Stage 4.2 Price approaches call side breakeven

Skip this step if Iron Fly is too small or breached the breakeven too fast.

##### Action: Roll down hedges on both sides

1. Wait for price to come close to the call side breakeven.
2. `Roll down the hedged long call` i.e. slide down the `call side hedge 0.55% to 0.75% inside breakeven` like so:
	1. Exit the call side long position and book the profit.
		- You may not be able to book profit if many days have passed and the call side incurred some theta decay. [...](https://youtu.be/REA-YxpS14c?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=821)
	2. Buy a new call with strike 0.55% to 0.75% inwards from the breakeven.
		- This was your second turn. It is best to shift call side hedge only once.
		- Do not do this more than twice.
		- 0.75% is 100 points in Nifty.
		- 0.55% is 200 points in Bank Nifty.
3. Observe the payoff chart again.
		- The losses on the call side will further go down.
		- This losses on the put side will slightly rise.
		- The blue t+0 line in opstra will become flatter on the call side.
		- The breakeven range will further reduce.
4. `Roll up the hedged long put` i.e. slide up the `put side hedge 0.75% inside breakeven` for safety from the gap downs like so:
	1. Exit the put side long position and book the loss.
	2. Buy a new put with strike 0.55% to 0.75% inwards to the breakeven.
		- This will reduce losses on the put side.
		- This would reduce the breakeven range even more.
		- 0.75% is 100 points in Nifty.
		- 0.55% is 200 points in Bank Nifty.

### Case 2. When price approaches put side breakeven

## Stage 5. Breakeven breach
[...](https://youtu.be/9IodHBgG8Z8?t=1362)

Once price breaches the breakeven point the entire goal of doing adjustment is to gradually reduce losses caused by the directional move of the market. We can comfortably manage the trade till expiry and close it with a minimum possible loss.

##### Action: Sell an extra option and roll

1. Sell an extra option w/ 1 lot from breakeven on the non tested side. [...](https://youtu.be/9IodHBgG8Z8?t=1792)
	1. Pick a `strike at or close to the breakeven` on the non tested side.
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
4. Exit this short option when...
	- The strike price of put crosses the middle of payoff chart i.e. the middle of original straddle cone (green zone).
	- The current price reverses, moves in the oppsite direction and crosses the middle point of the Iron Fly.
5. Repeat step 2 through 4 as market moves further in the same direction.
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

## Stage 6. Iron Fly failure

1. Exit with the lowest drawdown, cost to cost, or at the current MTM profit.
2. Create new Iron Fly in the direction of the market.

# Step 7 (B). Adjust position w/ delta
[...](https://www.youtube.com/watch?v=DKJ5LnYgzQA)

1. Create an Iron Fly using 50Δ CE/PE w/ 20Δ hedges
2. When positional delta breaches 25Δ create a spread on the untested side.
	1. Sell a 20Δ option.
	2. Buy a 10Δ option.
3. Track sell side delta of this spread. Do nothing on the buy side of spread.
4. Exit the sell side once it goes below 10Δ.
5. Sell a new 20Δ option.
6. Go to step 3.

# Step 8. Exit

- Exit on or before 8 DTE for Monthly Iron Fly.
	- Position must be exited by Wednesday 10:20 AM of the 3rd week of expiry month.
	- Be ready for the new next month's expiry Iron Fly deployment on Wednesday 10:20 AM of the 3rd week of expiry month.
- Exit when the Monthly Iron Fly delivers 2% profit.
- Exit when the Weekly Iron Fly delivers 1% profit.
- Exit when M2M profit goes above 50% of Max Profit.
- Exit when following happens in sequence:
	1. You did several adjustment to manage loss.
	2. Price after several adjustment has gone beyond one end of the Iron Fly's breakeven.
	3. The price then reversed back.
	4. The price moved substantially in the opposite direction.
	5. Finally the price is on verge of crossing the middle point of Iron Fly.
	6. Since the price is crossing the midle of the Iron Fly again and as several days may have passed w/ lot of adjustment you finally see some MTM profit to safely exit.
- Exit when the volatility rises substantially and it makes more sense to initiate a new Iron Fly with better premiums and increased breakeven range compared to the current one.
- If Iron Fly fails then exit with the lowest drawdown, cost to cost, or at the current MTM profit.

---

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
