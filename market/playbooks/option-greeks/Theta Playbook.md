- Positive theta means you have credit strategy.
- Theta is negative for buyers because he is paying premium.
- Theta is positive for sellers because he is receiving premium.
- Sellers make more profit when they keep position overnight.
- Option selling is tough for intraday because major theta decay happens overnight.

# Time Decay Prevention
[...](https://www.youtube.com/watch?v=tulEP6IDLmk)

## Problems with Option Buying
[...](https://youtu.be/tulEP6IDLmk?t=110)

1. Time decay
2. IV Crash
	- Incur loss when IV comes down.
3. You can't do adjustment.
	- With option selling you can easily...
		- Roll up/down.
		- Sell extra option on the non tested side.
		- You can make use of collateral.

## Debit vertical spread w/ zero 𝜃 decay
[...]([...](https://youtu.be/tulEP6IDLmk?t=322))

Mix option buying with option selling like so... [...](https://youtu.be/tulEP6IDLmk?t=173)
- For bullish view do Bull Call Spread.
	- Buy ITM call.
		- This will have a less 𝜃 decay.
		- You will incur loss due to 𝜃 decay.
	- Sell OTM call.
		- You will earn through 𝜃 decay.
		- With this you will offset 𝜃 decay loss in long option.
- For bearish view do Bear Put Spread.
	- Buy ITM put.
	- Sell OTM put.

### Approach 1. Match greeks
[...](https://youtu.be/tulEP6IDLmk?t=334)

- Choose ITM strike and OTM strikes with matching theta values.

### Approach 2. Match premiums diagonally
[...](https://youtu.be/tulEP6IDLmk?t=353)

1. Establish target where the price will go.
2. Sell an option (say CE) with strike matching the target.
	- Short call if you are bullish.
	- Short put if you are bearish.
3. Look for an option of the opposite type (i.e. PE in this case) with a premium as that of the short option.
	- Select a put strike with premium as that of short call in bullish case.
	- Select a call strike with premium as that of short put in bearish case.
4. Buy the corresponding option but with the type as that of the short option (i.e. CE in this case).
	- Long call in bullish case.
	- Long put in bearish case.

### Approach 3. Calculate time value
 [...](https://youtu.be/G4EIKF_Hirw?t=592)

1. Select an ITM strike which... [...](https://youtu.be/tulEP6IDLmk?t=272)
	- Is not too deep ITM.
	- Has lowest [[Trade#Bid-Ask Spread]].
	- Has lowest time value.
2. Buy the option with the selected strike.
3. Calculate the time value of this option.
	- Call Time Value => `Premium` - (`Spot Price` - `Strike Price`)
	- Put Time Value => `Premium` - (`Strike Price` - `Spot Price`)
4. Search for a strike which has premium that matches the above calculated time value.
5. Short the option.
