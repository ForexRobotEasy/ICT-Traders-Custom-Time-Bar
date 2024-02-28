# ICT Traders Custom Time Bar ReadMe

This code is a custom time bar indicator for MetaTrader 5 platform. It allows users to select a specific time zone and displays OHLC (open, high, low, close) lines based on the selected time zone or the actual server time. Additionally, it adds vertical lines at specific times and allows users to customize the color and label of the horizontal lines.

## How it works

1. Initialization:
   - The code includes the necessary files for the dropdown menu control.
   - The global variable `g_timezone` is declared to store the selected time zone from the dropdown menu.
   - The `OnInit()` function is called during expert initialization and creates the dropdown menu for time zone selection. It adds three options: Eastern Standard Time (New York Local Time), Central Standard Time, and Pacific Standard Time.

2. Tick function:
   - The `OnTick()` function is called on every tick and performs the main functionality of the code.
   - It retrieves the selected time zone from the dropdown menu using the `CControlDropdown::GetValue()` method and saves it to the `g_timezone` variable.
   - It converts the server time to local time based on the selected time zone using the `ConvertToTimeZone()` function.
   - It adds a vertical line at a specific time in the selected time zone by comparing the local time with a specific time in the desired time zone.
   - It calculates and draws the OHLC lines based on the selected time zone or actual server time. The values are retrieved using the `iOpen()`, `iHigh()`, `iLow()`, and `iClose()` functions.

3. Additional functions:
   - The `ConvertToTimeZone()` function is responsible for converting the server time to local time based on the selected time zone. The implementation logic for this conversion is not shown in the code and needs to be implemented separately.
   - The `AddVerticalLine()` function adds a vertical line at a specific time with the given color. The implementation logic for adding a vertical line is not shown in the code and needs to be implemented separately.
   - The `AddHorizontalLine()` function adds a horizontal line at the given price with the given label and color. The implementation logic for adding a horizontal line is not shown in the code and needs to be implemented separately.

Please note that this code is provided by Forex Robot Easy Team as a sample that can work as described in the ICT Traders Custom Time Bar product. Forex Robot Easy Team is not the official developer of this product. To find the official developer and obtain the detailed reviews and trading results of this product, please visit the following link: [ICT Traders Custom Time Bar Review and Trading Results](https://forexroboteasy.com/forex-robot-review/ict-traders-custom-time-bar-review-optimize-forex-trading/)

## Product Description

ICT Traders Custom Time Bar is a powerful MetaTrader 5 indicator developed by an experienced team of traders. This indicator allows users to customize their time bar display and optimize their trading strategies based on specific time zones.

Key Features:
- Select from three popular time zones: Eastern Standard Time (New York Local Time), Central Standard Time, and Pacific Standard Time.
- Display OHLC lines based on the selected time zone or the actual server time.
- Add vertical lines at specific times in the selected time zone for better visualization of trading opportunities.
- Customize the color and label of the horizontal lines for easy identification of important price levels.

ICT Traders Custom Time Bar is designed to enhance your trading experience by providing accurate and customizable time bar information. By optimizing your trading strategies based on specific time zones, you can effectively analyze market movements and make informed trading decisions.

Please note that Forex Robot Easy Team is not the official developer of ICT Traders Custom Time Bar. We only provide this sample code to demonstrate the functionality of the product. To obtain the official version, detailed reviews, and trading results of ICT Traders Custom Time Bar, please visit the official developer's website using the MQL5 platform.
