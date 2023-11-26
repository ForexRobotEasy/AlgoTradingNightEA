# AlgoTradingNightEA Code ReadMe

This ReadMe file provides an overview of the AlgoTradingNightEA code. The code is designed to be used in the MetaTrader 5 (MQL5) platform for automated forex trading. It is important to note that ForexRobotEasy is not the official developer of this product, but we are providing a sample code that can work as described in the product.

## Table of Contents
1. [Currency Pairs](#currency-pairs)
2. [Expert Initialization](#expert-initialization)
3. [Expert Deinitialization](#expert-deinitialization)
4. [Expert Start](#expert-start)
5. [Evening Check](#evening-check)
6. [Price Deviation Calculation](#price-deviation-calculation)
7. [Price Deviation Acceptance Check](#price-deviation-acceptance-check)
8. [Additional Filters Check](#additional-filters-check)
9. [Trade Opening](#trade-opening)
10. [Program Entry Point](#program-entry-point)

## Currency Pairs <a name='currency-pairs'></a>
The code includes an array named `currencyPairs`, which contains a list of currency pairs to be traded. The default pairs included in the code are 'USDCHF', 'EURUSD', 'GBPUSD', 'EURCHF', 'USDCAD', 'GBPAUD', 'CADCHF', 'EURAUD', 'AUDCHF', and 'GBPCHF'. Traders can modify this array to include or exclude currency pairs as desired.

## Expert Initialization <a name='expert-initialization'></a>
The `OnInit()` function is called when the expert advisor is initialized. This function can be used to perform any necessary initialization tasks. The function should return `INIT_SUCCEEDED` if initialization is successful.

## Expert Deinitialization <a name='expert-deinitialization'></a>
The `OnDeinit()` function is called when the expert advisor is deinitialized. This function can be used to perform any necessary deinitialization tasks. The `reason` parameter indicates the reason for deinitialization.

## Expert Start <a name='expert-start'></a>
The `OnTick()` function is called on every tick. This function checks if it is evening and if the price deviation is within an acceptable range. If these conditions are met, it checks for additional filters. If all conditions are satisfied, it calls the `OpenTrade()` function to open a trade.

## Evening Check <a name='evening-check'></a>
The `IsEvening()` function is used to check if it is evening. The current implementation returns `true` as a placeholder value for testing. Traders should modify this function to check if it is evening based on their trading strategy.

## Price Deviation Calculation <a name='price-deviation-calculation'></a>
The `GetPriceDeviation()` function calculates the current price deviation. The current implementation returns `0.01` as a placeholder value for testing. Traders should modify this function to calculate the price deviation based on their trading strategy.

## Price Deviation Acceptance Check <a name='price-deviation-acceptance-check'></a>
The `IsPriceDeviationAcceptable()` function checks if the price deviation is within an acceptable range. The current implementation returns `true` as a placeholder value for testing. Traders should modify this function to check if the price deviation meets their criteria.

## Additional Filters Check <a name='additional-filters-check'></a>
The `PassAdditionalFilters()` function checks if additional filters pass. The current implementation returns `true` as a placeholder value for testing. Traders should modify this function to check if all additional filters are satisfied based on their trading strategy.

## Trade Opening <a name='trade-opening'></a>
The `OpenTrade()` function is called to open a trade. Traders should add their code to open a trade within this function.

## Program Entry Point <a name='program-entry-point'></a>
The `OnStart()` function is the program entry point and is called when the expert advisor starts. Traders can add any necessary code within this function.

For more detailed reviews and trading results of this product, please visit the [AlgoTradingNightEA Review](https://forexroboteasy.com/forex-robot-review/algotradingnightea-review-real-results-pricing-updates/) page on ForexRobotEasy.com. Please note that ForexRobotEasy is not the official developer of this product, but we provide information and samples regarding the product. To find the official developer of this product, please refer to the MQL5 platform.
