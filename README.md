# OzzieQuid EA

This is a sample code for the OzzieQuid EA, developed by the Forex Robot Easy Team. The OzzieQuid EA is designed to trade the GBP/AUD currency pair on the H4 timeframe. It uses daily tops and bottoms in conjunction with Pivot Points to determine entry and exit points for trades.

## Input Parameters

- `LotSize` (default: 0.01): The lot size for trading.
- `StopLoss` (default: 100): The stop loss in pips.
- `TakeProfit` (default: 200): The take profit in pips.

## Initialization

The expert advisor checks if the current timeframe is H4. If not, it prints an error message and returns `INIT_FAILED`. It also adds the necessary indicators and sets the indicator name as 'OzzieQuid EA'.

## Deinitialization

The expert advisor removes any added indicators when it is being deinitialized.

## Start Function

In the `OnTick()` function, the expert advisor gets the daily tops and bottoms in confluence with Pivot Points. It calculates the pivot points and checks if the current price is above the daily top or below the daily bottom.

If the current price is above the daily top, a buy order is opened with the specified lot size, stop loss, and take profit. If the order is opened successfully, a success message is printed. Otherwise, a failure message is printed.

If the current price is below the daily bottom, a sell order is opened with the specified parameters. The same process is followed to check if the order is opened successfully or not.

## Tick Function

The `OnCalculate()` function is responsible for calculating the pivot points and displaying them on the chart. It calculates the pivot points, resistance levels (R1, R2, R3), and support levels (S1, S2, S3). It creates horizontal lines on the chart to visualize these levels.

## Product Description

Introducing the OzzieQuid EA, a sophisticated forex trading robot developed by the Forex Robot Easy Team. This expert advisor is specifically designed to master the GBP/AUD market with precision and sophistication.

The OzzieQuid EA utilizes a unique strategy based on daily tops and bottoms in conjunction with Pivot Points. It carefully analyzes market conditions on the H4 timeframe to identify profitable trading opportunities.

With customizable input parameters such as lot size, stop loss, and take profit, the OzzieQuid EA provides flexibility to suit different trading preferences and risk tolerance levels.

Key Features:
- Designed for the GBP/AUD currency pair on the H4 timeframe.
- Utilizes daily tops and bottoms in confluence with Pivot Points.
- Opens buy orders when the price is above the daily top and sell orders when the price is below the daily bottom.
- Customizable input parameters for lot size, stop loss, and take profit.

Please note that Forex Robot Easy is not the official developer of the OzzieQuid EA. We are simply showcasing a sample code that demonstrates how this product works. To find the official developer of the OzzieQuid EA and access detailed reviews and trading results, please visit [this link](https://forexroboteasy.com/forex-robot-review/ozziequid-ea-review-mastering-gbpaud-market-with-sophistication/).

For more information and to explore other forex trading products, please visit our website: [https://www.forexroboteasy.com](https://www.forexroboteasy.com)
