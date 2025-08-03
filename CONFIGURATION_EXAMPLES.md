# Configuration Examples

## Trading Style Configurations

### 1. Scalping Setup (1-5 min charts)

#### Breakout Detection
```
Lookback Length: 5
Range Multiplier: 1.2
```

#### FVG Settings
```
Session: "0930-1600"
Box Color Up: Green (80% transparency)
Box Color Down: Red (80% transparency)
Max Days: 1
Draw NY Open: true
```

#### CRT Timeframes
```
Enable: H1, H4, Daily only
H1 Color: Orange
H4 Color: Blue  
Daily Color: Purple
50% Levels: enabled for all
```

#### CRT Labels
```
Max Labels: 20
Bullish Style: Triangle Up
Bearish Style: Triangle Down
Size: Small
```

#### Advanced FVG
```
Threshold: 0.5%
Auto: false
Dynamic: true
Show Dashboard: true
```

#### CRT Time Analysis
```
Enable: true
Check Large Candles Only: true
Max Wick Ratio: 0.3
```

---

### 2. Day Trading Setup (15m-1H charts)

#### Breakout Detection
```
Lookback Length: 14
Range Multiplier: 1.5
```

#### FVG Settings
```
Session: "0932-1600"
Max Days: 2
Draw NY Open: true
Draw Opening Price: true
```

#### CRT Timeframes
```
Enable: H1, H2, H4, Daily, Weekly
Colors: Distinct colors for each TF
Line Width: 2
Mid Line Width: 1
50% Levels: enabled
```

#### CRT Options
```
Minimum Bars: 3
Maximum Bars: 200
Touch Detection: Both wick and body
```

#### Advanced FVG
```
Threshold: 1.0%
Unmitigated Levels: 5
Mitigation Levels: true
Show Dashboard: true
Location: Top Right
```

#### CISD Settings
```
Bull CISD Color: Green
Bear CISD Color: Red
Line Width: 2
Line Extension: 10 bars
Statistics Table: enabled
```

---

### 3. Swing Trading Setup (4H-Daily charts)

#### Breakout Detection
```
Lookback Length: 20
Range Multiplier: 2.0
```

#### FVG Settings
```
Session: "0932-1600"
Max Days: 5
All drawing options: enabled
```

#### CRT Timeframes
```
Enable: Daily, Weekly, Monthly
2D: enabled
Colors: Professional color scheme
Line Widths: 3 (high/low), 2 (mid)
```

#### CRT Labels
```
Max Labels: 50
Show all timeframe labels: true
End-of-line labels: true
Offset: 10
```

#### Advanced FVG
```
Threshold: 2.0%
Unmitigated Levels: 10
Mitigation Levels: true
Dashboard: enabled
Size: Normal
```

#### HTF Candles
```
Enable: true
Timeframe: 1D (for 4H charts) or 1W (for Daily charts)
Max Display: 15
```

---

### 4. News Trading Setup

#### Breakout Detection
```
Lookback Length: 10
Range Multiplier: 2.5
```

#### CRT Time Analysis
```
Enable: true
Specific Hours: 6, 10, 14 (high impact news times)
Large Candle Filter: true
Max Wick Ratio: 0.2
```

#### Alert Configuration
```
All CRT alerts: enabled
FVG alerts: enabled
CISD alerts: enabled
Breakout alerts: enabled
```

---

### 5. Range Trading Setup

#### CRT Timeframes
```
Focus on: H4, Daily, Weekly
Touch Detection: Wick touch primary
Body touch: secondary confirmation
```

#### CRT Options
```
Minimum Bars: 10
Maximum Bars: 500
Conservative range validation
```

#### Advanced FVG
```
Threshold: 1.5%
Focus on mitigation levels
Dashboard tracking: enabled
```

---

### 6. Trend Following Setup

#### EMA Analysis
```
All EMAs enabled: 20, 50, 100, 200
Dynamic coloring: enabled
Labels: enabled
```

#### CISD Settings
```
Statistics table: enabled
Track market state changes
Alert on state changes: enabled
```

#### Multi-timeframe Analysis
```
Weekly and Monthly CRT: primary
Daily: secondary
Lower timeframes: confirmation only
```

---

## Performance Configurations

### High-Performance (Older devices)
```
- Disable HTF Candles
- Limit to 3 CRT timeframes
- Max labels: 15
- FVG max days: 1
- No dashboards
- Reduced line extensions
```

### Standard Performance
```
- Enable most features
- 4-5 CRT timeframes
- Max labels: 30-50
- FVG max days: 2-3
- Dashboards as needed
```

### Full Feature (Modern devices)
```
- All features enabled
- All 7 CRT timeframes
- Max labels: 100+
- FVG max days: 5
- All dashboards and statistics
- HTF candle visualization
```

---

## Alert Configurations

### Conservative Alerts
```
- CRT touches: Daily and Weekly only
- FVG: Formation only (not mitigation)
- CISD: State changes only
- Breakout: High threshold (2.0+)
```

### Active Trading Alerts
```
- All CRT timeframes
- FVG formation and mitigation
- All CISD alerts
- Breakout: Standard threshold (1.5)
- CRT sweeps: enabled
```

### High-Frequency Alerts
```
- All available alerts
- Lower thresholds
- Multiple timeframe confirmations
- Real-time notifications
```

---

## Visual Customization Examples

### Professional Theme
```
Colors:
- Bulls: #00ff88 (bright green)
- Bears: #ff4444 (bright red)  
- Neutral: #888888 (gray)
- Background: minimal transparency
- Lines: clean, consistent widths
```

### Dark Theme Optimized
```
Colors:
- Bulls: #4CAF50 (material green)
- Bears: #F44336 (material red)
- EMAs: contrasting colors
- Backgrounds: higher transparency
- Text: white/light colors
```

### High Contrast
```
Colors:
- Bulls: #00FF00 (pure green)
- Bears: #FF0000 (pure red)
- Lines: maximum width
- Labels: large size
- High transparency levels
```

---

## Risk Management Integration

### Position Sizing Helpers
```
- Use CRT ranges for stop loss placement
- FVG levels for entry refinement
- Multiple timeframe confirmation required
- CISD for trend bias
```

### Stop Loss Strategies
```
- Below/above CRT ranges
- FVG mitigation levels
- CISD invalidation points
- ATR-based from breakout levels
```

### Take Profit Targeting
```
- Next CRT level
- FVG fill targets
- Previous swing highs/lows
- Multiple timeframe resistance/support
```

---

*Remember: Always backtest any configuration before using in live trading. These are starting points that should be adjusted based on your specific market, timeframe, and trading style.*