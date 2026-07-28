Here is a complete, structured, and in-depth guide to understanding and using Bollinger Bands for trading. It covers everything from the foundational concepts to advanced strategies, risk management, and common pitfalls.

---

### 1. What Are Bollinger Bands?

Bollinger Bands are a technical analysis tool developed by John Bollinger in the early 1980s. They consist of three lines plotted on a price chart:

- **Middle Band:** A simple moving average (SMA), typically 20 periods.
- **Upper Band:** Middle Band + (Standard Deviation × a multiplier), typically 2.
- **Lower Band:** Middle Band – (Standard Deviation × a multiplier), typically 2.

The bands are dynamic support and resistance levels that expand and contract based on market volatility. Their primary purpose is to provide a relative definition of high and low prices, allowing traders to assess whether prices are relatively high or low compared to recent history, while also visualizing volatility.

---

### 2. Calculation and Parameters

Understanding the math behind the indicator is crucial to interpreting it correctly.

**Formula:**
- Middle Band = 20-period Simple Moving Average (SMA) of closing prices.
- Upper Band = Middle Band + (20-period Standard Deviation × 2)
- Lower Band = Middle Band – (20-period Standard Deviation × 2)

**Key Parameters:**
- **Period (default 20):** Determines the lookback for the moving average and standard deviation. A shorter period (e.g., 10) makes the bands more responsive and tighter, while a longer period (e.g., 50) makes them smoother and slower to react.
- **Standard Deviation Multiplier (default 2):** Sets the width of the bands. Statistically, with a 20-period setting and normally distributed data, approximately 95% of price action should fall within the bands. Lowering it to 1.5 would contain about 87% of prices, making touches more frequent. Raising it to 2.5 or 3 captures more extreme moves.
- **Moving Average Type:** The classic setting uses a Simple Moving Average (SMA), but Exponential (EMA) can be used for more weight on recent prices. John Bollinger recommends the SMA for consistency.

---

### 3. Core Concepts and Interpretation

To "learn and understand" Bollinger Bands, you must internalize these three foundational principles:

#### A. Volatility Visualization (Expansion and Contraction)
- **Contraction (The Squeeze):** When the bands narrow significantly, it signals a period of low volatility. This is often a precursor to a sharp price move in either direction. The squeeze does *not* predict the direction, only that a breakout is imminent.
- **Expansion:** When the bands widen sharply, it confirms a high-volatility move is underway. Prices will often "ride" the bands, with the upper band acting as dynamic resistance in an uptrend and the lower band as support in a downtrend.

#### B. Relative Definition of High and Low
- A tag of the upper band, by itself, is not a sell signal. In a strong uptrend, price can walk up the band, indicating extreme strength.
- A tag of the lower band is not automatically a buy signal; in a downtrend, price can walk down the lower band.
- Bollinger Bands answer the question: “Is price high or low on a relative basis?” They must be combined with other tools to judge the trend and momentum.

#### C. Mean Reversion vs. Trend Continuation
- In a ranging (sideways) market, price tends to revert to the middle band after touching an outer band. This is the basis for “fade” strategies.
- In a strongly trending market, price hugs an outer band and rarely touches the middle band. Trying to fade the band in such an environment leads to disaster.

---

### 4. The Three Essential Trading Strategies

John Bollinger himself teaches these core setups. Master these before adding complexity.

#### Strategy 1: The Bollinger Bounce (Mean Reversion)
- **Market Condition:** Range-bound, non-trending market. Confirmed by a flat middle band or an ADX below 20.
- **Setup:** Price touches or closes outside the lower band, then an upward reversal candle forms (bullish engulfing, hammer, etc.). The trade is a long entry, targeting the middle band.
- **Confirmation:** Look for a change in momentum, e.g., RSI moving up from oversold, a bullish divergence, or increased volume on the reversal candle.
- **Short Version:** Price touches upper band in a range, bearish reversal candle appears, target middle band.
- **Stop Loss:** Just beyond the extreme of the reversal candle or a few ticks beyond the band.

#### Strategy 2: The Bollinger Squeeze (Volatility Breakout)
- **Market Condition:** Bands are at their narrowest in the last 6 months (can be quantified using BandWidth indicator). This is the calm before the storm.
- **Setup:** Wait for a close decisively outside the bands (closing above the upper band or below the lower band) *after* a prolonged squeeze. This signals a volatility breakout.
- **Directional Filter:** Use volume surge and an indicator like the ADX (rising above 25) or a momentum oscillator to confirm the breakout direction. A close above the upper band with massive volume is a strong bullish continuation signal.
- **Target:** Ride the trend until price closes back inside the bands or touches the middle band, or use a trailing stop.
- **Failed Squeeze:** If price breaks out but immediately reverses and closes back inside the bands, it’s a head fake—often a powerful signal in the opposite direction.

#### Strategy 3: Walking the Bands (Trend Continuation)
- **Market Condition:** Strong, established trend. Middle band is sloping steeply. Price repeatedly touches or closes near the outer band without meaningful pullbacks.
- **Setup:** In an uptrend, price pulls back *only* to the middle band (not the lower band), finds support, and forms a continuation candle (e.g., a bull flag). Enter long with a target near the upper band.
- **Rules:** The middle band acts as dynamic support in an uptrend and dynamic resistance in a downtrend. A failure to hold the middle band often signals a trend weakening or reversing.
- **Exit:** When price finally breaks and closes on the other side of the middle band against the trend, the walk is over.

---

### 5. Advanced Concepts and Companion Indicators

No indicator works in isolation. Bollinger Bands provide a framework; other tools give the signals.

#### %b (Percent B)
This indicator tells you precisely where price sits relative to the bands.
- **Formula:** %b = (Closing Price – Lower Band) / (Upper Band – Lower Band)
- **Values:** 
  - %b = 1.0 means price is at the upper band.
  - %b = 0.0 means price is at the lower band.
  - %b > 1.0 means price is above the upper band (a “tag” from outside).
  - %b < 0.0 means price is below the lower band.
- **Use:** It’s essential for quantifying setups. A “tag” is %b > 1 or < 0. Also, look for divergences: price makes a higher high but %b makes a lower high, warning of waning momentum.

#### BandWidth
This measures the width of the bands as a percentage of the middle band.
- **Formula:** BandWidth = (Upper Band – Lower Band) / Middle Band
- **Use:** It directly identifies the squeeze. The lowest BandWidth reading over a lookback period (e.g., 125 days) flags the setup. A sudden spike in BandWidth confirms the expansion.

#### Combining with Other Indicators (The Bollinger Band Toolkit)
- **Volume:** A breakout from a squeeze without volume expansion is suspect. A reversal tag must show a volume climax or spike to be reliable.
- **RSI (Relative Strength Index):** Use to confirm overbought/sold conditions on band tags in ranges. In a walk-the-bands trend, RSI will stay overbought (above 70) for a long time, which is a sign of strength, not weakness.
- **MACD:** A moving average crossover can help confirm a trend reversal after a band tag. The signal line crossover near the middle band offers an entry.
- **Price Patterns:** Double bottoms and tops are powerfully confirmed by Bollinger Bands. A classic “W” bottom in a downtrend forms when the first low is at or below the lower band, the pullback stalls at the middle band, and the second low is *above* the lower band (a higher low relative to the bands). This is a high-probability reversal pattern. The opposite for an “M” top.

---

### 6. Timeframe Selection and Multi-Timeframe Analysis

- **Intraday Trading (1-min, 5-min, 15-min):** Bollinger Bands work well but are noisier. Use standard settings (20,2). The middle band on a 5-min chart acts as strong intraday trend support/resistance.
- **Swing Trading (1-hour, 4-hour, Daily):** The classic timeframe. The 20,2 settings on the daily chart capture two standard deviations over roughly a month of trading days, which is statistically robust. End-of-day tags on the daily lower band with a reversal candle form reliable swing lows.
- **Position Trading/Investing (Weekly, Monthly):** Use weekly Bollinger Bands to identify major market tops and bottoms. A monthly lower band tag with %b turning up is a rare, high-conviction long-term buy signal.
- **Multi-Timeframe Analysis:** The most powerful approach. 
  - Identify the macro trend on a higher timeframe (e.g., daily band slope).
  - Enter on a lower timeframe pullback (e.g., 1-hour tag of the middle band in the direction of the daily trend).
  - A squeeze on a higher timeframe broken on a lower timeframe is exceptionally explosive.

---

### 7. Risk Management and Trade Parameters

- **Stop Loss Placement:** When fading an outer band, place the stop just beyond the extreme of the reversal candle or beyond the band. When trading a squeeze breakout, the stop often goes inside the bands, below the breakdown level of the squeeze range.
- **Targets:** 
  - Mean reversion trades: Target the middle band. Scale out partially there, then hold a runner for the opposite band only if the market remains range-bound.
  - Breakout trades: Use a trailing stop (e.g., a 2-period ATR stop) or wait for a close on the opposite side of the middle band.
- **Position Sizing:** Because a squeeze breakout can whip, consider entering with a smaller size initially and adding once the breakout is confirmed and the bands are expanding.
- **False Signals:** Bollinger Bands give many false signals in choppy markets. The best filter is market regime: use trend identification (ADX, moving average slope, or visual inspection) to choose the right strategy. Do not use bounce strategies in a strong trend, and do not chase breakouts in a dead range.

---

### 8. Common Mistakes to Avoid

1. **Treating Band Tags as Automatic Overbought/Oversold Signals** – In a trend, they indicate strength, not exhaustion.
2. **Ignoring the Middle Band** – It is the anchor of the system, acting as support/resistance and a reversion magnet. When prices bounce between the middle and an outer band in a trend, it’s a sign of health.
3. **Using the Bands Without Confirmation** – Never enter solely because price touched a band. Wait for a price pattern, candlestick confirmation, or volume signal.
4. **Forgetting the Statistical Assumption** – Price can and does spend extended periods outside the bands. The 95% containment is theoretical and assumes a normal distribution; markets are fat-tailed.
5. **Over-Optimizing Parameters** – Stick to 20,2 unless you have a statistically validated reason to change. John Bollinger emphasizes that 20,2 works across all markets and timeframes if you know how to interpret them.

---

### 9. Practical Learning Path: How to Master Bollinger Bands

To truly understand them, follow this process:

1. **Read the Original Source:** John Bollinger’s book *Bollinger on Bollinger Bands* is the definitive guide. No secondary source can replace it.
2. **Memorize the Rules:** Bollinger’s 22 rules for using the bands are a checklist every trader should know. A few critical ones: “Bollinger Bands are not a standalone system.” “Tags of the bands are just tags, not signals.” “A close outside the bands is a continuation signal, not a reversal, unless proven otherwise.”
3. **Manual Backtesting:** Open a daily chart, scroll back in time, and manually walk through each day, noting band relationships, %b, and volume. Record what happens next. Do this for at least 100 trades.
4. **Paper Trade Using a Protocol:** Define exactly which strategy you are trading (e.g., “squeeze breakout only on daily chart, confirmed by volume > 1.5x average”). Journal every trade, recording the BandWidth at entry, %b at entry/exit, and the outcome.
5. **Integrate Slowly:** Start with just Bollinger Bands and volume. Master that before adding RSI or MACD. The goal is to understand what the bands are telling you, not to clutter your screen.

---

### Summary of the Bollinger Band Framework

- **Middle Band:** The trend and reversion point.
- **Upper/Lower Bands:** Dynamic extremes that expand with volatility and contract during consolidation.
- **Squeeze:** Low volatility warns of imminent expansion; trade the breakout with volume.
- **Bounce:** Works only in mean-reverting, range-bound markets; fade extreme tags with reversal confirmation.
- **Walk:** In trends, price respects the middle band as support/resistance, not the outer band.
- **Never Forget:** Bollinger Bands provide context about relative price levels and volatility. The signal must come from price action and complementary indicators.

Mastering Bollinger Bands is a journey in understanding market volatility and relative value, not memorizing a list of trade setups.