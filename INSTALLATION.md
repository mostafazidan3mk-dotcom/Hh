# Installation Guide

## Quick Setup

### Step 1: Copy the Code
1. Open the `comprehensive_trading_indicator.pine` file
2. Select all code (Ctrl+A / Cmd+A)
3. Copy to clipboard (Ctrl+C / Cmd+C)

### Step 2: Add to TradingView
1. Open [TradingView](https://tradingview.com)
2. Navigate to **Pine Editor** (bottom panel)
3. Click **"New"** to create a new indicator
4. Paste the copied code
5. Click **"Save"** and give it a name
6. Click **"Add to Chart"**

### Step 3: Configure Settings
The indicator has multiple configuration groups:

#### Essential Settings to Configure First:
1. **Breakout Detection**: Adjust lookback length (14) and range multiplier (1.5)
2. **FVG Settings**: Set your preferred session time and colors
3. **CRT Timeframes**: Enable/disable timeframes relevant to your trading
4. **CRT Labels**: Set maximum labels and styles

#### Advanced Configuration:
- **Advanced FVG**: Configure threshold and mitigation settings
- **CISD**: Customize line styles and colors
- **CRT Time Analysis**: Enable specific hour analysis
- **HTF Candles**: Set higher timeframe visualization

### Step 4: Set Up Alerts (Optional)
1. Right-click on chart → **"Add Alert"**
2. Select the indicator from the dropdown
3. Choose desired alert conditions:
   - Breakout signals
   - CRT touches
   - FVG formations
   - CISD changes

## Recommended Settings by Trading Style

### Scalping (M1-M5 charts)
```
Breakout Detection: Length=5, Multiplier=1.2
CRT Timeframes: Enable H1, H4, Daily only
Advanced FVG: Threshold=0.5%, Dynamic=true
CRT Time Analysis: Enable=true
```

### Day Trading (M15-H1 charts)
```
Breakout Detection: Length=14, Multiplier=1.5
CRT Timeframes: Enable H1, H4, Daily, Weekly
Advanced FVG: Threshold=1%, Show Dashboard=true
CISD: Enable statistics table
```

### Swing Trading (H4-Daily charts)
```
Breakout Detection: Length=20, Multiplier=2.0
CRT Timeframes: Enable Daily, Weekly, Monthly
Advanced FVG: Threshold=2%, Mitigation Levels=true
HTF Candles: Enable for higher timeframe context
```

## Troubleshooting

### Common Issues:

**1. Indicator not loading**
- Check Pine Script version is v6
- Ensure all code is copied correctly
- Verify chart has sufficient history (5000+ bars)

**2. Too many lines/labels error**
- Reduce max_labels setting in CRT options
- Disable unnecessary timeframes
- Lower historical days in FVG settings

**3. Performance issues**
- Disable HTF candle visualization if not needed
- Reduce number of active timeframes
- Lower max_bars_back if chart allows

**4. Alerts not working**
- Ensure alert conditions are properly configured
- Check TradingView alert limits
- Verify indicator is added to chart before setting alerts

### Performance Optimization:

For better performance on lower-end devices:
1. Disable HTF Candle Visualization
2. Limit CRT timeframes to 3-4 maximum
3. Set FVG max days to 1-2
4. Reduce max labels to 20-30
5. Disable dashboards if not needed

## Support

For technical issues:
1. Check TradingView Pine Script documentation
2. Verify your TradingView plan supports custom indicators
3. Ensure browser/app is updated to latest version

## Updates

To update the indicator:
1. Replace the old code with new version
2. Save the indicator
3. Refresh the chart
4. Reconfigure settings if needed

---

*Note: This indicator is provided as-is. Always test on paper trading before using with real money.*