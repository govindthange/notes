# Managing Long Options

## Problems with Option Buying

- `Time Decay`
- `IV Crash:` If IV drops, Option value falls.
- `Can't adjust positions:` Unlike in Option Selling where you can rolldown or rollup on opposite/tested side, with option buying you can't adjust strategy. If you buy the other side to balance your positoin, there is a high chance both sides will come crashing down.
- `Can't utilitize collaterals:` If you have collateral, you can really use it. With option selling you can sell against the collateral to reduce the margin.

## Solution - Sell OTM Option

When you buy an option, buy ITM and sell OTM option to compensate for the Time Decay.

- Bull Call Spread
	- buy ITM CE and sell OTM CE option i.e. strike price of short call is above the strike of long call.
	- Ensure that Theta values of both ITM CE and OTM CE are same.
	- If you cant match the greeks refer [[#Selecting ITM w o Greeks]].
- Bear Put Spread
	- buy ITM PE and sell OTM PE option i.e. strike price of short put is below the strike of long put.
	- Ensure that Theta values of both ITM CE and OTM CE are same.
	- If you cant match the greeks refer [[#Selecting ITM w o Greeks]].


With option buying you can only adjust the winning trades not losing trades.
- If position moves in your favor, close the position the spot price reaches the strike price of the longed option and reopen a new Bull/Bear Call/Put Spread.
- If the positoin moves against you then you will have to bear the loss and close the position.

### How to choose Strike Price?

- Never select OTM strike price based on a fixed distance (like selecting OTM by +/- 300 points above/below ATM).
- Always select OTM based on Premium and/or [[Option Greeks]]

#### Selecting OTM w/ Greeks (Theta)

To sell option choose the OTM option strike which has the same theta as that of the ITM option strike you bought. that Theta values of both ITE and OTM option strikes are same.

#### Selecting ITM w/o Greeks
[...](https://youtu.be/tulEP6IDLmk?t=356)

Use the following process when you dont have a way to check Greeks to find out IV and theta values.

- Say you are bullish on nifty and you think it will go to 15300.
- You will SHORT `15300CE` @ ₹200
- Now you need to find ITM CE to go LONG.
- Check the premium of OTM CE which you selected to short; its ₹200.
- Look for a PE which has ₹200 premium. Say its `14600PE`. You will use this strike price, i.e. 14600, to buy CE (Not PE).
- You will LONG `14600CE` at whatever price its available (say its @ ₹600).

Note: With this process you are actually selling closer to the Spot price and buying CE strike which is deep In The Money. Refer [[#Q A]] section below.

By following above process you will ensure that ITM and OTM legs of your Bull Call Spread strategy have same IV and Theta values and therefore will nullify each other's side effects.

Now you need not worry about Theta Decay in LONG CE position and IV Spike in SHORT CE positoin.

##### Q&A
[...](https://youtu.be/tulEP6IDLmk?t=514)

- Isn't buying regular CE is more profitable than buying Bull Call Spread?
	- You can buy more Bull Call Spread as margin requirement is reduced due to the spread setup.
- Won't buying deep ITM and selling CE closer to the Spot value affect R/R ratio?
	- Yes, R/R is less in Bull Call Spread created this way but R/R is very high in Bear Put Spread
- Handling Illiquid Stocks?
	- [...](https://youtu.be/tulEP6IDLmk?t=572)

# Managing Short Puts
[...](https://www.tastytrade.com/shows/trade-managers/episodes/short-put-management-01-02-2018)

## Managing w/o altering the trade

### Roll Short Puts

#### Roll same strike out

#### Do nothing

#### Role strike down and out
