[...](https://www.youtube.com/watch?v=93IgLvYIONo&list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&index=3) | [...](https://www.youtube.com/watch?v=pDT8R6AxYTs&list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&index=5)

`Double Diagonal Calendar Spread` is formed by combining 1 `Diagonal Calendar Spreads` (DCS) on the call side and another DCS on the put side.

- If you make Double DCS debit then it will work better in directional moves i.e. deploy it when VIX is low.
- Double DCS works better when `VIX is between 17 to 25`.
- Double DCS is a better `substitute when Iron Condor fails`.
- Double DCS is best suited `for weekly option selling`.
- Double DCS is not suited for monthly option selling as you end up too much for the back month hedge.
- References:
	- [Rules for calendar/diagonal spreads](https://www.thestreet.com/investing/options/15-rules-for-calendardiagonal-spreads-12003637)

# Step 1. Find range
[[Strategy Builder Playbook#Step 1 Find range]]

# Step 2. Cover range
[[Strategy Builder Playbook#Step 2 Cover range]]

 Note that max profit will be at the short option strike price.

# Step 3. Define risk

Hedge naked strangle with the credit received from selling a Double DCS.

1. Define risk with 1:1 Risk/Reward ratio.
	- If you receive ₹10,000 in credit, then only debit ₹10,000 for hedging.
	- Its fine to pay slightly extra.
2. Hedge the short position by buying option with the same lot size.
	- Skip the front week expiry (i.e. expiry of the option used for strangle) and go to the subsequent week expiry (aka back week expiry).
	- Pick the strike corresponding to the credit received from the sold options.
		- You may pay slightly extra because you will close this in the front week expiry.
		- It is best to pick strike which is atleast ₹10 higher than the credit received.
	- The profit in the middle of the payoff chart should be at least 1.5% of the margin.
	- By buying PE & CE options will increase breakeven range.

# Step 4. Deploy strategy

- Deploy strategy on Wednesday @ 10:30 AM or by Thursday @ 01:20 PM.
- Exit strategy next week on Wednesday @ 1:20 PM or by Thursday @ 9:20 AM.

## Position Size

1. Look at the blue t+0 line in opstra.
2. Move your cursor over the t+0 line at the lowermost breakeven point.
3. Note down the loss.
4. If this `loss` is ≤ `2% of total trading capital` only then deploy the strategy.
5. If `loss` > `2% of the total trading capital` then skip and wait for the next opportunity.

# Step 5. Monitor position
[[Strategy Builder Playbook#Step 4 Monitor position]]

# Step 6. Adjust position
[...](https://youtu.be/93IgLvYIONo?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=317)

- Adjust trade @ 01:20 PM by either balancing premium or delta.
- When market trends up/down the long calendar option of the back week offsets loss from the front week and vice versa. But this balance only happens if you keep receiving credit from the other side of the option.
- By periodically balancing the shorted position prevents loss because back week's calendar delta dominates front week's option delta as both have same lot size.

## Approach 1. Increase hedges
[...](https://youtu.be/pDT8R6AxYTs?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=1188)

Use this approach when market breaks a critical support/resistance and you are fearful about potential losses.

- When market starts to trend up then buy a front week call option at a strike matching the strike of the back week calendar call option.
	- This will make the blue t+0 line in opstra fully debit.
	- This will beautifully sustain the position if the market suddenly rallies up.
- When market starts to trend down then buy a front week put option at a strike matching the strike of the back week calendar put option.
	- This strategy works best in the falling market because market falls quickly.
	- It increases your breakeven range.

## Approach 2. Balance to neutralize premium
[ThetaGainers](https://www.youtube.com/watch?v=93IgLvYIONo) | [InvestaBull](https://www.youtube.com/watch?v=NhEBTmLzrgw) | [ManekAgicha](https://www.youtube.com/watch?v=ExdQGVC2GBQ)

Balance position by matching the call side option premium with the put side option premium.

##### Setup

- VIX should be between 13 to 16. You benefit from rising VIX.

##### Assumption

A strangle on `Nifty` was created like so:
- On the `front week` expiry `short` a `₹25 premium` OTM call & put.
- On the `back week` expiry `long` a call and a put strikes that is `near or slightly above the premium` of the call & put on the front week expiry.
- Deploy strategy on `Wednesday @ 10:30 AM` considering the front week expiry is on next week's Thursday.
	- Essentially you pick a `8 DTE front week expiry`

##### Adjustment

1. Monitor position at regular intervals.
	- Track on every 30 min candle close. <== InvestaBull Approach
	- Track every morning at 10:30 AM. <== ThetaGainers Approach
	- No need to do adjustment when price is within the green range of payoff chart i.e. under the green tent. <== ManekAgicha Approach
	- Adjust only when one of the breakeven point is breached. <== InvestaBull + ManekAgicha Approach
	- Adjust everytime there is an imbalance in premiums. <== ThetaGainers Approach
2. Do not touch DCS on the tested side.
	- Note that the tested side DCS does not incur huge losses because...
		- The delta of the long calendar option from the back week dominates the delta of the short option in front week.
		- Also the front week option of DCS and back week option calendar DCS effeciently manage each other since their lot size is same.
		- Note that the 2 options are able to manage each other because we keep rebalancing the position using the non tested side DCS while collecting more and more credit.
	- We are regularly collecting profits by closing existing DCS on the non tested side.
	- We are also accumulating further credits by creating new DCS on the non tested side.
3. Close DCS on the non tested side.
	- `Exit from both long & short options` on the non tested side to book their profits.
	- Say the non tested premium is at ₹12 and you don't book profit.
	- The market further moves on the tested side and raises its option premium to ₹70.
	- Now this time the non tested option premium of ₹12 won't be able to offset this loss.
		- Note that it has already reduce so much and did its job of offsetting losses thus far.
		- Now it needs to slow down its momentum so that it can gradually reduce to ₹0 by expiry.
		- You must get rid of this option as it is of no use to us now.
		- Book its profit and exit so that you can create a new DCS to balance the tested side DCS.
	- These imbalance in premium won't offset each other's losses.
	- As we iteratively collect profit we minimize our overall loss.
4. Create a new DCS on the non tested side to balance the current high `premium` of existing DCS on the tested side.
	1. Pick the current premium of the short option on the tested side.
	2. Select the strike having premium slightly lower than the premium you picked in above step.
		- Do not match the premium exactly.
			- If tested side option is at ₹50 then on non tested side select a strike of around ₹40. It should be below ₹50.
		- By matching the premium exactly will result in adverse inverse effect.
	3. Short the selected strike option. Max profit will be at this short option strike price.
	4. Now hedge this short position to complete this DCS:
		1. Skip the front week expiry (i.e. expiry of the option used for strangle) and go to the subsequent week expiry (aka back week expiry).
		2. Pick the strike corresponding to the credit received from the sold option.
5. Review the payoff chart in opstra like so:
	- The `revised payoff chart` should appear `re-balanced`.
	- The green/red `PnL line` and `blue t+0 line` should be `center aligned`.
	- The `red line` (boundary of the loss) should `not` be too `steep`.
		- A too steep line implies that even a slight move in that direction will result in a `quick` and `huge` loss.
6. Stop adjustments when...
	- When the red line becomes too stop. It is too risky to adjustment when the line is too steep. <== ManekAgicha Approach
	- Don't do more than 1 adjusment. <== ManekAgicha Approach
7. Exit when...
	- `Stop Loss` reaches 1.5% of the total capital deployed (margin). <== ThetaGainers Approach
	- `Return on Capital` reaches 1.5% <== ThetaGainers Approach
	- `Return on Capital` reaches 2% <== InvestaBull Approach
	- Profit reaches 50% of the `Max Profit`. <== InvestaBull Approach
	- The market moved in one direction and we made adjustment. Then market reverts and returns to the middle of the payoff chart. <== InvestaBull Approach
		- If we keep on adjusting on both sides then our `Profbability of Profit` will keep on reducing.
8. Repeat step 1 through 7.
	- Repeat on every 30 min candle close. <== InvestaBull Approach
	- Repeat daily at 1:20 PM. <== ThetaGainers Approach

## Approach 3. Balance to neutralize delta

When we neutralize delta we save ourselves from gamma and protect position from radical market moves.

### Approach 3.1. Neutralize delta regularly

Periodically (daily) balance the two DCS by matching their call side delta with their put side delta.

##### Deployment

Create a short strangle like so:
- On the `front week` expiry short a `20Δ strike` OTM call & put.
- On the `back week` expiry long a call and a put `strikes that match the premium` of call & put in the front week expiry.
- Deploy strategy on `Wednesday @ 10:30 AM` considering the front week expiry is on next week's Thursday.
	- Essentially you pick a `8 DTE front week expiry`

##### Adjustment

1. Do not touch DCS on the tested side.
2. Close DCS on the non tested side.
	- `Exit from both long & short options` on the non tested side to book their profits.
	- As we iteratively collect profit we minimize our overall loss.
3. Create a new DCS on the non tested side to balance the current `delta` of existing short option on the tested side.
	1. Pick the current delta of the short option on the tested side.
	2. Select the strike with delta matching the delta you picked in above step.
	3. Short the selected strike option. Max profit will be at this short option strike price.
	4. Now hedge this short position to complete this DCS:
		1. Skip the front week expiry (i.e. expiry of the option used for strangle) and go to the subsequent week expiry (aka back week expiry).
		2. Pick the delta corresponding to the delta of sold option.
4. Review the payoff chart in opstra like so:
	- The `revised payoff chart` should appear `re-balanced`.
	- The green/red `PnL line` and `blue t+0 line` should be `center aligned`.
	- The `red line` (boundary of the loss) should `not` be too `steep`.
		- A too steep line implies that even a slight move in that direction will result in a `quick` and `huge` loss.
5. Repeat step 1 through 4.

### Approach 3.2. Neutralize delta after 50% drop
[...](https://www.youtube.com/watch?v=Fa_pn9W1bos)

Balance the two DCS by matching their call side delta with their put side delta but only when one of the delta drops by half.

##### Setup

- VIX should be below 18.
	- When vix is low, there is a less chance of gap-up/down.
		- This strategy won't work if there are too many gap-up/down.
		- There are very few strategies that can save you from gap-up/down.
	- You will incur loss when VIX falls.
	- You will incur gain when VIX rises.

##### Deployment

Create a short strangle like so:
- On the `front week` expiry short a `≤ 20Δ strike` OTM call & put.
- On the `back week` expiry long a call and a put `strikes with premium ≤ the premium of call & put in front week short option expiry`. This will turn the overall strategy into credit.
- Deploy strategy on `Thursday @ 9:20 AM` considering the front week expiry is on next week's Thursday.
	- Essentially you pick a `7 DTE front week expiry`.

##### Adjustment

1. Monitor deltas of short positions at every 30 min candle close.
	- Wait for one of the short option delta to reduce by half (40% to 50%).
	- If there is no move in the market and delta has not reduce by half skip to the last step.
2. Do not touch DCS on the tested side.
3. Close DCS on the non tested side.
	- `Exit from long & short options` on the non tested side to book their profits.
	- As we iteratively collect profit we minimize our overall loss.
4. Create a new DCS on the non tested side to balance the current `delta` of existing short option on the tested side.
	1. Pick the current delta of the short option on the tested side.
		- When selected delta is around 50, it becomes a `Short Straddle Diagonal Calendar`.
	2. Select the strike with delta matching the delta you picked in above step.
		- Note that this delta has now reduced by half.
	3. Short the selected strike option on front expiry. Max profit will be at this short option strike price.
	4. Now hedge this short position to complete this DCS:
		1. Skip the front week expiry (i.e. expiry of the option used for strangle) and go to the subsequent week expiry (aka back week expiry).
		2. `Either` pick a strike with `premium` ≤ the premium of front week expiry `short option` (step 4.3 above). This will maintain the overall strategy as credit.
		3. `Or` pick a strike with `delta` matching the delta of front week expiry `long option`. [...](https://youtu.be/Fa_pn9W1bos?t=808) | [...](https://youtu.be/Fa_pn9W1bos?t=985)
5. Review the payoff chart in opstra like so:
	- The `revised payoff chart` should appear `re-balanced`.
	- The green/red `PnL line` and `blue t+0 line` should be `center aligned`.
	- The `red line` (boundary of the loss) should `not` be too `steep`.
		- A too steep line implies that even a slight move in that direction will result in a `quick` and `huge` loss.
6. Repeat step 1 through 5 on the next 30 min candle close.

### Approach 3.3. Neutralize delta after 50% drop w/o touching the hedges
[...](https://www.youtube.com/watch?v=HalqbeA-wK0)

Balance the two DCS by matching their call side delta with their put side delta when one of the delta drops by half but without touching the hedges.

##### Deployment

Create a short strangle like so:
- On the `front week` expiry `short` a `≤ 20Δ strike` call & put.
- On the `back week` expiry `long` a `≤ 20Δ strike` call & put.
- The selected strikes should not be above 22Δ.
	- If you don't find strike around 20 then wait and deploy strategy later during the day.
- Deploy strategy on `Monday` considering the front week expiry is on next week's Thursday.
	- Essentially you pick a `10 DTE front week expiry`.

##### Adjustment

1. Monitor deltas of short positions on daily candle close.
	- Wait for one of the short option delta to reduce by half.
	- If there is no move in the market and delta has not reduce by half skip to the last step.
2. Do not touch DCS on the tested side.
3. Exit from the short option on the non tested side to book its profit.
	- `Do not touch the hedges` on the non tested side.
	- As we iteratively collect profit we minimize our overall loss.
4. Create a new short position on the non tested side to balance the current `delta` of existing short option on the tested side.
	1. Pick the current delta of the short option on the tested side.
		- When selected delta is around 50, it becomes a `Short Straddle Diagonal Calendar`.
	2. Select the strike with delta slightly lower than the delta you picked in above step.
		- Note that this delta has now reduced by half.
	3. Short the selected strike option on front expiry. Max profit will be at this short option strike price.
	4. Go long on the back week expiry option and pick the strike that matches the premium of the shorted front week expiry option (step 4.3 above).
5. We `need not look at the payoff charts` and focus only on adjusting the delta.
6. Stop adjustments when...
	- DTE ≤ 2
		- There is no point in doing adjustment when only 2 days are left.
		- If we do adjustment and a bigger move comes during this time then it will result in a far bigger loss due to gamma.
	- or `Double DCS` becomes an `Iron Fly`
7. Repeat step 1 through 6 on the next day morning @ 10:30 AM.