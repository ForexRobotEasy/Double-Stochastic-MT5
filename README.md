# Double Stochastic MT5

This is a custom indicator developed by Forex Robot Easy Team. It is designed to calculate the Double Stochastic values for a given period. The Double Stochastic is a popular technical indicator used in financial trading, particularly in the analysis of price momentum and trend reversals.

## Indicator Settings

- Chart Window: Enabled
- Indicator Buffers: 2
- Indicator Color 1: Red
- Indicator Color 2: Green

## Input Parameters

- KPeriod: The period for calculating the K value (default: 14)
- DPeriod: The period for calculating the D value (default: 3)
- Slowing: The slowing value (default: 3)
- OverboughtLevel: The overbought level (default: 80)
- OversoldLevel: The oversold level (default: 20)

## Indicator Buffers

- StochasticBuffer: Buffer for storing the calculated K values
- RsiBuffer: Buffer for storing the calculated D values

## Indicator Initialization

The indicator buffers are mapped and initialized in the `OnInit()` function. The indicator label is set as 'Double Stochastic MT5'.

## Indicator Calculation

The indicator values are calculated in the `OnCalculate()` function. The function takes the necessary input parameters and price data to calculate the Double Stochastic values.

The function first checks if there are enough bars for calculation. If not, it returns 0.

Then, it calculates the Stochastic values for each bar using the given input parameters. The calculation involves summing the differences between the high and low prices over the specified periods. The K and D values are then stored in the respective indicator buffers.

Finally, the function returns the total number of bars calculated.

## Product Description

Double Stochastic MT5 is a custom indicator developed by Forex Robot Easy Team. It is designed to provide traders with insights into price momentum and trend reversals.

The indicator calculates the K and D values of the Double Stochastic indicator based on the provided input parameters. These values can be used to identify potential overbought and oversold levels in the market.

The indicator is easy to use and can be applied to any financial instrument and time frame. It is a valuable tool for traders looking to make informed trading decisions based on price momentum and trend analysis.

Please note that ForexRobotEasy is not the official developer of this product. We only provide sample code that can work similarly to the described product. To find the official developer of this product, please refer to MQL5.

For detailed reviews and trading results of this product, please visit [Forex Robot Easy - Double Stochastic MT5 Review](https://forexroboteasy.com/forex-robot-review/double-stochastic-mt5-review-enhanced-forex-indicator-analysis/).
