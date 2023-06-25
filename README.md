Trading Strategy is just an example of breakout of horizontal resistance line after 3rd touch point. Performs very poorly.
</br>
</br>

## **Overview** ##

0. DownloadData.ipynb to download bulk OHLC data from binance if needed.
1. Global Variables, OHLC Data, Calculate 'Simple/Objective' Indicators
2. Define & Calculate 'Complex/Subjective' Indicators (Ex: Horizontal Lines). (Per 250k rows of OHLC data takes ~2.5 mins to find them).
3. Define Trading Strategy (Per 250k rows can take 10 seconds to 2 mins+ to run depending on how many trades a strategy finds).
4. Analyzes Trading Results
    1. Candlestick Chart with Trades
    2. Trade Stats Calculations
    3. Cumulative Portfolio Value Graph, Underwater Plot, Rolling Risk Metrics
    4. Distribution of Daily Returns, Distribution of Randomly Sampled Trades
    5. Returns from Entry (Useful post-mortem)

</br>

## **Pictures** ##

</br>
</br>
You can zoom in on the graph in the code to check and make sure entries are correct. Plotly graphs don't show up in the code viewer in github.
</br>
</br>
<img src="Pictures/candlestickplot.png">
</br>
</br>
<img src="Pictures/candlescloseup.png">
</br>
</br>
<img src="Pictures/cumportvalue.png">
</br>
</br>
<img src="Pictures/underwaterplot.png">
</br>
</br>
<img src="Pictures/rollingsharpe.png">
</br>
</br>
<img src="Pictures/rollingsortino.png">
</br>
</br>
<img src="Pictures/rollingvolatility.png">
</br>
</br>
<img src="Pictures/dailyreturns.png">
</br>
</br>
<img src="Pictures/tradesampling.png">
</br>
</br>
<img src="Pictures/returns.png">
