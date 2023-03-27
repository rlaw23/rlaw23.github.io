---
layout: page
title: QuantConnect vs Backtrader
parent: Algo Trading
nav_order: 2
---

## Why I chose QuantConnect over Backtrader
Backtrader, backtesting.py, and QuantConnect all utilize a similar bar-by-bar streaming approach to backtesting data. While these packages share many similarities, each has unique strengths and weaknesses that make them better suited for certain use cases.

<br/>

### Backtesting.py
Initially, I explored the backtesting.py package due to its simplicity and informative examples on the official site. While backtesting.py has the least steep learning curve among the three, it gave me a valuable understanding of the general working of backtesting packages. However, I quickly discovered that it is not capable of handling multi-asset strategies, which led me to search for alternatives.

### Backtrader
Backtrader offers a more robust set of capabilities compared to backtesting.py, including multi-asset trading and live trading connectivity, making it a suitable choice for more advanced traders. However, its official forums are replete with spam, and its Github repository has not seen new commits in some time, which became a concern to me.

### QuantConnect
QuantConnect, on the other hand, offers several advantages over both Backtrader and backtesting.py. The most significant one being its cloud-hosted data which eliminates the need to separately retrieve data from platforms like IBKR or SimFin, saving traders valuable time. QuantConnect has prebuilt execution, insight and risk management modules which greatly help traders to spin up a working algorithm in the short time. Additionally, QuantConnect has an active community that is always sharing ideas which are important for individual traders looking for stimulation. As QuantConnect is a profit-making company, it's motivated to keep its platform up-to-date and add new features.