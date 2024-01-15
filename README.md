# Sweet VWAP

Sweet VWAP is a trading strategy based on the Volume Weighted Average Price (VWAP) indicator. It is developed by the Forex Robot Easy Team and more information about this product can be found [here](https://forexroboteasy.com/forex-robot-review/sweet-vwap-forex-software-unbiased-review-real-results/). Please note that ForexRobotEasy is not the official developer of this product, and this code is only a sample that can work as described in the product.

## Description

Sweet VWAP is an automated trading strategy that uses the VWAP indicator to identify buy and sell signals. The VWAP indicator calculates the average price of a financial instrument based on its trading volume. The strategy executes trades when the current price is above or below the VWAP value.

## Features

- Uses the VWAP indicator to generate trading signals.
- Executes buy or sell trades based on the position of the current price relative to the VWAP value.
- Closes open trades when the current price crosses the open trade price.

## Requirements

- MetaTrader 4 platform.
- Trade library.
- Volume indicator.
- Moving Averages indicator.

## Installation

1. Copy the code into your MetaEditor.
2. Compile and install the EA on the desired chart.
3. Make sure the necessary libraries are included in the correct folders.

## Usage

1. Initialize the VWAP indicator by calling the `InitVWAP` function in the `OnInit` event.
2. Execute the VWAP trading strategy by calling the `ExecuteVWAPStrategy` function in the `OnTick` event.
3. Handle trading events by implementing the `OnTrade` function.
4. Deinitialize the VWAP indicator in the `OnDeinit` event.

## Custom Functions

### InitVWAP

This function initializes the VWAP indicator by setting its parameters and creating the necessary objects.

### ExecuteVWAPStrategy

This function executes the VWAP trading strategy by retrieving the VWAP value and the current price, and executing buy or sell trades based on their comparison.

### OnTrade

This function handles trading events by checking for open trades, retrieving the current price and trade price, and closing trades if the current price crosses the open trade price.

### OnInit

This function is called during program initialization and initializes the VWAP indicator by calling the `InitVWAP` function.

### OnDeinit

This function is called during program deinitialization and deinitializes the VWAP indicator by destroying the created objects.

### OnTick

This function is called on each tick and executes the VWAP trading strategy by calling the `ExecuteVWAPStrategy` function.

## Disclaimer

Please note that ForexRobotEasy is not the official developer of this product. The code provided is a sample that can work as described in the product. To find the official developer of this product, please use MQL5.

For detailed reviews and trading results of this product, please visit [here](https://forexroboteasy.com/forex-robot-review/sweet-vwap-forex-software-unbiased-review-real-results/).
