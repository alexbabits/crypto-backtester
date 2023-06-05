                                                    HORIZONTAL RESISTANCE LINES

Notes:
- Cleaned up, functionality all works. Functions large & necessary. Difficult to breakup while maintaining functionality due to delicate conditions for line creation.

Flexibility of timeframes & trading entries:
- Works for all timeframes, need to specify a time interval in minutes with corresponding candle data.
- Can calculate returns and results based on OHLC from any touchpoint or candle near a touchpoint if needed.

Flexibility of identifying line:
- Can change the percentage of ATR for line price or candle touch areas.
- Can change weighted mean for line price and candle touch area based on any mix of OHLC.
- Can change waiting period which determines minimum wait time between touch points, helps avoid clumps of near candles counting as multiple touches.

Ideas:
- Horizontal Support lines would work very similarly
- Could make slope=0 channels with horizontal support+resistance lines using this code
- If can make slope=0 channels, then could also make slanted channels.
- Could be used as a base right now to create +EV trading strategy for resistance/support lines if bulk data is loaded instead of sample data.

Overview: 
1. Bulk data already loaded (30 months worth of BTC/USD and ETH/USD atm). Will get more coins after adjusting code to account for multiple coins at once.
2. Finds Horizontal resistance lines by finding first two points.
3. Finds the rest of the touch points.
4. Calculates returns from an entry point. (Useful when have bulk data to help optimize strategy ideas)
5. Calculates trading results based on a sample/basic strategy.
6. graphs the candlestick chart with all the line and trade info. Graphs returns plot for entries over time.