# 📥 Step 1: Data Comes First

Before we train models, backtest strategies, or build classifiers, the first step is **always** data collection.

Trading systems — especially those involving structure classification or event detection — are only as good as the data they learn from. Garbage in, garbage out.

## 🔍 Why Data Gathering Matters

- 🧠 Models trained on **random candles** without context will chase noise  
- 🏗️ Understanding **market structure** requires clean, multi-timeframe data  
- 🧾 Event classification (spoofs, reversals, squeezes) requires **labeling** and **human insight**  
- ⏱️ Different timeframes give different truths: 1-minute noise can signal daily intent

---

## ✅ What This Stage Involves

- Collecting raw OHLCV data (1m, 5m, 15m, 1h, daily)
- Tagging key events: consolidations, fakeouts, volume shifts, etc.
- Logging price reactions to news, volume spikes, liquidity gaps
- Preparing this data for feature extraction, visualization, and eventual model input

---

## ⚠️ If You Skip This Step...

> You’ll end up building a model that “works” on backtest charts — but fails the moment you try to understand *why* it made a trade.

So this repo starts with a simple truth:

> **Don’t build a classifier until you’ve studied what you’re trying to classify.**
