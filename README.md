# lookback_option

A Lookback Option is a type of exotic option that allows the holder to "look back" over the life of the option to determine the optimal payoff. The unique feature of lookback options is that they provide the holder with the advantage of the best price of the underlying asset during the option's life, either to minimize the strike price for a call option or to maximize the strike price for a put option.


Underlying Asset (S): The asset on which the option is based (e.g., a stock, index).
Strike Price (K): The price at which the option can be exercised. This can be fixed at the outset (for Fixed Lookback Options) or determined by the best price during the option's life (for Floating Lookback Options).
Maximum Price (S_max): The highest price of the underlying asset during the life of the option.
Minimum Price (S_min): The lowest price of the underlying asset during the life of the option.
Final Price (S_T): The price of the underlying asset at the option's maturity.

Call Option: Gives the holder the right to buy the underlying asset.
Put Option: Gives the holder the right to sell the underlying asset.


1) Fixed Lookback Option:
The strike price is set at the inception of the option. The payoff is determined based on the maximum or minimum price of the underlying asset during the life of the option.

Call Option Payoff:
Payoff = max(S_max - K, 0)
Where:
S_max is the maximum price of the underlying asset during the option's life.
K is the fixed strike price.

Put Option Payoff:
Payoff = max(K - S_min, 0)
Where:
S_min is the minimum price of the underlying asset during the option's life.

2) Floating Lookback Option:
The strike price is determined based on the minimum price for a call option or the maximum price for a put option during the life of the option. The payoff is then calculated using the final price of the underlying asset at maturity.

Call Option Payoff:
Payoff = max(S_T - S_min, 0)
Where:
S_T is the final price of the underlying asset at maturity.
S_min is the minimum price of the underlying asset during the option's life.

Put Option Payoff:
Payoff = max(S_max - S_T, 0)
Where:
S_max is the maximum price of the underlying asset during the option's life.
