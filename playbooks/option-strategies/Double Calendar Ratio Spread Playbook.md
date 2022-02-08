# Step 1. Find range
[[Strategy Builder Playbook#Step 1 Find range]]

# Step 2. Cover range
[[Strategy Builder Playbook#Step 2 Cover range]]

# Step 3. Define risk

Hedge naked strangle with the received credit through `Credit Ratio Diagonal Calendar Spread`.

1. Define risk with 1:1 Risk/Reward ratio.
	- If you receive ₹10,000 in credit, then only debit ₹10,000 for hedging.
	- Its fine to pay slightly extra.
2. Hedge the short position in ratio (not entirely in 1:1.
	- Skip the near expiry (ifront week/month) i.e. expiry of the option used for strangle and go to the subsequent expiry (AKA next expiry or back week/month expiry).
	- Pick the strike corresponding to the credit received from the sold options.
	- You may pay slightly extra because you will close this position in the near expiry (i.e. front week/month).
	- By buying PE & CE options will increase breakeven range.

# Step 4. Monitor position
[[Strategy Builder Playbook#Step 4 Monitor position]]

# Step 5. Adjust position
[...](https://youtu.be/dhEPY7DUBwI?list=PLWWIQDCw20f2k9frpTPK9bhZQO50Hyg1g&t=469)

## Possibility 1. When stock trends up

Reduce loss on the call side in 2 stages.

### Stage 1. Adjust upon breach of 50% range (300 Points)

#### Sell an extra put at far OTM

- Sell far OTM put till the price breaches the strike of the shorted call option.
- It will flatten the t+0 blue line in opstra.

### Stage 1. Adjust upon breach of shorted CE strike

- Buy call option at the breakeven point.
- By buying call option it will remove the ratio spread and make it 1:1 diagonal calendar spread on the call side.

## Possibility 2. When stock trends down

Do the opposite.

