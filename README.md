Pair Trading Strategy (GitHub)

Identified pairs of stocks with co-movement properties, modeling the spread and ratio relationships to quantify relative price behavior.

Applied linear regression to model expected spread, computed residuals (error series), and used Augmented Dickey-Fuller (ADF) test to ensure stationarity (i.e. mean reversion of the residual series). 
Zerodha

Constructed a trade trigger: when the residual diverges beyond ± k standard deviations (signal threshold), enter long-short pair (buy cheap, short expensive), expecting reversion.

Defined exit rules based on mean reversion or residual crossing back toward zero.

Backtested across multiple stock pairs/market regimes, tracking metrics such as Sharpe ratio, drawdown, and win rate.

Integrated signal generation into pipeline using Python (Pandas, statsmodels).

Achieved consistent relative value alpha with robust risk controls (max drawdown bounds, entry size limits).
