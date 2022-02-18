[Weekly Iron Fly](https://www.youtube.com/watch?v=REA-YxpS14c) | [Monthly Iron Fly](https://www.youtube.com/watch?v=9IodHBgG8Z8) | [...](https://youtu.be/dhEPY7DUBwI?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=592)

- Iron Fly (Straddle) loss is less than the Iron Condor (Strangle) loss.
- Iron Fly's Risk/Reward is over 1:2.5.

# Step 1. Wait for the setup

1. VIX is above 18.
2. Theta Gainer prefers Bank Nifty for Iron Fly.

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

Monitor daily @ 10:30 AM.

Act when market breaks through an overhead resistance or underlying support.

# Step 7. Adjust

## Approach 1. Follow straddle's adjustments
[[Short Straddle Playbook#1 3 Monthly Position]]

## Approach 2. Slide hedges, sell option and roll
[...](https://youtu.be/9IodHBgG8Z8?t=1291)

The only reason you do adjustments in Iron Fly is because when the back turn happens you can benefit from it.

> If in the beginning spot price is closer to one side of the breakeven point because you chose strike in the middle of S/R range then for that side skip the steps in Stage 1 to 3.
	- For the side which is now close to breakeven follow Stage 4.1 steps right away (as 1st step).
		- I.E. bring the hedge 0.55% to 0.75% inside on that side of the breakeven.
	- For the other side, which is far away from the spot, follow all the steps from Stage 1 to Stage 4.

### Stage 1. Risk defined straddle

##### Action: Start w/ outside hedges
[...](https://youtu.be/9IodHBgG8Z8?t=911)

Start with a defined risk straddle.
- You do not need a proper Iron Fly right in the beginning.
- Cut cost by not putting hedges around breakeven right from the start.
- For `weekly`, directly deploy a straddle at 10:20 AM `with stop loss but without hedges`.
- For `monthly`, define risk by putting hedges far outside of breakevens and trade it like a straddle.
	- Put `hedges 2% outside of breakeven`.
		- It is 200 points in Nifty.
	- The breakeven range will decrease after deploying the hedges.
		- This breakeven range would be far less if you hedged right at the breakevens.
	- This will also increase your Probability of Profit.

### Stage 2. 11% DTE wait

##### Action: Wait till 11% of DTE

- `Either` wait for 11% of DTE to pass.
	- In `weekly` trades, after deploying a naked straddle at 10:20 AM, `wait till 03:20 PM` before proceeding to next stage.
	- In `monthly` trades, after deploying a defined risk straddle, `wait for 3-5 days` before proceeding to next stage.
- `Or` wait for 1.5% impulsive move in any one direction. <== GovindThange Approach

Waiting may lead to some MTM profit. Also the cost of buying hedges may go down. You can then convert this straddle into an `Iron Fly` or a `Loss Less Iron Fly`. [...](https://youtu.be/REA-YxpS14c?&t=281)

### Stage 3.  Iron Fly launch

##### Action: Convert to Iron Fly
[...](https://youtu.be/9IodHBgG8Z8?t=1056)

1. Move hedges inwards to breakeven.
	- Close hedges deployed 2% out side of breakevens.
	- Deploy new `hedges at the 2 breakevens`.
	- This will convert straddle to a proper Iron Fly.
	- This will reduce the breakeven range.
	- This will reduce max. loss by few points.
2. Start following the market.

### Stage 4. Directional move
[...](https://youtu.be/9IodHBgG8Z8?t=1200)

As a guideline 1.5% move in any one direction in Nifty is bothersome and requires adjustments.

Shifting hedges decreases the breakeven range so do this step only when the breakeven range is over 7.5% (i.e. 100 x range/spot). We need a good breakeven range to do adjustments later.

> Step 1 through 4 are alternative to shifting Straddle. If you don't follow these 1-4 steps or shift straddle then the step 6 alone, i.e. selling an extra option and rolling it, won't recover much losses.

#### Stage 4.1 Price moves impulsively

##### Action: Roll down the hedged long call

1. Wait for 1.5% to 1.7% impulsive move in one direction.
	- This is 180-200 points move in Nifty.
2. `Roll the trending side hedge` 0.55% to 0.75% inwards from the breakeven.
	1. Slide the `hedge inwards breakeven by 0.55% to 0.75%`.
	2. Exit the long option on the trending side.
		- You may see some profit.
		- You may not see profit if volatility drops.
		- You may not see profit if many days have passed and there was theta decay. [...](https://youtu.be/REA-YxpS14c?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=821)
	3. Buy a new option as hedge on the tested side.
		- Pick a strike 0.55% to 0.75% inwards from the breakeven point.
		- It is best to do this just once. This was the first turn.
		- 0.75% is 100 points in Nifty.
		- 0.55% is 200 points in Bank Nifty.
3. Observe the payoff chart.
		- The losses on the trending side will go down.
		- This losses on the non trending side will slightly rise.
		- The blue t+0 line in opstra will become flatter on the trending side.
		- The breakeven range will reduce which is bad for future adjustment.

==Do not touch the hedge on the non trending side yet!==

You can only do few shifts on the non trending side. So save this for later.

#### Stage 4.2 Price approaches call side breakeven

Skip this step if Iron Fly is too small or price breaches the breakeven too fast.

##### Action: Roll hedges inwards on both sides

1. Wait for price to approach closer to breakeven point on the trending side.
2. `Roll the trending side hedge` 0.55% to 0.75% inwards from the breakeven.
	1. Exit the long option on the trending side.
		- You may see some profit.
		- You may not see profit if volatility drops.
		- You may not see profit if many days have passed and there was theta decay. [...](https://youtu.be/REA-YxpS14c?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=821)
	2. Buy a new option as hedge on the tested side.
		- Pick a strike which is inwards from breakeven point by 0.55% to 0.75% of the spot price.
		- It is best to do this just once. This was the first turn.
		- This was your second turn. It is best to shift call side hedge only once.
		- Do not do this more than twice.
		- 0.75% is 100 points in Nifty.
		- 0.55% is 200 points in Bank Nifty.
3. Observe the payoff chart again.
		- The losses on the trending side will go down.
		- This losses on the non trending side will slightly rise.
		- The blue t+0 line in opstra will become flatter on the trending side.
		- The breakeven range will further reduce.
4. Next, for the safety from gap-ups/down, also `roll the non trending side hedge` 0.75% inwards from the breakeven.
	1. `Exit the long` option on the non trending side.
		- You will see some loss.
	2. Buy a new option as hedge on the non trending side.
		- Pick a strike which is inwards from breakeven point by 0.55% to 0.75% of the spot price.
		- 0.75% is 100 points in Nifty.
		- 0.55% is 200 points in Bank Nifty.
		- This will reduce losses on the non trending side.
		- This would reduce the breakeven range even more.

### Stage 5. Breakeven approach w/ MTM profit ≥ 1% while

##### Action: Convert to a Loss Less Iron Fly
[...](https://youtu.be/REA-YxpS14c?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=276) | [...](https://youtu.be/REA-YxpS14c?t=167)

You can only make an Iron Fly loss less after you see some MTM profit.

1. Wait for 50% DTE to pass.
	- Do not attempt to make Iron Fly loss less right in the beginning.
	- If you make an Iron Fly loss less right from the beginning then you will not get enough range to ride the trade.
	- The cone in the payoff chart will become very narrow and thin.
2. Wait to `accumulate 1% MTM profit`.
	- This is 1% of `capital deployed as margin` + surplus `margin saved for selling of extra options`.
3. Make an Iron Fly loss less only when...
		- The spot price is too far away from the Max Profit zone (the green structure in payoff chart).
		- `And` the MTM is showing considerable profit that you don't want to risk loosing.
		- `And` the DTE is close i.e. very less time is remaining for expiry.
		- `And` your confidence level is not high.
		- `And` there is little hope of market returning.
4. Wait for price to approach the breakeven point on one side.
5. Bring hedges inside the breakeven point of the side being tested.
	- Slide the hedge inwards by 1% to 1.2%.
		- Exit from the existing hedge on the tested side.
		- Create a new hedge `hedge 1% to 1.2% inside breakeven`.
	- This is typically 400 points inside breakevens in Bank Nifty.
	- Do not bring hedges inwards on both sides at the same time.
	- Analyze payoff chart to confirm a proper `One Sided Loss Less Iron Fly`.
		- The side which was made loss should appear all green w/o distorting the structure of chart.
		- Note that you sacrificed your Max Profit potential in order to make it loss less.
6. Now wait for price to approach the breakeven point on the other side.
7. Bring hedges inside the breakeven point of the other side which is being tested.
	- Slide the hedge inwards by 1% to 1.2%.
		- Exit from the existing hedge position on the tested side.
		- Create a new `hedge 1% to 1.2% inside breakeven`.
	- This is typically 400 points inside breakevens in Bank Nifty.8. Analyze payoff chart to confirm Loss Less Iron Fly.
	- Analyze the payoff chart to confirm a  `Complete Loss Less Iron Fly` that is loss less on both the sides.
8. To lock MTM gains even further `repeat step 3 through 7`.
	- Making Iron Fly loss less drastically reduces the Max. Profit.
	- Do this in conjunction with a proper technical analysis.

> Do not make Iron Fly completely loss less. Leave enough on table so that you are not fearful and at the same time have enough room to be in the trade (do adjustments) till expiry. [...](https://youtu.be/REA-YxpS14c?t=1085)

### Stage 6. Breakeven breach
[...](https://youtu.be/9IodHBgG8Z8?t=1362)

Once price breaches the breakeven point the entire goal of doing adjustment is to gradually reduce losses caused by the directional move of the market. We can comfortably manage the trade till expiry and close it with a minimum possible loss.

##### Action: Sell an extra option and roll

1. Sell an extra option w/ `1 lot` from `breakeven` of the `same monthly expiry` on the non tested side. [...](https://youtu.be/9IodHBgG8Z8?t=1792)
	1. Pick a `strike at or close to the breakeven` on the non tested side.
	2. Now short an option with this selected strike.
2. Wait for the above option premium to `reduce by 50%`, or `by ₹20 in Nifty`, or `by ₹30 in Bank Nifty` and then exit it.
3. If market moves further in the same direction then again short an option on the non tested side.
	- If premiums are high enough then
		- `Either` select a strike with premium ₹20 (in Nifty) or ₹30 (in Bank Nifty) lesser than the one you shorted in steps above.
		- `Or` select a strike with premium same as earlier one when you shorted it.
		- `Or` select a strike that is far by 7% to 8% (i.e. 1000 points in Nifty).
	- Ensure that the strike price is safe as per your analysis.
		- Keep analyzing the chart for support region.
		- If the short put strike distance from the spot is 7% to 8% (say 1000 points in Nifty) then it can be considered a safe distance.
		- If the market has shown a straight impulsive move towards upside and only few days are left for the monthly expiry then you can even short options till the strike distance from the spot is 3.5% to 4% (i.e. 500 points in Nifty).
4. Exit this short option when...
	- The strike price of put crosses the middle of payoff chart i.e. the middle of original straddle cone (green zone).
	- `Or` the VIX is high and rising and the current price has reversed, moved in the oppsite direction and came within the breakeven.
5. Repeat step 2 through 4 as market moves further in the same direction.
	- Never cut your Iron Fly trade if you can bear the loss shown on the right side.
	- Although selling option on the non tested side pose undefined risk, but before causing  this loss it will first come inside the straddle range to incur Max Profit. Your staddle is the first primary protection from the undefined loss.
	- As you keep selling options and come inwards from the left side you will no more see a triangle/cone in payoff chart. It will become flat on the top. [...](https://youtu.be/IaEjcuBNPgg?t=1193)
	- Be warned about shifting put too deep inside from the non tested side.
		- By selling an extra option on the non tested side the loss on the tested side of payoff chart is fixed.
		- New short puts created with strikes too deep inside will pose risk if market reverses.
		- Once market reverses the short put will quickly become ITM.
		- Say you created a straddle at 13,300 then go inside by just 300 to 400 points only.
			- This will reduce your max profit potentially substantially.
			- Say current lot size is of 50 quantity.
			- If you move inside by 300 points then you lose profit by ₹15,000 (300 x 50).
			- If market reverses your final profit will be reduced by ₹15,000.

### Stage 7. Iron Fly failure

1. Exit with the lowest drawdown, cost to cost, or at the current MTM profit.
2. Create new Iron Fly in the direction of the market.

## Approach 3. Rebalance delta
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
	4. The price continued its move in the opposite directoin.
	5. The price moved substantially in the opposite direction.
	6. The price is on the verge of crossing the mid point of Iron Fly.
	7. Several days have passed.
	8. There is still some MTM profit left for a safe exit.
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
