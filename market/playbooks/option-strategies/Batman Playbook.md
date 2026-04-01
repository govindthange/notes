Its a double 1:2 ratio spread

# Step 1. Deploy

## Approach 1: Batman w/ 600 strike

> First of every month @ 3:15 PM

1. Long 1 CE 600 strikes above ATM
2. Short 2 CE 700 strikes above ATM
3. Long 1 CE 600 strikes below ATM
4. Short 2 CE 700 strikes below ATM

Exit?
- When VIX crosses 25?
- When MTM loss exceeds 3%?

## Approach 2: Many batmans
[...](https://youtu.be/cMTLBTt2jdU?t=344)

Enter 1st of every month @ 9:50 like so: [...](https://youtu.be/cMTLBTt2jdU?t=468)

Capital: 4.2L to 4.8L

Buy-sell-buy-sell  on put and call side
50-350-650-950 strikes away from ATM on put and call side both
1-2-2-4 lots on put and call side both.

Say ATM is @ 17850 strike
1. Long 1 lot 50 points above ATM (17800PE x 1)
2. Short 2 lots 300 points above step #1 strikes (17500PE x 2)
3. Long 2 lots 300 points above step #2 strikes (17200PE x 2)
4. Short 4 lots 300 points above step #3 strikes (16900PE x 4)
5. Follow same approach on CE side.


## Approach 3: Balanced legs w/ Delta
[...](https://www.youtube.com/watch?v=SxLwcdWJhWI&t=17s)

> Deploy on Friday @ 9:30 AM. [4th March 2022](https://youtu.be/SxLwcdWJhWI?t=215)

Margin: ₹1.6L for Nifty w/ 1:2 lots

1. Long 1 CE w/ 40Δ (NTM)
2. Short 3 CE w/ 30Δ (OTM)
3. Long 2 CE w/ 10Δ (Far OTM) 
4. Long 1 PE w/ 40Δ (NTM)
5. Complete PE side leg like so:
	- Follow the strike price difference of CE side.
	- We don't follow the same rules for setting PE leg. [...](https://youtu.be/SxLwcdWJhWI?t=151)
	- Count the distance of each CE option from ATM or from the 40Δ option strike and then set up PE side leg accordingly.
	- If we sold 3 CE options 500 points away from ATM, then we will sell 500 points PE options away from ATM.

## Approach 4: Double ratio spread w/ Delta
[Jul 2023 Deployment](https://youtu.be/fxr9MYgCSZY?t=122) | [Aug 2023 Deployment](https://www.youtube.com/watch?v=JaZagM0-O5g)

> Deploy on first Monday of every month @ 10 AM

Margin: ₹1.6L for Nifty w/ 1:2 lots

1. Short 2 PE w/ ≤ 25Δ
	- 18950PE @ ₹84.3 x 2 Lots
2. Long 1 PE w/ 100 points ITM strike above the Short PE
	- 19050PE @ ₹104.2 x 1 Lot
3. Short 2 CE w/ premium ≥ premium of sold PE
	- We do not match delta because it will get us lower premium for CE.
	- 19700PE @ ₹94 x 2 Lots
4. Long 1 CE w/ 100 points ITM strike below the Short CE
	- We again match CE option premium to the premium of bought PE option
	- 19600CE @ ₹111 x 1 Lot

The above sample deployment gave a range of 1000 to 1200 point range.

# Step 2. Adjust

## Approach 3 Adjustment

Adjust upon breach of break-even point. [...](https://youtu.be/SxLwcdWJhWI?t=456)

1. Wait for price to breach one of the break-even point.
2. Exit the 3 short options on the opposite side leg of the breached break-even point.
3. Short 3 options w/ 30Δ (OTM). This will push the break-even further.

4. `If market continues` in the same direction and again breaches the newly pushed break-even point, we again shift the opposite side of leg.
OR we will bring the 2 bought option on the break-even side inwards.

5. `If market reverses` and comes inside the strike of the 3 sold option on the breached break-even side then we exit the 3 newly short options in step 3 above. [...](https://youtu.be/SxLwcdWJhWI?t=503)
6. Now after adjustment #5, if market reverses again, then we wait for it to breach the new breakeven and exit [...](https://youtu.be/SxLwcdWJhWI?t=576)

## Approach 4 Adjustment

- Do not lose more than 2-3 percent.
- Exit when MTM loss ≥ 3%
- Exit when VIX shoots over 25

### Option 1: Buy to protect against overnight gap up/down
[...](https://youtu.be/xblhqvS_dLY?t=520) | [...](https://youtu.be/PjR4_52lFWI?list=PLWWIQDCw20f2JlRy0YNVi7AoM6HoEec4y&t=186)

Handle risk of loss due to 100 point gap-up shown by the blue line in payout chart.

1. Long 1 CE w/ 100 points above the Short CE strike.
	- For the above Approach 1 example, long 1 lot of  19800CE @ ₹51.5
2. Exit the hedge, when you enter back in the middle safe zone of batman ensuring that there is no loss in +2.5% percent over night move.

### Option 2: Shift to protect against overnight gap up/down
[...](https://youtu.be/xblhqvS_dLY?t=346) 

Handle risk of loss due to 100 point gap-up shown by the blue line in payout chart.

#### Step 1. Shift the PE side upwards 
[...](https://youtu.be/PjR4_52lFWI?list=PLWWIQDCw20f2JlRy0YNVi7AoM6HoEec4y&t=412)

1. Close the opposite side option positions.
	- If market is rallying upward (i.e. price is approaching the pyramid on the right side in Payout chart) then close the Long and Short PE legs.
2. Long 1 PE w/ 50 or 100 points above ATM strike
3. Short 2 PE w/ 100 points below the Long PE strike

#### Step 2. Buy if market continues its bullish momentum.
[...](https://youtu.be/PjR4_52lFWI?list=PLWWIQDCw20f2JlRy0YNVi7AoM6HoEec4y&t=578)

Now, if market still moves against you then follow Option 1 as above.

### Option 3: Option 2 -> Option 1

First shift, and then hedge the naked option.