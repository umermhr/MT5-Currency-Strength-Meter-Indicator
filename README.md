# CM Strength Indicator for MetaTrader 5 (MT5)

The **CM Strength Indicator** is a custom MetaTrader 5 (MT5) indicator designed to measure and display the relative strength of major currencies in the forex market. It helps traders identify strong and weak currencies, which can be useful for making informed trading decisions.

---

## Features

- **Currency Strength Meter**: Displays the relative strength of 8 major currencies (USD, EUR, GBP, JPY, AUD, NZD, CAD, CHF).
- **Real-Time Updates**: The indicator updates in real-time, showing the current strength of each currency.
- **Historical Comparison**: Compares the current strength of currencies with their strength 30 minutes ago.
- **Customizable Pairs**: Supports both default currency pairs and custom pairs provided by the user.
- **Visual Indicators**: Uses color-coded text and arrows to indicate whether a currency is gaining or losing strength.
- **Easy to Use**: Simple and intuitive interface for quick analysis.

---

## Installation

1. **Download the Indicator**:
   - Download the `CM Strength.mq5` file from this repository.

2. **Copy the File to MT5**:
   - Open your MetaTrader 5 platform.
   - Go to `File > Open Data Folder`.
   - Navigate to `MQL5 > Indicators`.
   - Copy the `CM Strength.mq5` file into the `Indicators` folder.

3. **Compile the Indicator**:
   - Restart your MT5 platform or refresh the `Navigator` panel.
   - Drag and drop the `CM Strength` indicator onto a chart.
   - If prompted, allow the indicator to access external resources.

4. **Configure Settings**:
   - Adjust the input parameters (e.g., `x_axis`, `y_axis`, `UseDefaultPairs`, `OwnPairs`) as needed.

---

## Input Parameters

| Parameter          | Description                                                                 |
|--------------------|-----------------------------------------------------------------------------|
| `x_axis`           | Horizontal position of the indicator on the chart.                         |
| `y_axis`           | Vertical position of the indicator on the chart.                           |
| `UseDefaultPairs`  | If `true`, the indicator uses the default 28 currency pairs.               |
| `OwnPairs`         | Comma-separated list of custom currency pairs (e.g., `"EURUSD,GBPUSD"`).    |

---

## How It Works

1. **Currency Strength Calculation**:
   - The indicator calculates the strength of each currency based on its performance across multiple currency pairs.
   - It uses the bid price and price range of each pair to determine the relative strength.

2. **Display**:
   - The indicator displays the strength of each currency in a sorted list, with the strongest currency at the top.
   - Arrows indicate whether a currency is gaining (▲) or losing (▼) strength compared to the previous calculation.

3. **Color Coding**:
   - The strength values are color-coded to provide a quick visual reference:
     - **Green**: Strong currency.
     - **Red**: Weak currency.
     - **Orange/Yellow**: Moderate strength.

---

## Example Usage

1. **Identify Strong/Weak Currencies**:
   - Look for currencies at the top (strong) or bottom (weak) of the list.
   - Use this information to identify potential trading opportunities.

2. **Compare Historical Strength**:
   - Observe the arrows to see if a currency is gaining or losing strength over time.
   - This can help you anticipate trend reversals or continuations.

3. **Customize Currency Pairs**:
   - If you want to focus on specific pairs, use the `OwnPairs` input to define your custom list.

---

## Notes

- The indicator is designed for use in the forex market and works best with major currency pairs.
- Ensure your MT5 platform is connected to a reliable data source for accurate calculations.
- The indicator does not provide trading signals directly but can be used as part of a broader trading strategy.

---

## Contributing

If you'd like to contribute to this project, feel free to fork the repository and submit a pull request. Suggestions for improvements and bug fixes are welcome!

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Disclaimer

This indicator is provided for educational and informational purposes only. It does not constitute financial advice, and you should conduct your own research before making any trading decisions. The developer is not responsible for any losses incurred while using this indicator.

---

For questions or support, please open an issue in this repository or contact the developer directly.