# speculatorlab
Backtest your trading strategies

Ruby based backtesting engine that you can test your trading strategies against.

```
require "trader"

include Trader

s = Strategy.new("My strategy") do
  buy(stop: (close - 10)) if close > 100
  sell(stop: (close + 10)) if close < 100
end
```
