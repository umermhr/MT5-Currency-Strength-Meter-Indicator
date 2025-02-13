# CM Strength Indicator

The CM Strength Indicator is a custom MetaTrader 5 (MT5) indicator that measures the strength of various currency pairs and displays the results on the chart. This indicator helps traders to identify strong and weak currencies, which can be useful for making trading decisions.

## Features

- Calculates the strength of multiple currency pairs.
- Displays the strength of each currency on the chart.
- Uses both current and previous currency strength for comparison.
- Customizable display settings.

## Installation

1. Download the `CM Strength.mq5` file.
2. Open the MetaTrader 5 platform.
3. Go to `File` -> `Open Data Folder`.
4. Navigate to `MQL5` -> `Indicators`.
5. Copy the `CM Strength.mq5` file into the `Indicators` folder.
6. Restart the MetaTrader 5 platform.
7. In the Navigator window, find the `CM Strength` indicator under `Indicators`.
8. Drag and drop the indicator onto a chart.

## Inputs

- `x_axis`: X-axis position for the display.
- `y_axis`: Y-axis position for the display.
- `UseDefaultPairs`: Use the default 28 currency pairs.
- `OwnPairs`: Comma-separated list of custom currency pairs.

## Usage

Once the indicator is added to the chart, it will display the strength of the selected currency pairs. The strength is calculated based on the price movements and displayed in a color-coded format. The indicator also shows the direction of the strength change using arrows.

## Functions

### `OnInit()`
Initializes the indicator, sets up the currency pairs, and starts the timer.

### `OnCalculate()`
Handles the calculation of the indicator values.

### `OnDeinit()`
Cleans up when the indicator is removed from the chart.

### `OnTimer()`
Calls the `GetSignals()` and `displayMeter()` functions to update the display.

### `GetSignals()`
Calculates the strength and other metrics for each currency pair.

### `displayMeter()`
Displays the calculated strength values on the chart.

### `SetText()`
Creates and sets the properties of a text object on the chart.

### `SetObjText()`
Creates and sets the properties of a text object with a specific font on the chart.

### `currency_strength()`
Calculates the current strength of a given currency.

### `old_currency_strength()`
Calculates the previous strength of a given currency.

### `color_for_profit()`
Determines the color to use for displaying the strength based on its value.

## License

This indicator is provided under the MetaQuotes Software Corp. license. For more information, visit [MetaQuotes Software Corp.](https://www.mql5.com).

## Disclaimer

Trading in the financial markets involves risk. This indicator is provided for informational purposes only and should not be considered as financial advice. Always do your own research before making any trading decisions.

---

For more information, visit the [MetaQuotes Software Corp.](https://www.mql5.com) website.