Short Strangle w/o Hedge

## Warning
[...](https://youtu.be/6VP7UuoN7Ho?t=307)

- Never deploy any strategy without hedges.
- Never short a 45 DTE naked strangle.
- In high VIX environment 45 DTE is bad even for strangles w/ hedges (i.e. Iron Condors).
- Naked strangles should only be deployed near expiry.
- Strangle's failure comes before straddle's failure.

# Step 1. Wait for the setup
[...](https://youtu.be/fZe6ClmdbZg?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=476)

1. High IVP
	- IVP > 23% in Nifty
	- IVP > 30% in Bank Nifty
	- With IVP gets better premiums.
	- High premiums gives better breakeven range.
	- Generally VIX shoots up when market falls. This is ideally the best time to enter strangle but since there is lot of fear only few do it. [...](https://youtu.be/fZe6ClmdbZg?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=541)

## Deploying far OTM strangles
[...](https://youtu.be/MIF7oq2J9Pw?t=145)

- There are not much benefits of deploying far OTM strangles.
- If there is a gap down in Bank Nifty then your ₹100 put will go to ₹500 but ₹100 call cannot go to ₹0. Call won't be able to offset losses from put.
- To prevent losses you will have to have a bearish view.
	- Set up a Bearish Credit Call Spread.
	- The spread width will be your max loss.

## Deploying near OTM strangles
[...](https://youtu.be/MIF7oq2J9Pw?t=334)

- The benefit is high premium.
- High credit (Say ₹200-₹250 in Bank Nifty on each side) results in high breakeven range (500 points).
- If there is a small gap up/down in Bank Nifty then both sides compensate each other well.

# Step 2. Deploy

- Choosing the underlying [...](https://youtu.be/fZe6ClmdbZg?t=1816)
	- New traders should prefer Nifty.
	- Experienced traders should prefer Bank Nifty for higher profit at higher risk.
- For `weekly`, deploy on Thursday @ 3 PM w/ 7 DTE.
	- ThetaGainer deploys weekly strangle on Wednesday @ 3 PM
	- ThetaGainer recommends deploying weekly strangles on Monday/Tuesday @ 12 PM and then follow the market using chart.
	- Its only for experienced traders. [...](https://youtu.be/fZe6ClmdbZg?t=947)
	- Strangles creates problem to weekly traders due to delta. [...](https://youtu.be/fZe6ClmdbZg?t=965)
	- New traders should do monthly strangles for first 6 months.
- For `monthly`, deploy w/ 45 DTE [...](https://youtu.be/fZe6ClmdbZg?t=637)
	- Strangles are not reliable for monthly strategy.
	- Many don't prefer in Indian market.
	- Its better for new traders.
	- For monthly strangles, don't try to collect high credit at the time of deployment. [...](https://youtu.be/fZe6ClmdbZg?t=861)
		- Try to collect small premium and then increase your collection by slowly increasing the lot size and/or premium.
		- Adjustment in monthly strangles is inevitable. If you start with a high credit in the beginning, with more adjustment you will eventually have a small breakeven range to ride the market. Instead start small and collect by doing more adjustments.
		- Note that whenever you adjust a strangle, it increases your credit. So you end up earning more than what you had originally targetted. [...](https://youtu.be/fZe6ClmdbZg?t=821)
			- Start with 30 premium.
			- Then book profits in 30 premium.
			- The try to book profits with 25 premium.
		- Try to maintain high range while having a high Probability of Profit.

## Position Size

[Budgeting strangles in Nifty | ThetaGainers](https://youtu.be/fZe6ClmdbZg?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=307)
- ₹1,60,000 Lakhs for 1 lot strangle.
- If you have a capital of ₹10,00,000, then do not deploy more than ₹6,00,000 capital.
- With ₹6,00,000 lakhs one can create 6 lots.
- Target 4% RoC
- 1 lot strangle generates ₹2,000 returns per week.
- 6 lot strangle would generate ₹2,000 x 6 => ₹12,000/week => ₹48,000/month

[Selecting monthly vs weekly strangles | ThetaGainers](https://youtu.be/fZe6ClmdbZg?t=695)

> Note that whenever you adjust a strangle, it increases your credit. So you end up earning more than what you had originally targetted. [...](https://youtu.be/fZe6ClmdbZg?t=821)

[Decide earning target | ThetaGainers](https://youtu.be/fZe6ClmdbZg?t=1910)
- How much you want to earn if your capital is ₹4,00,000?
	- 4% Monthly RoI => ₹4,00,000 x 4% => ₹16,000
- How will 16,000 come? [...](https://youtu.be/fZe6ClmdbZg?t=1926)
	- If you earn 24 points in a week.
	- In a month you can do 24 x 4 points.
	- Create a weekly strangle in Nifty by selling a ₹12 tstrike call & put.
	- Create a weekly strangle in Bank Nifty by selling a ₹45 tstrike call & put.
	- Create a monthly strangle in Nifty by selling a ₹30 tstrike call & put.
	- Create a monthly strangle in Bank Nifty by selling a ₹70 to ₹90 tstrike call & put.

# Step 3. Adjust
[...](https://youtu.be/ZnSVMv7jgTc?t=169) | [...](https://youtu.be/fZe6ClmdbZg?t=1119)

- Never adjust after the spot price has moved beyond the short strikes.
- Note that whenever you adjust a strangle, it increases your credit. So you end up earning more than what you had originally targetted. [...](https://youtu.be/fZe6ClmdbZg?t=821)
- Strangles creates problem to weekly traders due to delta. [...](https://youtu.be/fZe6ClmdbZg?t=965)
	- As your short strike approaches ATM, delta sharply increases.
	- Suppose you are short CE @ 18500, short PE @ 17500 and spot price has reached 18300 then you must address this ASAP.
	- And if you are near expiry gamma further accelerates delta's effect on premium.

## Approach 1.  Rebalance delta till Straddle | Weekly
[...](https://www.youtube.com/watch?v=OUVmA9_9bnM)

1. Create a strangle by selling 20Δ to 22Δ call & put.
	- `Or` sell 3% OTM call & put.
2. Deploy strangle only when...
	1. B/E > 2.75% of the spot price for DTE <= 2.
		- `Or` B/E > 3.75% of the spot price for DTE > 2.
	2. `And` B/E range fully covers/engulfs the expected move.
		- Calculate expected average move for the day using one of the following formulas:
			- `Expected % Move` = `IV` / √(365/3)
			- `Expected % Move` = `IV` * √(3/365)
			- [[Option Greeks#Calculating Expected Move or Range using IV]]
		- The use the expected move to calculate the upper and lower range that price can touch.
3. Monitor premiums of short call & short put.
	- Wait for one of the premiums to drop by 50%.
4. Exit the leg whose premium has dropped by 50% from the value that was there in delta neutral state.
	- This means, as you iterate through the steps, track premium to become half from its value that was there at the time you adjusted it to delta neutral state.
	- Don't compare 50% drop from the initial price when you added the contract.
5. Exit the other leg `when`...
	- `Either` other leg's delta (or positional delta) is ≥ 45Δ.
		- Do not sell ITM contracts by choosing 50+ delta values.
		- If opstra shows 0 or 100 as delta then refer options chain and check what are the delta values of the upper and lower strike price.
		- Gauge delta using this upper and lower values.
	- `Or` other leg's delta (or positional delta) is ≥ 40Δ.
		- `And` current price after adjustment would still be towards one end of the breakeven range.
6. `If` both legs are closed `then` create a fresh straddle like so:
	- `Either` create a strangle by selling 25Δ call & put `when` DTE <= 2.
	- `Or` create a strangle by selling 20Δ call & put `when` DTE > 2.
7. `If` you created a new strangle after exiting both the legs `then` go to step 2.
8. Sell another option with type that of above exited leg and `delta lower/matching the positional delta` after exiting.
		- If opstra shows 0 or 100 as delta then refer options chain and check what are the delta values of the upper and lower strike price.
		- Gauge delta using this upper and lower values.
		- You may even match the premium of the other option.
9. Stop adjustments `when`...
	- Strangle becomes straddle.
		- Now follow [[Short Strangle Playbook#Step 3 Adjust]]
10. Go to step 3.

[Strong trend | 01 Jan 2021 - 14 Jan 2021](https://youtu.be/OUVmA9_9bnM?t=158)
- Managed 7% up move.

## Approach 2. Rebalance delta till Iron Fly | Weekly
[...](https://youtu.be/ZnSVMv7jgTc?t=204) | [...](https://youtu.be/fZe6ClmdbZg?t=1126)

When you have deployed a strangle, your view is that market should stay neutral and volatiltiy should also stay down.
	- When volatility increases, main problem comes when premium stops dropping and market starts moving.
	- Essentially this movement itself is your delta.
	- To address this problem you should try to neutralize this delta to 0.
	- Neutralizing delta means balancing the position.
	- When premium of one side substantially decreases in relation to the other side then it can no more offset otherside losses.
	- Delta of one side becomes faster than the other side's delta.
	- This means the rate at which one side's premium decreases is greater than the rate at which the other side's premium increases.

##### Action: Roll shorts to match delta

1. Monitor delta of both strikes in every 1 hour candle close.
2. Wait for one of the short option's delta to go far below the other option's delta.
	- When you reach this point the delta of one side is faster than the other side delta.
	- So the rate at which one side premium decreases is greater than the rate at which the other side premium increases.
	- Due to delta imbalance the gains of one side can't compensate for the other side's losses.
	- At this stage you must rebalance this strangle.
3. Adjust the untested side like so:
	- `If` short put delta goes far below short call delta `then`
		- Exit the short put.
		- Sell a new put with delta that is slightly lower than the short call's delta.
		- Try to match delta by 75% only.
		- Do not select put strike above spot price.
		- Do not sell ITM put. Convert to straddle instead.
	- `Else if` short call delta goes far below short put delta `then`
		- Exit the short call.
		- Sell a new call with delta that of current short put.
		- Do not select call strike below spot price.
		- Do not go ITM. Convert to straddle instead.
	- As and when we do adjustments the breakeven range will reduce.
4. If one of the option goes ITM then convert this strangle to straddle.
	- Do not go ITM and make it an inverted strangle. [...](https://youtu.be/fZe6ClmdbZg?t=1511)
		- You can still risk this as long as your intrinsic value, i.e. the inverted strangle width, is lower than the received credit. [...](https://youtu.be/fZe6ClmdbZg?t=1565)
		- Not recommended for new traders.
		- [Example of Inverted Strangle](https://youtu.be/fZe6ClmdbZg?&t=3315)
	- Going ITM results in problem not due to delta but when market reverses. [...](https://youtu.be/ZnSVMv7jgTc?t=1789)
5. Stop adjustment when...
	- Strangle becomes straddle.
6. If strangle becomes straddle then convert it to an  `Iron Fly`.
	- Once we reach `Iron Fly` position and leave it.
7. Exit when...
	- Upon reaching straddle the premium collected through final straddle increases by 12%.
		- i.e. When ₹300 premium in Nifty becomes ₹340. [...](https://youtu.be/fZe6ClmdbZg?t=1448)
	- MTM loss exceeds 2% of deployed margin.
	- You are risking an inverted strangle and see a slight profit.
8. Go to step 1.

## Approach 3. Rebalance premium till Iron Fly | Weekly
[...](https://youtu.be/ZnSVMv7jgTc?t=711)

##### Action: Roll shorts to match price/premiums

1. Create a delta neutral strangle like so:
	- A weekly strangle in Nifty can be created by selling a ₹12 tstrike call & put.
	- A weekly strangle in Bank Nifty can be created by selling a ₹45 tstrike call & put.
	- A monthly strangle in Nifty can be created by selling a ₹30 tstrike call & put.
	- A monthly strangle in Bank Nifty can be created by selling a ₹70 to ₹90 tstrike call & put.
2. Monitor premiums of both sides in every 30 min candle close.
3. Wait for one of the short option's premium to go far below the other option's premium.
	- Due to premium imbalance the gains of one side can't compensate for the other side's losses.
	- At this stage you must rebalance this strangle.
4. Adjust the untested side like so:
	- `If` short put premium goes below 50% of short call premium `then`
		- Exit the short put.
		- Sell a new put with a premium slightly lower than the current short call.
			- Generally when market is trending up the put side IV is high relative to call side IV.
			- So if market comes down fast, the VIX will go up due to fear.
			- The put side premium will react faster than the call side premium.
		- Do not select put strike above spot price.
		- Do not go ITM. Convert to straddle instead.
	- `Else if` short call premium goes below 50% of short put premium `then`
		- Exit the short call.
		- Sell a new call with a premium as that of current short put.
		- Do not select call strike below spot price.
		- Do not go ITM. Convert to straddle instead.
	- As and when we do adj ustments the breakeven range will reduce.
5. If one of the option goes ITM then convert this strangle to straddle.
	- Do not go ITM and make it an inverted strangle. [...](https://youtu.be/fZe6ClmdbZg?t=1511)
		- You can still risk this as long as your intrinsic value, i.e. the inverted strangle width, is lower than the received credit. [...](https://youtu.be/fZe6ClmdbZg?t=1565)
		- Not recommended for new traders.
		- [Example of Inverted Strangle](https://youtu.be/fZe6ClmdbZg?&t=3315)
	- Going ITM results in problem not due to delta but when market reverses. [...](https://youtu.be/ZnSVMv7jgTc?t=1789)
6. Stop adjustment when...
	- Strangle becomes straddle.
7. If strangle becomes straddle then convert it to an  `Iron Fly`.
	- Once we reach `Iron Fly` leave it.
	- The Iron Fly hedges is what prevents bigger loss from happening. [...](https://youtu.be/ZnSVMv7jgTc?t=1702)
8. Exit when...
	- Upon reaching straddle the premium collected through final straddle increases by 12%.
		- i.e. When ₹300 premium in Nifty becomes ₹340. [...](https://youtu.be/fZe6ClmdbZg?t=1448)
	- MTM loss exceeds 2% of deployed margin.
1. Go to step 2.

Backtesting:
- [01 Oct 2020 | A weekly strangle in a trending move](https://youtu.be/ZnSVMv7jgTc?t=1131)
	- We managed a directional move of 600 points in a 300 point wide strangle with a small loss of ₹1,515.
	- The small losses are very easy to cover.
	- The loss would have been ₹7,972 had we not converted strangle into an Iron Fly. [...](https://youtu.be/ZnSVMv7jgTc?t=1702)
- [09 Sep 2021 | 4 weekly strangles in a trending move](https://youtu.be/fZe6ClmdbZg?t=2062)

## Approach 4. Shift strangle upon huge overnight move
[...](https://youtu.be/6VP7UuoN7Ho?t=684)

Your goal is to recover losses due to a huge move in overnight strangle by...
1. Shifting option inwards on the non tested side to match the non tested premium.
2. Shifting option outwards on the tested side.

## Approach 5.  Sell extra option upon new swing high/lows
[...](https://youtu.be/MIF7oq2J9Pw?t=712)

### Scenario 1. As market makes higher-highs/lows

##### Action: Sell an extra put

1. Wait for market to break overhead resistance while forming higher-highs/lows.
2. Sell an extra put w/ 1 lot from bottom if IV is not high.
3. If you want safety from gap-down then covert naked short call into a bear credit spread.
	- Buy a far OTM put below short put.
	- The spread width will be the max loss.
4. If market follows up and forms new higher-highs/lows go to step 2.

### Scenario 2. As market makes lower-highs/lows

##### Action: Sell an extra call

1. Wait for market to break underlying support while forming lower-highs/lows.
2. Sell an extra call w/ 1 lot from top if IV is not high.
3. If you want safety from gap-up then covert naked short put into a bull credit spread.
	- Buy a far OTM call above short call.
	- The spread width will be the max loss.
4. If market follows up and forms new lower-highs/lows go to step 2.

# Step 4. Exit
[...](https://youtu.be/fZe6ClmdbZg?t=444)

- Exit when M2M profit goes above 50% of Max Profit.
	- Move on to next strangle instead of chasing profits in an existing strangle.
	- Run with time.
- Exit when MTM loss exceeds 2% of deployed margin.
- Exit ASAP if an adjust lead to an inverted strangle and still you see a slight profit.

---

Reference:
- [04 May 2020 | Strangle vs Straddle Adjustments | ThetaGainers](https://youtu.be/MIF7oq2J9Pw?t=77)
- [04 June 2020 | Recvering losses in overnight strangles | ThetaGainers](https://youtu.be/6VP7UuoN7Ho?t=684)
- [22 June 2020 | Q&A on strangles | ThetaGainers - Premium](https://youtu.be/zMwFaIqWYhs?t=4756)
- [01 Nov 2020 | Strangle adjustments | ThetaGainers](https://www.youtube.com/watch?v=ZnSVMv7jgTc)
- [12 Nov 2021 | All about strangles | ThetaGainers](https://www.youtube.com/watch?v=fZe6ClmdbZg)
	- [Danger with Inverted Strangles](https://youtu.be/fZe6ClmdbZg?t=1703)
	- [Example of Inverted Strangle](https://youtu.be/fZe6ClmdbZg?&t=3315)
