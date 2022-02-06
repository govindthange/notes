[...](https://www.youtube.com/watch?v=93IgLvYIONo&list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&index=3) | [...](https://www.youtube.com/watch?v=pDT8R6AxYTs&list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&index=5)

- It is a better substitute for `Iron Condor`.
- It is best suited for weekly option selling.
- It works better when VIX is between 17 to 25.
- It is not suited for monthly option selling as you end up too much for the back month hedge.

# Step 1. Find range
[[Strategy Builder Playbook#Step 1 Find range]]

# Step 2. Cover range
[[Strategy Builder Playbook#Step 2 Cover range]]

# Step 3. Define risk

Hedge naked strangle with the received credit through `Diagonal Calendar Spread`.

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

Deploy strategy on Wednesday @ 1:20 PM or by Thursday @ 01:20 PM.
Exit strategy next week on Wednesday @ 1:20 PM or by Thursday @ 9:20 AM.

# Step 5. Monitor position
[[Strategy Builder Playbook#Step 4 Monitor position]]

# Step 6. Adjust position
[...](https://youtu.be/93IgLvYIONo?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=317)

- Adjust trade @ 01:20 PM by either balancing premium or delta.
- When market trends up/down the long calendar option of the back week offsets loss from the front week and vice versa. But this balance only happens if you keep receiving credit from the other side of the option.
- By periodically balancing the shorted position prevents loss because back week's calendar delta dominates front week's option delta as both have same lot size.

## Approach 1. Adjust to neutralize premium gap

Balance position by matching the call side option premium with the put side option premium.

1. Do not touch options on the tested side.
2. Close the position on the non tested side and book the profit.
	- Say the non tested premium is at ₹12 and you don't book profit and the market moves to raise the tested side option to ₹70 then the non tested option premium will not even go from ₹12 to ₹2 so fast.
	- These imbalance in premium won't offset each other's losses.
3. Short a new option on the non tested side like so:
	1. Pick the current option premium of the tested side.
	2. Select the strike which has premium slightly lower than the picked premium on the non tested side.
		- Do not match the premium exactly.
			- If tested side option is at ₹50 then on non tested side select a strike of around ₹40.
		- By matching the premium exactly will result in adverse inverse effect.
	3. Short the selected strike option.

## Approach 2. Adjust to neutralize delta gap

Balance position by matching the call side delta with the put side delta.

1. Close the position on the non tested side and book the profit.
2. Short a new option on the non tested side like so:
	1. Pick the current option delta of the tested side.
	2. Select the strike which has delta slightly lower than the picked delta on the non tested side.
	3. Short the selected strike option.