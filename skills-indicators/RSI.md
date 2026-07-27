Here is a complete, detailed, and comprehensive guide to learning and deeply understanding the **RSI (Relative Strength Index)**. It covers everything from the basics to advanced concepts, formulas, signals, limitations, and combination strategies.

---

## 1. Definition and History

**RSI** stands for **Relative Strength Index**, a momentum oscillator that measures the speed and magnitude of price changes. It was developed by **J. Welles Wilder** and introduced in his 1978 book *New Concepts in Technical Trading Systems*.  
The RSI oscillates between **0 and 100**, and its primary goal is to gauge the **internal strength and weakness** of an asset based solely on closing prices over a specified look-back period.

---

## 2. Calculation Formula – Step by Step

The RSI calculation uses a smoothed average of gains and losses (Wilder’s smoothing method).

### Step 1: Choose the Period (n)
The default period is **14** (Wilder suggested 14 days for daily charts). For other timeframes you can adjust *n* (e.g., 9 or 21).

### Step 2: Calculate Price Changes (Δ)
For each bar, the change relative to the previous bar:  
Δ = Close<sub>today</sub> – Close<sub>yesterday</sub>

### Step 3: Separate Gains and Losses
- If Δ > 0 → **Gain** = Δ, Loss = 0  
- If Δ < 0 → **Loss** = |Δ|, Gain = 0  
- If Δ = 0 → both = 0

### Step 4: Initial Average Gain and Loss
For the first *n* periods, use a simple average:  
**First Average Gain** = Sum of Gains over *n* periods / *n*  
**First Average Loss** = Sum of Losses over *n* periods / *n*

### Step 5: Smoothed Averages (Wilder’s Method)
From bar *n+1* onward, use the following smoothing formula (effectively an EMA with α = 1/*n*):  

**New Average Gain** = [(Previous Average Gain × (*n*–1)) + Current Gain] / *n*  
**New Average Loss** = [(Previous Average Loss × (*n*–1)) + Current Loss] / *n*

> Note: This method provides a good balance between responsiveness and stability.

### Step 6: Calculate Relative Strength (RS)
**RS** = Average Gain / Average Loss  
(If Average Loss equals zero, RS is infinite and RSI is set to 100.)

### Step 7: Convert to RSI
**RSI = 100 – (100 / (1 + RS))**

This formula ensures the RSI always stays between 0 and 100.  
- If all periods are gains (Average Loss = 0) → RSI = 100  
- If all periods are losses (Average Gain = 0) → RSI = 0  
- RS = 1 (Average Gain = Average Loss) → RSI = 50

---

## 3. Numerical Example (5-period for simplicity)

| Bar | Close | Change (Δ) | Gain | Loss |
|-----|-------|------------|------|------|
| 1   | 44    | -          | -    | -    |
| 2   | 46    | +2         | 2    | 0    |
| 3   | 45    | –1         | 0    | 1    |
| 4   | 47    | +2         | 2    | 0    |
| 5   | 49    | +2         | 2    | 0    |

First Average Gain = (2+0+2+2)/5 = 1.2  
First Average Loss = (0+1+0+0)/5 = 0.2  
Initial RS = 1.2 / 0.2 = 6  
Initial RSI = 100 – (100 / (1+6)) = 100 – 14.29 ≈ **85.71**

For bar 6, if price drops to 48 (Δ = –1, Gain=0, Loss=1):  
New Avg Gain = [(1.2 × 4) + 0] / 5 = 0.96  
New Avg Loss = [(0.2 × 4) + 1] / 5 = 0.36  
RS = 0.96 / 0.36 = 2.667  
RSI = 100 – (100 / 3.667) ≈ **72.7**

And so on.

---

## 4. Basic Interpretation and Classic Levels

### Overbought and Oversold Zones
- **RSI > 70** → Overbought zone. Price has moved up strongly; a pause, correction, or reversal is likely. (Excessive buying pressure)
- **RSI < 30** → Oversold zone. Heavy selling pressure; a bounce or reversal upward is likely.
- Many traders focus on the *exit* from these zones (e.g., crossing back below 70 as a sell signal, or above 30 as a buy signal) rather than just being inside them.

### The 50 Centerline
- **RSI above 50** → Buyers are in control; medium-term uptrend.
- **RSI below 50** → Sellers dominate; medium-term downtrend.
- A cross of the 50 line can confirm a trend change.

### RSI Ranges
- An RSI oscillating between **40 and 60** usually indicates a sideways, range-bound market.
- In strong trends, RSI can stay in the 70–80 or 20–30 zones for extended periods, rendering the classic levels less useful without adjustment.

---

## 5. Period Settings – Impact on Sensitivity

| Period | Characteristics |
|--------|-----------------|
| **14 (default)** | Good balance between signal and noise; suitable for most markets and timeframes. |
| **9 or 10** | More sensitive, more signals but more noise; good for scalping or lower timeframes. |
| **21 or 25** | Smoother, fewer but stronger signals; suitable for longer-term trends. |
| **2** | Used for quick directional change detection; sometimes plotted alongside the main RSI to pinpoint micro-tops/bottoms. |

---

## 6. Core Trading Signals (4 Foundational Wilder Signals Plus Extras)

### 1. Overbought/Oversold Crossovers (Classic)
- **Buy Signal:** RSI moves from below 30 back above 30 (exit from oversold).
- **Sell Signal:** RSI falls from above 70 back below 70.
- Weakness: These signals fail frequently in strongly trending markets.

### 2. Centerline Crossovers (50 Level)
- **RSI rising above 50:** Bullish momentum strengthening.
- **RSI falling below 50:** Bearish momentum increasing.
- Best used in conjunction with trendline breaks on price.

### 3. Divergence – The Most Predictive Signal
Divergence occurs when price and RSI move in opposite directions.

#### Regular Divergence
- **Bearish Divergence:** Price makes a Higher High, but RSI makes a Lower High → weakening momentum, potential downward reversal.
- **Bullish Divergence:** Price makes a Lower Low, but RSI makes a Higher Low → selling pressure weakening, potential upward reversal.

> Crucial: Divergence carries more weight when it occurs near overbought/oversold zones (around 70/30). Confirmation via a trendline break on price or RSI is essential.

#### Hidden Divergence – Trend Continuation
- **Hidden Bullish Divergence:** Price makes a Higher Low, but RSI makes a Lower Low → confirms the uptrend and signals the end of a pullback.
- **Hidden Bearish Divergence:** Price makes a Lower High, but RSI makes a Higher High → confirms the downtrend and signals a sellable pullback.

#### Advanced (Extended) Divergence (Cardwell)
- Class A: Regular divergence.
- Class B: Hidden divergence.
- Class C: Price forms a double top/bottom but RSI shows a different move, often producing stronger signals.

### 4. Failure Swings – Wilder’s Own Pattern
This pattern warns of a reversal without the price needing to breach its prior swing point:
- **Top Failure Swing:**  
  1. RSI enters overbought (above 70).  
  2. RSI pulls back and makes a trough.  
  3. RSI rallies again but fails to exceed its previous overbought peak.  
  4. RSI then breaks below the prior pullback trough → **Sell signal**.
- **Bottom Failure Swing:** The opposite, starting below 30. RSI makes a higher trough during an oversold bounce and then breaks above the prior swing high.

### 5. Positive and Negative Reversals (Cardwell)
- **Positive Reversal:** Price makes a lower low, but RSI makes a much higher low, and then RSI breaks above its own breakout level → strong bullish strength.
- **Negative Reversal:** Price makes a higher high, RSI makes a lower high, and RSI breaks support.

### 6. Support and Resistance on RSI Itself
Just like price, the RSI line can have its own support/resistance levels and trendlines. A trendline break on RSI often precedes a trendline break on price, offering early warning.

---

## 7. RSI in Trending Markets – Dynamic Level Adjustments

In strong trends, RSI can remain overbought/oversold for a long time. To adapt:
- **Strong Uptrend:** Consider oversold not at 30 but at **40** or even **45**. Keep overbought at 70 or 80.
- **Strong Downtrend:** Consider overbought at **60** or **55**, and oversold at 30 or 20.
- Using a moving average of RSI (e.g., 9-period) can help identify the dominant trend’s direction and strength.

---

## 8. Advanced Concepts and Special Techniques

### 1. Smoothed RSI
Some platforms allow you to overlay a moving average on the RSI line. A cross of RSI above/below its own moving average acts like a MACD-style signal, giving bullish/bearish pulses.

### 2. Multiple Timeframe RSI
Aligning RSI signals across higher and lower timeframes multiplies their reliability. For example, daily RSI shows bullish divergence and the 1-hour RSI exits oversold.

### 3. RSI Range Behavior (Constance Brown)
- In bull markets, RSI typically oscillates between **40 and 90**, with 40 acting as strong support.
- In bear markets, between **10 and 60**, with 60 acting as a ceiling/resistance.

### 4. Using RSI as a Range Finder
If RSI consistently bounces between 40 and 60, the market is likely in a range, and other oscillators (like Stochastics) may be more effective. A breakout from this range signals the start of a trend.

### 5. Price Patterns on RSI
Chart patterns such as head and shoulders, triangles, and flags often appear on the RSI indicator itself. Their breakouts are interpreted the same way as on price.

### 6. Comparative/Internal RSI
Combining RSI with a comparative relative strength measure to compare two assets' strength.

---

## 9. Limitations of RSI

- **Inherent Lag:** Based on past prices, it is a lagging indicator; signals may be delayed.
- **False Signals in Strong Trends:** Prolonged overbought/oversold readings can generate multiple false reversal signals without filtering.
- **Repeated Divergences:** Price may continue moving while RSI prints divergence three or more times. Structural confirmation (e.g., trendline break) is necessary.
- **Sideways vs. Trending Markets:** Fixed 70/30 levels work well in ranges but poorly in trends. Dynamic adjustment is required.
- **Price Gaps:** Calculations rely entirely on closing prices; overnight gaps aren't directly factored into the smoothing.

---

## 10. Combining RSI with Other Tools (Increasing Reliability)

Never trade RSI alone. The best combinations:

| Complementary Tool | How to Use |
|--------------------|-------------|
| **Moving Averages (MA)** | RSI shows bullish divergence, and price crosses above a key MA (200 or 50). |
| **Horizontal Support/Resistance** | RSI signals near major S/R zones have higher success rates. |
| **Fibonacci** | Oversold RSI exit coincides with a bounce from a Fibonacci retracement level. |
| **MACD** | RSI divergence confirmed by a MACD crossover boosts signal strength. |
| **Volume** | Decreasing volume during bearish divergence adds confirmation. |
| **Candlestick Patterns** | RSI exits oversold with a Hammer candle → excellent buy setup. |
| **Bollinger Bands** | RSI oversold and price at lower Bollinger Band → reversal opportunity. |

---

## 11. Practical Trading Strategies (Examples)

### Strategy 1: Divergence + Trendline Break
1. Use 4-hour or daily timeframe.
2. Identify regular bullish divergence (price lower low, RSI higher low) below 30.
3. Draw a descending trendline on price.
4. Enter long when price breaks the trendline and closes above it.
5. Stop-loss below the recent swing low; target at next resistance.

### Strategy 2: RSI(2) Scalping Technique
- Set RSI period to 2.
- Buy: RSI(2) crosses back above 5 (or 10) from below.
- Sell: RSI(2) crosses below 95 from above.
- Best executed in the direction of the higher timeframe trend.

### Strategy 3: RSI + 50 Level with 200 MA Filter
- Only go long if price is above the 200 MA and RSI consolidates above 50.
- Only go short if price is below the 200 MA and RSI holds below 50.

---

## 12. Visual Display and Interpretation Tips

- Plot fixed horizontal lines at 30 and 70 (and optionally 50).
- RSI line oscillates; divergences are drawn with trendlines connecting peaks/troughs on both price and RSI.
- Some platforms shade the 50 area.
- It's best displayed as a line (not histogram) with conditional coloring (e.g., red above 70, green below 30).

---

## 13. Final Points and Summary

- RSI is a **momentum oscillator**, not a pure directional tool. It measures the *strength* behind the move.
- Use it as a **filter or confirmation tool**, never as the sole reason to enter a trade.
- High-timeframe divergences (4-hour, daily) tend to be more reliable.
- No indicator is perfect; always use proper risk management and stop-losses.
- To gain a deep understanding, manually calculate the RSI for a few periods. This cements the concept of "smoothed average gain and loss."
- Study the original works by Wilder and Cardwell for deeper insight.

By mastering these concepts, you don't just learn how to use RSI — you learn the **philosophy behind it**: price is not just a number, but a reflection of the ongoing battle between buyers and sellers, which RSI quantifies.