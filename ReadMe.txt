*** Finished bare bones for now, good for basics. Functions still chonky. Can do general cleanup, but functionality all works.***


Works good on 5 min and 60 min data, should work fine on any other timeframe as well. 
Change the ATR wiggle room or weighted mean of how candle sticks are measured to change the strictness of the definition of a horizontal resistance line.

1. Loads data.
2. Finds Horizontal resistance lines by finding first two points.
3. Finds the rest of the points.
4. Calculates returns from an entry at the 3rd touchpoints close. (Useful when have bulk data - to help optimize strategy ideas)
5. Calculates trading results based on a sample/basic strategy.
6. graphs the candlestick chart with all the line and trade info. Graphs returns plot for entries over time.

Details: 'touch points' for horizontal lines aren't going to be perfect. Weighted the touch based on mixes of ATR and weighted mean between high and close or low and close, depending on what was needed. Minimum distance between distinct 'touches' was set to 10 candles.

Notes: Returns calculation was necessary even if not used directly in calculating trading results, to see if for example, 'returns after 3rd point', could possibly yield good results. So then a trading strategy was applied to that. The function that calculates returns is basically a rough probe to see what's out there and if a trading strategy in that general area should be applied.