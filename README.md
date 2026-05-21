# 🚀 Bakome Buy Sell Indicator – Advanced TradingView Signal Tool

**Pine Script v5** | EMA Crossovers | ATR Stop Loss | Risk‑Reward 1:3 | Intermediate TPs | Info Table | Alerts

![Animation top](assets/demo_animation_top.gif)

---

## 📌 Overview

The **Bakome Buy Sell Indicator** is a professional trading system for **TradingView** (Pine Script v5).  
It generates high‑confidence **BUY/SELL signals** based on EMA crossover, with **full position management**:

- ✅ Entry signal (with optional candle confirmation)
- ✅ Dynamic **Stop Loss** (ATR‑based)
- ✅ **Take Profit** with configurable Risk:Reward (default 1:3)
- ✅ **Intermediate TP levels** (visual dotted lines + labels)
- ✅ Real‑time **info table** (Status, Entry, SL, TP, current R:R)
- ✅ Alerts for every event (BUY, SELL, TP hit, SL hit, invalidation)

Perfect for **XAUUSD**, **forex**, **indices**, and any trending market.

---

## 🔧 Features

| Feature | Description |
|---------|-------------|
| **Fast / Slow EMA** | Green and orange moving averages (user‑adjustable lengths) |
| **Trend detection** | Bullish when fast EMA > slow EMA, bearish otherwise |
| **Candle confirmation** | Optional: require bullish/bearish candle for entry |
| **ATR Stop Loss** | Multiplier applied to ATR (default 0.5) |
| **Risk:Reward** | Configurable ratio (default 3:1) |
| **Intermediate TPs** | Visual dotted lines for partial profit levels |
| **Info Table** | Top‑right panel showing live position data |
| **Alerts** | Custom alerts for signals, TP, SL, invalidation |
| **Invalidation marker** | Yellow diamond when a signal is invalidated by opposite entry |

---

## ⚙️ Input Parameters

| Parameter | Default | Description |
|-----------|---------|-------------|
| Fast EMA | 5 | Period for fast EMA |
| Slow EMA | 13 | Period for slow EMA |
| ATR Period | 14 | Period for ATR calculation |
| SL Multiplier (ATR) | 0.5 | Stop loss distance = ATR × multiplier |
| Risk:Reward (R:R) | 3.0 | Reward = Risk × value |
| Require candle confirmation | true | Signal only if close > open (BUY) or close < open (SELL) |

---

## 📥 Installation

1. **Copy** the Pine Script code from `Bakome_Buy_Sell_Indicator_v5.pine`.
2. Open **TradingView** → Pine Editor (bottom panel).
3. **Paste** the code.
4. Click **“Add to Chart”**.
5. Customize settings via the indicator’s input dialog.

---

## 🖼️ Preview

![Animation bottom](assets/demo_animation_bottom.gif)

---

## 📊 How It Works

- The indicator waits for a **trend change** (fast EMA crosses slow EMA).
- If **candle confirmation** is enabled, it also checks that the closing price is above the opening price (for BUY) or below (for SELL).
- Once a signal triggers:
  - **Entry price** = current close
  - **Stop loss** = low/high ± ATR × multiplier
  - **Risk** = distance between entry and stop loss
  - **Final take profit** = entry ± risk × risk‑reward
- Intermediate TP lines are drawn at fractions of the total risk.
- A **floating table** shows position status, entry, SL, TP, and current R:R.
- **Alerts** can be set for BUY, SELL, TP hit, SL hit, or signal invalidation.

---

## 🧪 Recommended Use

- **Timeframe**: 15‑minute or 1‑hour
- **Assets**: XAUUSD (Gold), major forex pairs (EURUSD, GBPUSD), indices (US30, SP500)
- **Risk management**: never risk more than 1‑2% of your capital per trade.

---

## 📜 License

MIT – free for personal and commercial use.  
*Trade responsibly. Past performance does not guarantee future results.*

---

## 👤 Author

**Bakome** – open‑source developer and trading system designer.  
GitHub: [BAKOME-Hub](https://github.com/BAKOME-Hub)

---

![Animation bottom](assets/demo_animation_bottom.gif)  
*Place your own animated demo GIFs in the `assets/` folder.*
