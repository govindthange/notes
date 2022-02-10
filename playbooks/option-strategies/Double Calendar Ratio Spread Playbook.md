[...](https://youtu.be/zMwFaIqWYhs?list=PLOggP3CmSaMDKsajRrNOECS4U94v4xvxc&t=3220)

Iron Condor + Calendar + Ratio Spread

# Step 1. Find range
[[Strategy Builder Playbook#Step 1 Find range]]

# Step 2. Cover range
[[Strategy Builder Playbook#Step 2 Cover range]]

# Step 3. Define risk

Hedge naked strangle with the received credit through `Credit Ratio Diagonal Calendar Spread`.

1. Define risk with 1:1 Risk/Reward ratio.
	- If you receive ₹10,000 in credit by shorting a given option, then spend ₹10,000 to buy option for hedging the short option.
	- Its fine to pay slightly extra.
2. Hedge the short position in 3:5 ratio (Its a ratio spread so don't buy 1 for 1 hedge.).
	- Skip the near expiry (front week/month) i.e. expiry of the option used for strangle and go to the subsequent expiry (AKA next expiry or back week/month expiry).
	- Pick the strike corresponding to the credit received from the sold options.
	- You may pay slightly extra because you will close this position in the near expiry (i.e. front week/month).
	- By buying PE & CE options will increase breakeven range.

# Step 4. Monitor position
[[Strategy Builder Playbook#Step 4 Monitor position]]

# Step 5. Adjust position

No adjustment is needed till market moves beyond 1.75% (or 300 points move in nifty) in one direction.

## Possibility 1. When stock trends up

Reduce loss on the call side in 2 stages.

### Stage 1. Adjust upon breach of 50% range (300 Points)

#### Sell a near expiry OTM put
[...](https://youtu.be/dhEPY7DUBwI?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=469)

- Sell a near expiry OTM put once price rises by 1.75% (300 points in nifty) but has not breached the strike of shorted call option.
- Selling an extra put will flatten the t+0 blue line in opstra.

### 2. Adjust upon breach of shorted CE strike

#### Buy a next expiry OTM call
[...](https://youtu.be/dhEPY7DUBwI?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=572)

- Buy a next expiry call option at the breakeven strike once the strike of shorted call option is breached.
- By buying call option it will remove the ratio spread and make it 1:1 diagonal calendar spread on the call side.

## Possibility 2. When stock trends down

Do the opposite.

# Step 6. Exit

- For weekly trades, exit within 2 days or whenever you see profit of 2%.
	- If you deployed strategy on Monday then exit by Wednesday i.e. within 2 days.
- For monthly trades, exit by 15th of the month.
	- If you deployed strategy on the first week of the month then exit by the end of 2nd week.