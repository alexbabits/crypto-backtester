                                                    HORIZONTAL RESISTANCE LINES

Notes:
- Think of more ways to improve trading strategy for horizontal lines
- Last thing to do is adjust functions to take in multiple coin pair df's at once. And download+save other pairs/coins data.

Flexibility in general:
- Can input any timeframe.
- Can change entry/exits/trading strategy/fees/etc.

Flexibility of identifying horizontal resistance line:
- Can change the percentage of ATR for line price for candle touch points.
- Can change weighted mean for line price and candle touch area based on any mix of OHLC.
- Can change waiting period which determines minimum wait time between touch points, helps avoid clumps of near candles counting as multiple touches.

Ideas:
- Horizontal Support Lines (Very similar to Horiontal Resistance Lines).
- Horizontal Channels: Horizontal support+resistance lines using this code.
- Slanted Channels: non-zero slope support+resistance lines would create channels. Probs use horizontal line ideas and least squares combined.
- ML could/will be used to optimize Entry/SL/TP/trailing SL levels, based on the features (indicators) and target ('returns' or 'net_pl_with_fee').

Overview: 
0. Bulk test data (BTC-USDT and ETH-UDST) already loaded in csv. Do not re-run binance API.
1. Load in csv and make OHLC+indicators df (btc_usdt_df for example).
2. Finds Horizontal resistance lines by finding first two points.
3. Finds the rest of the touch points.
4. Calculates trading results based on a sample/basic strategy.
5. Calculates analysis from entry point.
6. Graphs/Charts.

Useful tools/gpt plugins:
https://askyourpdf.com/upload


