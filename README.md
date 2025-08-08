# Comprehensive Trading Indicator - CRT + FVG + CISD + EMAs

A comprehensive Pine Script indicator that combines multiple advanced trading analysis techniques for TradingView.

## 📊 Features

This indicator integrates 8 powerful trading analysis tools:

### 1. **Breakout Detection**
- Identifies large candles that break above average range
- Configurable lookback length and range multiplier
- Visual signals with shape plots and background highlighting

### 2. **EMA Analysis** 
- Four EMAs: 20, 50, 100, and 200 periods
- Dynamic color coding based on slope direction
- Live labels showing current EMA values

### 3. **Fair Value Gap (FVG) Detection - Session Based**
- Detects first FVG of trading session (9:32-16:00 NY time)
- Customizable session times and box colors
- NY market open time and price markers
- Supports multiple days history

### 4. **Multi-Timeframe CRT (Consolidation Range Touch)**
- Tracks consolidation ranges across 7 timeframes:
  - 2-day, 1-hour, 2-hour, 4-hour, Daily, Weekly, Monthly
- Configurable touch detection (wick/body)
- Visual range lines with 50% midpoint levels
- Alert system for range touches
- Customizable labels and colors

### 5. **Advanced FVG Detection with Mitigation**
- Advanced FVG detection with threshold settings
- Mitigation tracking and visualization
- Dynamic vs static display modes
- Statistics dashboard showing FVG counts and mitigation rates
- Unmitigated levels highlighting

### 6. **CISD (Change in State of Delivery) Detection**
- Market structure change detection
- Bullish and bearish CISD level identification
- Configurable line styles and extensions
- Statistics table showing current market state

### 7. **CRT Specific Time Analysis**
- Time-based CRT analysis for specific hours (6, 10, 14 EST)
- Large candle filtering with wick ratio analysis
- CRT sweep detection and alerts
- Special time highlighting

### 8. **HTF Candle Visualization**
- Higher timeframe candle representation on current chart
- Special time period highlighting (purple candles)
- Configurable display settings
- Real-time candle updates

## ⚙️ Configuration Groups

### Breakout Detection
- **Lookback Length**: Period for average range calculation (default: 14)
- **Range Multiplier**: Threshold for breakout detection (default: 1.5)

### FVG Settings
- **Session Time**: Trading session for FVG detection
- **Box Colors**: Customizable up/down colors
- **Max Days**: Number of historical days to display
- **NY Open Markers**: Toggle time lines and price levels

### CRT Timeframes
- **Enable/Disable**: Individual timeframe toggles
- **Colors**: Custom colors for each timeframe
- **50% Levels**: Midpoint level display options

### CRT Options
- **Minimum/Maximum Bars**: Range validation parameters
- **Line Widths**: Visual customization
- **Touch Detection**: Wick vs body touch settings

### CRT Labels
- **Label Styles**: Multiple shape options
- **Colors**: Bullish/bearish color schemes
- **Label Management**: Maximum count and positioning

### Advanced FVG
- **Threshold**: Percentage or auto-calculation
- **Mitigation Levels**: Show/hide mitigation lines
- **Dynamic Mode**: Real-time vs static boxes
- **Dashboard**: Statistics display options

### CISD Settings
- **Colors**: Bull/bear CISD colors
- **Line Styles**: Solid, dotted, or dashed
- **Extensions**: Forward projection settings
- **Statistics Table**: Market state tracking

### CRT Time Analysis
- **Time Filtering**: Specific hour analysis
- **Candle Filtering**: Large candle detection
- **Wick Ratios**: Body-to-wick ratio thresholds

### HTF Candles
- **Timeframe**: Higher timeframe selection
- **Display Count**: Maximum candles to show
- **Visual Settings**: Colors and positioning

## 🚨 Alert System

The indicator includes comprehensive alerts for:
- Breakout detection (bullish/bearish)
- CRT range touches (all timeframes)
- FVG formation and mitigation
- CISD state changes
- CRT sweeps

## 📈 Usage Instructions

1. **Add to Chart**: Copy the Pine Script code to TradingView
2. **Configure Settings**: Adjust parameters in each group based on your trading style
3. **Enable Alerts**: Set up alerts for desired conditions
4. **Monitor Dashboard**: Use statistics tables for market state awareness

## 🔧 Technical Requirements

- **Pine Script Version**: v6
- **Chart Requirements**: 
  - Max lines: 500
  - Max labels: 500
  - Max bars back: 5000
- **Overlay**: Must be applied as overlay indicator

## 📝 Key Functions

### Core Detection Functions
- `process_tf()`: Multi-timeframe consolidation range processing
- `detect()`: Advanced FVG detection with thresholds
- `in_session()`: Session time validation
- Market structure analysis for CISD

### Visual Management
- `plot_lines()`: Dynamic line plotting and updates
- `manageLabelCount()`: Label count optimization
- `make_box()`: FVG box creation with metadata
- HTF candle visualization methods

### Utility Functions
- `getLabelStyle()`: Label style conversion
- `getLabelSize()`: Size parameter conversion
- `day_of_week_text()`: Day identification
- Time-based calculations

## 💡 Trading Applications

This indicator is designed for:
- **Scalping**: Quick breakout and FVG opportunities
- **Swing Trading**: Multi-timeframe CRT analysis
- **Market Structure**: CISD and HTF analysis
- **Session Trading**: NY session FVG patterns
- **Alert-Based Trading**: Automated signal detection

## ⚠️ Important Notes

- Configure timeframes according to your trading style
- Adjust threshold parameters for your market conditions
- Use appropriate risk management with all signals
- Backtest settings before live trading
- Monitor performance statistics regularly

## 📄 License

This Pine Script code is subject to the terms of the Mozilla Public License 2.0.

## 👤 Author

© Zidanola

---

*For questions, support, or contributions, please refer to the TradingView community or Pine Script documentation.*
