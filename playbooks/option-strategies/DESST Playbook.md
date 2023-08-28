
# Delta Enhanced Short Spread Thrust (DESST)

This name reflects the step-by-step enhancement of a short spread, where we begin with a long position and then layer on the spread components. It also highlights the delta aspect, which is central to the strategy's design. The name is broad enough to encompass both the call and put variations of our strategy.

"Delta Enhanced Thrust" implies the forceful directional bias achieved through the combination of the option and spread.  The initial 24 delta option purchase followed by the spread with different delta levels creates a powerful and overwhelming flow of gains.

### Delta

With delta we control the option's sensitivity to changes in the underlying asset's price.

- By combining different delta options, we create a nuanced position that reacts to changes in the underlying's price.
    - 24, 12, 8 gives 3% max loss
	    - => 0.13% gives % gain or % loss
	    - => 0.2% change gives % gain or % loss
	    - => 0.3% change gives 1% gain or ?% loss
    - 50, 30, 20 gives 6% max loss
	    - => 0.13% gives % gain or % loss
	    - => 0.2% change gives % gain or % loss
	    - => 0.3% change gives % gain or % loss
    - 80, 50, 30 gives 15% max loss
	    - => 0.13% gives 1.56% gain or 1.18% loss
	    - => 0.2% change gives 2.1% gain or 1.7% loss
	    - => 0.3% change gives 3.3% gain or 2.7% loss

### Short Spread

We employ a short spread by taking simultaneous long and short positions to potentially benefit from specific market movements.

### Delta Enhancement

Delta Enhancements signify that we progressively modify a traditional long option position by creating a short spread using different delta options.

This name effectively communicates the structure and intent of our strategy, indicating that it involves options with a gradient of delta values.

# Stretegy

In this strategy we combine a long put/call option with a short put/call spread involving two lots. Here's how this combination might look:

Long Put Option (1 Lot):
    Buy 1 lot of put options at a specific strike price.
    This position benefits from a significant decline in the price of the underlying asset. Your potential profit is unlimited, as the asset's price can theoretically fall to zero. However, your potential loss is limited to the premium you paid for the put option.

Short Put Spread (2 Lots):
    Sell 2 lots of put options at a lower strike price.
    Simultaneously, buy 2 lots of put options at a higher strike price.
    The premium received from selling the lower strike put options helps offset the cost of buying the higher strike put options.
    This position benefits from limited price movements within a specific range and from decreasing implied volatility. Your potential profit is limited to the net premium received, and your potential loss is limited to the difference between the strike prices minus the net premium received.