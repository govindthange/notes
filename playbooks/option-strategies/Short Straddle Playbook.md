Straddle works better than Strangles.
- `If` you create a strangle that has
	1. Same premium as that of corresponding straddle.
	2. Same breakeven as that of straddle.
- `And` there is a directional move
- `Then` Strangle may show some loss whereas straddle may retain its profit or at least show no losses.

Straddles are best when you are able to collect good premiums and you can manage position actively.

# Step 1. Wait for the setup
[...](https://www.youtube.com/watch?v=H8z3Es-Rgso)

1. High evironment.
2. IV rank above 50%.
3. High premiums.
	- Deploy straddles only when you can collect higher premiums.
		- ₹600 is considered good for monthly straddles in Bank Nifty
		- ₹300-₹400 is considered good for monthly straddles in Nifty
	- With higher premium you can cover bigger range and comfortably ride the market.
	- With sufficient premiums you can adjust with confidence.

# Step 2. Define risk

- For safety hedge naked straddle using `far OTM strikes` of `next expiry` `outside breakeven`.
- Don't make it Iron Fly by keeping hedges close to breakeven. Its a different strategy.

# Step 3. Deploy

- For `intraday` in Bank Nifty, deploy on Wednesday and Thursday only.
	- Enter @ 10:00 AM.
	- Exit @ 12:00 PM to 1:00 PM.
	- Between 10 AM to 1:00 PM there is not much movement in market.
- Its not safe to do intraday ATM straddle on Friday and Monday.
- For `monthly`, deploy straddle like so:
	- Have 45 DTE strategy.
	- Enter trade on the 3rd week, Wednesday @ 10:20 AM of current month.
	- Exit trade on last thursday of next month.
- For `weekly`, depoy straddle like so:
	- Enter trade on Wednesday @ 10:20 AM or 01:20 PM.
	- Exit trade next week on Wednesday @ 3:00 PM or by Thursday @ 10:20 AM.

> In monthly trades, for first 10 days use future spot price for picking strikes. Later towards the end of month you can use normal spot price for picking strikes. [...](https://youtu.be/A-zpeOlgtOY?t=1697)

# Step 4. Adjust

The very meaning of straddle is that you have deployed a strategy to create balance. [...](https://youtu.be/c9bcctkLV7A?t=1481)
- This means whenever market extends towards one side, the other side's profit must offset the losses from tested side.
- When you reach a point where you `straddle shows losses` then it means you have reached a point of imbalance.
	- Delta of one side has become faster than the other side delta.
	- So the rate at which one side premium decreases is greater than the rate at which the other side premium increases.
	- You must cut this straddle.
- When you reach a profit where your `straddle shows profit` and then it `undergoes imbalance` then you may not be able to catch it from the surface.
	- You will not directly see a loss.
	- First your profit will erode and then losses will appear.
	- To prevent this track premiums of both side and compare to see whether overall it is resulting in a loss.
	- When premium of one side substantially decreases in relation to the other side then it can no more offset otherside losses. [...](https://youtu.be/c9bcctkLV7A?t=806)
		- Whenever the 2 premiums reaches 1:3+ ratio then exit the straddle. [...](https://youtu.be/c9bcctkLV7A?t=1016)
			- Wait for the tested side short premium to go over 3 times higher than the non tested side short premium and then exit.
			- When you reach 1:3+ that means you are coming near to the straddle edge.
			- This is a best technique to exit before incurring further losses.
		- Do not let your current profit erode further.
		- There is no need to further wait and realize loss.
		- You have reached a point where you create a fresh straddle where both sides are well balanced.

## Approach 1.  Adjust using TA
[...](https://youtu.be/H8z3Es-Rgso?t=392)

Act when market breaks through an overhead resistance or underlying support.

1. Monitor S/R levels or candlestick patterns.
2. Do not do anything if market is within your defined straddle range.
3. When market `goes up by 0.55% to 0.75%` or `approaches an overhead resistance`... [...](https://youtu.be/H8z3Es-Rgso?t=735)
	1. First, roll up the short put.
	2. Next, as market follows up, gradually increase short put quantity (i.e. sell extra puts).
		- 0.75% is 100 points in Nifty.
		- 0.55% is 200 points in Bank Nifty.
4. When market attempts to `breach overhead resistance`...
	1. Decrease short call quantity by half and `convert it to a Ratio Spread`.
	2. Do not touch the next expiry long call as its working in your favor.
5. `Roll up the extra short put` when its premium become worthless.

[Weekly Backtest](https://youtu.be/H8z3Es-Rgso?t=1000)

## Approach 2. Shift straddle upon impulsive move

The entire logic behind straddle is collection of high premium. As long as you are in the center there is no reason to fear.

### 1.1. Intraday in weekly position
[...](https://youtu.be/A-zpeOlgtOY?t=868)

1. Wait for 25% directional move of the total breakeven range.
	- This is 50% of breakeven on one side.
	- If you have 440 points on each side, then wait for a 110 point move.
	- Being an intraday trade, monitor it very closely.
2. Exit from current straddle...
	- There is 25% directional move of the total breakeven range.
	- Spot price has breached breakeven range i.e. it has gone beyond total points received in credit. [...](https://youtu.be/c9bcctkLV7A?t=145)
3. Create a new straddle at the current point.
4. Go to step 1.

### 1.2. Weekly Position

For overnight safety also follow [[#Approach 3 Iron Fly for overnight safety]]

1. Wait for 1.5% to 1.7% move in one direction.
	- In points this is roughly 25% of the total received credit.
	- 140 points in Nifty.
	- 350-400 Points in Bank Nifty.
2. Exit from current straddle when...
	- There is 1.5% to 1.7% move from the middle in one direction.
	- Spot price has breached breakeven range i.e. it has gone beyond total points received in credit. [...](https://youtu.be/c9bcctkLV7A?t=145)
3. Create a new straddle at the current point.
	- Analyze chart to pick an appropriate strike and breakeven.
		- Analyze premiums in daily.
		- Find the percent move for daily beyond which the loss will start.
	- You may loose some points.
		- Sometime you may lose 500 points, sometime 800 points.
		- These losses my accumulate to 2000.
		- But if you close near the center of this straddle by the end of expiry, these losses won't matter much.
4. Go to step 1.

### 1.3. Monthly Position

For overnight safety also follow [[#Approach 3 Iron Fly for overnight safety]]

1. Wait for 0.75% to 1.25% move in one direction.
	- In points this is roughly 15% of the total received credit.
	- Configure alerts on TradingView.
2. Upon 0.75% to 1.25% move in one direction sell an extra option on the non tested side.
	- Sell an OTM Weekly option w/ 1 lot.
		- Pick an OTM strike which in points is far by 2.5% of the spot price.
		- This is 1000 points in Bank Nifty.
	- This helps in offseting losses on the tested side.
	- This also helps in covering the cost of shifting straddle. [...](https://youtu.be/A-zpeOlgtOY?t=1165)
	- By selling extra options on non tested you not only make money out of your comfort zone, you also get to shift straddle at low cost, and then return back to your comfort zone.
3. Regularly monitor the extra sold option for its premium.
	 - Configure alerts on MTM.
4. Exit the extra sold option when its premium goes below ₹15.
	1. Exit the exsiting short option.
	2. Sell another OTM Weekly option.
		- Pick an OTM strike which in points is far by 2.5% of the spot price.
		- This is 1000 points in Bank Nifty.
	3. Observe the payoff chart again. [...](https://youtu.be/A-zpeOlgtOY?t=2225)
		- Whenver you add a weekly option in a monthly strategy the payoff graph may look bad.
			- It is not able to match pricing and expiry.
			- It can be fixed by changing the payoff date.
5. Wait for 1.5% to 1.7% move from the middle in one direction.
	- Configure alerts on TradingView.
	- In points this is roughly 25% of the total received credit.
	- 140 points in Nifty.
	- 350-400 Points in Bank Nifty.
6. Exit from the current straddle when...
	- Premium of one side has substantially decreased and it can no more offset losses from the opposite side short. [...](https://youtu.be/c9bcctkLV7A?t=806)
	- The current MTM is at ₹1,500 to ₹2,000 loss (in Bank Nifty).
		- In first iteration, where you started from ₹0 MTM, exit upon ₹2,000 loss.
		- In subsequent iteration, say you are at  ₹6,200 MTM when you set up a new straddle, then exit as soon you go below ₹4,200 MTM profit.
	- The market has moved by 1.5% to 1.7% from the middle in one direction.
	- Spot price has breached breakeven range i.e. it has gone beyond total points received in credit. [...](https://youtu.be/c9bcctkLV7A?t=145)
7. Create a new well balanced straddle from the current point.
	- Analyze chart to pick proper strike and breakeven.
		- Analyze premiums in daily.
		- Find the percent move for daily beyond which the loss will start.
	- You may loose some points.
		- Sometime you may lose 500 points, sometime 800 points.
		- These losses my accumulate to 2000.
		- But if you close near the center of this straddle by the end of expiry, these losses won't matter much.
8. Stop shifting straddle when...
	- You reach 2 DTE.
		- You can't collect much credit when only 2 days are left for expiry.
9. Exit straddle when...
	- MTM loss goes over 2% to 2.5% of deployed margin.
	- MTM profit is over 4% of deployed margin (i.e. 4% [[Glossary#RoC]]).
	- You reach 2 DTE.
10. Go to step 3.
	- Try to bear some loss. Shifting too quickly drains away the max profit potential in situtation when market reverts.

[Backtesting of a trending move](https://youtu.be/A-zpeOlgtOY?t=1588)
- We safely managed a directional move of 4000 points.

[Backtesting of zig-zag moves](https://youtu.be/c9bcctkLV7A?t=276)
- This was an extreme scenario where managing straddles is very difficult.
- Market showed radical 1000 points move on both directions.

## Approach 3. Iron Fly for overnight safety
[...](https://youtu.be/A-zpeOlgtOY?t=1055)

If you need overnight safety from gap up/down of next opening, do as follows:

1. Create an Iron Fly @ 3:25 PM.
	- To cut cost you can buy hedges far OTM.
	- This will safeguard your overnight position.
2. Exit from Iron Fly in next session @ 9:20 AM.
	- It will cost you theta for that night.

## Approach 4. Neutralize delta
[...](https://youtu.be/A-zpeOlgtOY?t=996)

Delta beyond a certain point fail to balance the position.

##### Action: Neutralize delta

When you see delta of one side is losing its value, shift straddle at that point.

> Shifting a straddle means neutralizing delta.

## Approach 5. ITM strangles w/ delta balancing
[...](https://youtu.be/A-zpeOlgtOY?t=1201)

### 4.1 Non recommended yet popular technique

1. Wait for positional delta to breach 20Δ.
2. Rebalance delta.
	- You may end up with an inverted strangle.
	- Inverted strangle once formed, begins eating your max profit.
	- Inverted strangle ultimately turns into a red payoff chart.
3. Go to step 1.
	- With iterations a straddle becomes inverted strangle.

> This is not a recommended approach because you end up with an inverted strangle. You will eventually see a red payoff chart and become clueless about what to do next.

### 4.2. Recommended technique
[...](https://youtu.be/A-zpeOlgtOY?t=1321)

1. Wait for positional delta to breach 20Δ.
2. Rebalance delta.
	- You may end up with an inverted strangle.
	- Inverted strangle once formed, begins eating your max profit.
	- Inverted strangle ultimately turns into a red payoff chart.
3. If any of the option turns ITM then exit both options and create a strangle at those strikes.
	- You can bear the loss caused due to exiting ITM options.
4. Go to step 1.
	- With iterations a `straddle becomes an inverted strangle`.
	- You shift `inverted strangle to strangle`.
	- With iterations a `strangle becomes straddle`.

## Approach 6. Iron Fly upon breakeven breach
[...](https://www.youtube.com/watch?v=obXDTxHDjhk)

##### Action: Convert to Iron Fly and exit

1. Create an Iron Fly @ ATM strikes.
2. Exit Iron Fly when market breaches the breakeven.
3. Go to step 1.

## Approach 7. Shift straddle upon high VIX
[...](https://www.youtube.com/watch?v=KbFS8dciI24)

When market range has not shifted but volatility has increased then deploy a new straddle.

Ride with the rising VIX.

---

Reference:
- [18 Jul 2020 | Straddle Basics w/ Management | ThetaGainers](https://www.youtube.com/watch?v=H8z3Es-Rgso)
- [19 Nov 2021 | All adjustments | ThetaGainers](https://www.youtube.com/watch?v=A-zpeOlgtOY)
- [27 Nov 2021 | Zig-Zag Move Adjustment | ThetaGainers](https://www.youtube.com/watch?v=c9bcctkLV7A)
- [04 Oct 2013 | Iron Fly vs Short Straddle | TastyTrade](https://www.youtube.com/watch?v=YcQcpZ3EmCE)
