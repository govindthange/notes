Straddle works better than Strangles.
- `If` you create a strangle that has
	1. Same premium as that of corresponding straddle.
	2. Same breakeven as that of straddle.
- `And` there is a directional move
- `Then` Strangle may show some loss whereas straddle may retain its profit or at least show no losses.

Straddles are best when you are able to collect good premiums and you can manage position actively.

# Step 1. Wait for the setup
[...](https://www.youtube.com/watch?v=H8z3Es-Rgso)

1. High VIX evironment.
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
- For `weekly`, deploy straddle like so:
	- Enter trade on Wednesday @ 10:20 AM or 01:20 PM. You may even enter on Thursday @ 3:15 PM.
		- In Nifty you can collect ₹200 on each side of call & put.
		- In Bank Nifty you can collect ₹400 on each side of call & put.
	- Exit trade next week on Wednesday @ 3:00 PM or by Thursday @ 10:20 AM.
- For `monthly`, deploy straddle like so:
	- Have 45 DTE strategy.
	- Enter trade on the 3rd week, Wednesday @ 10:20 AM of current month.
	- Exit trade on last thursday of next month.

> In monthly trades, for first 10 days use future spot price for picking strikes. Later towards the end of month you can use normal spot price for picking strikes. [...](https://youtu.be/A-zpeOlgtOY?t=1697)

## Iron Fly for overnight safety
[...](https://youtu.be/A-zpeOlgtOY?t=1055)

If you need overnight safety from gap up/down of next opening, do as follows:

1. Create an Iron Fly @ 3:25 PM.
	- To cut cost you can buy hedges far OTM instead of breakeven.
	- This will safeguard your overnight position.
2. Exit from Iron Fly in next session @ 9:20 AM.
	- It will cost you theta for that night.

# Step 4. Adjust

The very meaning of straddle is that you have deployed a strategy to create balance. [...](https://youtu.be/c9bcctkLV7A?t=1481)
- This means whenever market extends towards one side, the other side's profit must offset the losses from tested side.
- When you reach a point where your `straddle shows loss` then it means you have reached a point of imbalance.
	- Delta of one side has become faster than the other side's delta.
	- So the rate at which one side's premium decreases is greater than the rate at which the other side's premium increases.
	- You must exit this straddle to create a new one.
- When you reach a point where your `straddle shows profit` and then it `undergoes imbalance` then you may not be able to catch it from the surface.
	- You will not directly see a loss.
	- First your profit will erode and then losses will appear.
	- To prevent this only track newly added premiums on both sides and check whether the 2 together results in a loss.
	- When premium of one side substantially decreases in relation to the other side then it can no more offset other side's loss. [...](https://youtu.be/c9bcctkLV7A?t=806)
		- Whenever the 2 premiums reaches 1:3+ ratio then exit the straddle. [...](https://youtu.be/c9bcctkLV7A?t=1016)
			- Wait for the tested side short premium to go over 3 times higher than the non tested side short premium and then exit.
			- When you reach 1:3+ that means you are coming near the edges of your straddle.
			- Exiting upon 1:3 ratio is a best way to prevent further losses.
		- Do not let your current profit erode any further.
		- There is no need to further wait and realize loss.
		- You have reached a point where you create a fresh straddle where both sides are well balanced.

## Approach 1. Shift straddle upon threshold breach | Weekly

The entire logic behind straddle is collection of high premium. As long as you are in the center there is no reason to fear.

> Compared to Iron Fly where we wait until breach of breakevens and then react. In naked straddles we don't have hedges and therefore we must react faster.

### 1.1. Intraday in weekly position
[...](https://youtu.be/A-zpeOlgtOY?t=868)

1. Wait for `25% directional move` of the total breakeven range.
	- This is 50% of breakeven on one side.
	- If you have 440 points on each side, then wait for a 110 point move.
	- Being an intraday trade, monitor it very closely.
2. `Exit from current straddle` when...
	- There is 25% directional move of the total breakeven range.
	- Spot price has breached breakeven range i.e. it has gone beyond total points received in credit. [...](https://youtu.be/c9bcctkLV7A?t=145)
3. `Create a new straddle` at the current point.
4. Go to step 1.

### 1.2. Weekly Position

> When you are conservative and concerned about black swan event then follow [[#Iron Fly for overnight safety]]

1. Define a `shifting threshold` for us to react when price breaches it. [...](https://youtu.be/A-zpeOlgtOY?t=1845)
	- The threshold signifies an `average movement range` of the underlying. [...](https://youtu.be/A-zpeOlgtOY?t=511)
		- Find IV of the underlying.
		- Calculate expected average move for the day using one of the following formulas:
			- `Expected % Move` = `IV` / √365
			- `Expected % Move` = `IV` * √(1/365)
			- [[Option Greeks#Calculating Expected Move or Range using IV]]
		- Bank Nifty's average daily movement range is 1.5% to 1.7% of the spot price. [...](https://youtu.be/A-zpeOlgtOY?t=532)
		- If Bank Nifty moves by 400 points in a given day then it means something worth noticing has happened which warrants a reaction.
	- In points this is...
		- 25% of the total received credit.
		- 140 points in Nifty.
		- 350-400 Points in Bank Nifty.
	- Configure alerts on TradingView.
2. Wait for price to `completely breach the shifting threshold`.
	- Await `1.5% to 1.7% move` from the middle in one direction.
3. `Exit from current straddle` when...
	- When price completely breaches the shifting threshold.
	- `Or` spot price has breached breakeven range i.e. it has gone beyond total points received in credit. [...](https://youtu.be/c9bcctkLV7A?t=145)
	- `Or` premium of one side in relation to the other side has substantially decreased (3:1 ratio) and it can no more offset losses from the opposite side short. [...](https://youtu.be/c9bcctkLV7A?t=806)
4. `Create a new straddle` at the current point.
	- Shift it such that the breakevens lies beyond the average movement range of the underlying. [...](https://youtu.be/A-zpeOlgtOY?t=511)
	- Analyze chart to pick an appropriate strike and breakeven.
		- Analyze premiums in daily.
		- Find the percent move for daily beyond which the loss will start.
	- You may loose some points.
		- Sometime you may lose 500 points, sometime 800 points.
		- These losses my accumulate to 2000.
		- But if you close near the center of this straddle by the end of expiry, these losses won't matter much.
5. Go to step 2.

## Approach 2. Shift straddle upon `staged` threshold breach | Monthly

> When you are conservative and concerned about black swan event then follow [[#Iron Fly for overnight safety]]

#### Stage 1. Threshold breach by 50%

1. Define a `shifting threshold` for us to react when price breaches it. [...](https://youtu.be/A-zpeOlgtOY?t=1845)
	- The threshold signifies an `average daily movement range` of the underlying. [...](https://youtu.be/A-zpeOlgtOY?t=511)
		- Find IV of the underlying.
		- Calculate expected average move for the day using one of the following formulas:
			- `Expected % Move` = `IV` / √365
			- `Expected % Move` = `IV` * √(1/365)
			- [[Option Greeks#Calculating Expected Move or Range using IV]]
		- Bank Nifty's average daily movement range is 1.5% to 1.7% of the spot price. [...](https://youtu.be/A-zpeOlgtOY?t=532)
		- If Bank Nifty moves by 400 points in a given day then it means something worth noticing has happened which warrants a reaction..
	- In points this is...
		- 25% of the total received credit.
		- 140 points in Nifty.
		- 350-400 Points in Bank Nifty.
	- Configure alerts on TradingView.
2. Wait for price to `cross 50% of the shifting threshold` defined above.
	- Await `0.6% to 0.75% move` in one direction. [...](https://youtu.be/A-zpeOlgtOY?t=1845)
	- In points this is roughly 15% of the total received credit.
3. Upon 50% breach of shifting threshold `sell an extra option` on the non tested side. [...](https://youtu.be/A-zpeOlgtOY?t=1886)
	- `Sell an OTM Weekly option` w/ 1 lot.
		- Pick an OTM strike which in points is `far by 2.75%` of the spot price.
		- This is 1000 points in Bank Nifty.
	- This helps in offseting losses on the tested side.
	- This also helps in covering the cost of shifting straddle. [...](https://youtu.be/A-zpeOlgtOY?t=1165)
	- By selling extra options on non tested you not only make money out of your comfort zone, you also get to shift straddle at low cost, and then return back to your comfort zone.
4. Regularly monitor that extra sold option's premium.
	 - Configure alerts on MTM.
5. Exit that extra sold option when its premium goes below ₹15. [...](https://youtu.be/A-zpeOlgtOY?t=1955)
	1. Exit the exsiting short option.
	2. Sell another OTM Weekly option.
		- Pick an OTM strike which in points is far by 2.75% of the spot price.
		- This is 1000 points in Bank Nifty.
	3. Observe the payoff chart again. [...](https://youtu.be/A-zpeOlgtOY?t=2225)
		- Whenver you add a weekly option in a monthly strategy the payoff graph may look bad.
			- It is not able to match pricing and expiry.
			- It can be fixed by changing the payoff date.
			- Aloways keep payoff date right.

#### Stage 2. Threshold breach by 100%

6. Wait for price to `completely breach the shifting threshold`.
	- Await `1.5% to 1.7% move` from the middle in one direction.
7. Monitor P/L of the newly created straddle.
	- When your straddle is in profit that means your straddle is working.
	- Only focus on the P/L of recently shorted CE & PE option combination.
	- Ignore all other transactions related to previous straddle/s and their adjustments.
	- Ignore the overall P/L shown in opstra. Use calculator to calculate P/L of the new combo.
8. `Exit from current straddle` when...
	- When spot price completely `breaches the shifting threshold`.
	- `Or` spot price `breaches the breakeven range` i.e. it has gone beyond total points received in credit. [...](https://youtu.be/c9bcctkLV7A?t=145)
	- `Or` ratio of the `two premiums goes beyond 1:3+` and they can no more offset each other's losses. [...](https://youtu.be/c9bcctkLV7A?t=806)
	- `Or` the most recent straddle pair incurs ₹1,500 to ₹2,000 loss (in Bank Nifty).
		- You are not concerned with gains/losses of straddle in previous iterations. Focus on P/L of newer straddle only.
		- In first iteration, where you started from ₹0 MTM, exit upon ₹2,000 loss.
		- In subsequent iteration, say you are at  ₹6,200 MTM when you set up a new straddle, then exit as soon you go below ₹4,200 MTM profit.
9. `Create a new straddle` from the current point.
	1. Analyze chart to pick a proper strike and breakeven.
		- Analyze premiums in daily.
		- Find the percent move for daily beyond which the loss will start.
	2. First exit from that extra weekly option you sold to offset losses in previously created straddle.
	3. Create a well balanced straddle.
		- You may loose some points.
		- You may loose 500 points to 800 points.
		- These losses my accumulate to 2000.
		- But if you close near the center of this straddle by the end of expiry, these losses won't matter much.
10. `Stop shifting` straddle when...
	- You reach 2 DTE.
		- You can't collect much credit when only 2 days are left for expiry.
11. `Exit straddle` when...
	- MTM loss goes over 2% to 2.5% of deployed margin.
	- MTM profit is over 4% of the deployed margin (i.e. 4% [[Glossary#RoC]]).
	- You reach 2 DTE.
12. Go to step 2.
	- Try to bear some loss. Shifting too quickly drains away the max profit potential in situtation when market reverts.

[Strong Trend | 01 Oct 2021 - 28 Oct 2021](https://youtu.be/A-zpeOlgtOY?t=1588)
- We safely managed a trending directional move of 4500 points in Bank Nifty.

[Zig-Zag Move | 1 Sep 2021 - 30 Sep 2021](https://youtu.be/c9bcctkLV7A?t=276)
- This was a challenging scenario where managing straddles was extremely difficult.
- The move had highest probability of a straddle failing.
- Since the straddle collected ₹1,000 as premium it easily managed first 3 moves.
	- First move was 937 points down in 4 days 3 hours.
	- Second move was 663 points up in 1 day.
	- Third move was 540 points down 4 days 6 hour.
- Market showed radical 1000 points move on both directions. [...](https://youtu.be/c9bcctkLV7A?t=688)
	- Forth move was 1795 move in 3 days. [...](https://youtu.be/c9bcctkLV7A?t=736)
	- Fifth move was 1615 points down in 5 days.
	- Sixth move was 1831 points up in 5 days 18 hours.
	- Final move was 1016 points down in 2 days 4 hours.

## Approach 3. Shift straddle upon high VIX
[...](https://www.youtube.com/watch?v=KbFS8dciI24)

When market range has not shifted but volatility has increased then shift straddle by exiting the current straddle and creating a new straddle.

Ride with the rising VIX.

## Approach 4. Shift straddle upon delta imbalance
[...](https://youtu.be/A-zpeOlgtOY?t=996)

> Shifting a straddle means neutralizing delta.

This is not a very feasible adjustment technique because you end up with an inverted strangle. [...](https://youtu.be/A-zpeOlgtOY?t=1276)

##### Action: Neutralize delta
[...](https://youtu.be/A-zpeOlgtOY?t=1213)

1. Monitor delta of both strikes in every 1 hour candle close.
	- Delta beyond a certain point fail to balance the position.
	- When you see delta of one side is losing its value, shift straddle at that point.
2. Wait for short option's delta mismatch to go beyond 20Δ.
	- You deploy at straddle with 50Δ put and call options.
		- 50Δ means you are at the center.
	- Wait for the delta of call or put option move by +/- 20Δ.
		- 50Δ option becomes 70Δ then that means call price has increased.
		- or 50Δ option becomes 30Δ.
	- When you reach this point the delta of one side is faster than the other side delta.
	- So the rate at which one side premium decreases is greater than the rate at which the other side premium increases.
	- Due to delta imbalance the gains of one side can't compensate for the other side's losses.
	- At this stage you must rebalance this strangle.
3. Upon mismatch, you exit from the lower delta option and buy another option with delta matching that of other higher delta. [...](https://youtu.be/A-zpeOlgtOY?t=1257)

## Approach 5. ITM strangles w/ delta balancing
[...](https://youtu.be/A-zpeOlgtOY?t=1201)

### 4.1. Straddle -> Inverted Strangle (Non recommended)

1. Wait for positional delta to breach 20Δ.
2. Rebalance delta.
	- You may end up with an inverted strangle.
	- Inverted strangle once formed, begins eating your max profit.
	- Inverted strangle ultimately turns into a red payoff chart.
3. Go to step 1.
	- With iterations a straddle becomes inverted strangle.

> This is not a recommended approach because you end up with an inverted strangle. You will eventually see a red payoff chart and become clueless about what to do next.

### 4.2. Straddle -> Inverted Strangle -> Strangle -> Straddle (Recommended)
[...](https://youtu.be/A-zpeOlgtOY?t=1321)

1. Wait for positional delta to breach 20Δ.
2. Rebalance delta.
	- You may end up with an inverted strangle.
	- Inverted strangle once formed, begins eating your max profit.
	- Inverted strangle ultimately turns into a red payoff chart.
3. If any of the option turns ITM then exit both options and `create a strangle` at those strikes.
	- You can bear the loss caused due to exiting ITM options.
4. Go to step 1.
	- With iterations a `straddle becomes an inverted strangle`.
	- You shift `inverted strangle to strangle`.
	- With iterations a `strangle becomes straddle`.

## Approach 6.  Adjust using TA
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

## Approach 7. Iron Fly upon breakeven breach
[...](https://www.youtube.com/watch?v=obXDTxHDjhk)

##### Action: Convert to Iron Fly and exit

1. Create an Iron Fly @ ATM strikes.
2. Exit Iron Fly when market breaches the breakeven.
3. Go to step 1.

---

Reference:
- [04 Oct 2013 | Iron Fly vs Short Straddle | TastyTrade](https://www.youtube.com/watch?v=YcQcpZ3EmCE)
- [18 Jul 2020 | Straddle basics w/ adjustments | ThetaGainers](https://www.youtube.com/watch?v=H8z3Es-Rgso)
- [19 Nov 2021 | All about adjustments | ThetaGainers](https://www.youtube.com/watch?v=A-zpeOlgtOY)
- [27 Nov 2021 | Adjustment in large zig-zag moves | ThetaGainers](https://www.youtube.com/watch?v=c9bcctkLV7A)
