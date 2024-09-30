# Milk and Money

A dairy farm's profits are subject to volatility, due fluctuations in their costs of production, like grain or energy prices. Similarly, the farm’s revenue is volatile due to fluctuation in their mailbox price. The mailbox price is the net price the farm receives for their milk after accounting for marketing fees, transportation costs, and other expenses. To reduce uncertainty in their operations, the farm can hedge using derivative instruments, primarily futures and options, that are offered on the Chicago Mercantile Exchange (CME).

Hedgers in a commodity market usually take one of two positions. “A short hedger is a market participant with an inherently long position in a commodity. A long hedger is a market participant with an inherently short position in a commodity” (Bittman 2013, p. 52). The farmers are short hedgers as they intend to sell the dairy they produce at some point in the future and want to protect the price they will receive for it in the cash (physical) market. 

As short hedgers, the farmers can hedge using futures contracts. “A futures contract is an agreement between two parties, a buyer and a seller, to exchange a standardized good, the commodity, for an agreed-upon price at a specific date in the future, the delivery date” (Bittman 2013, p. 4). By shorting (selling) futures the farmers can mitigate their risk of lower prices in the cash market. The farm locks in its profitability, as a loss in one market should be offset by a gain in the other (Yamey, 1971) – i.e. a reduced selling price in the cash market should be offset by gains in the futures market and an increased cash selling price will be offset by a loss in their futures position. The farm’s hedge is composed of their positions in both the cash and futures markets. 

While the short futures hedge mitigates the risk of falling selling prices, it eliminates their gains should market prices increase. An alternative hedge available to them is a long-put option strategy. The put option market provides the farmers with added flexibility, as they have the right, not the obligation, to sell a futures contract at a certain price. Due to this added flexibility, the put option strategy establishes a price floor while retaining the opportunity to realise gains should market prices increase (Hauser and Eales, 1987). However, to enter a put option position the farm must pay a premium. Some advanced price risk management strategies reduce the cost of a premium through a combination of a long put/short call, establish a price window. However, through this method the farmers are unable to fully capture the benefits of a rising market. 

As the farmers are unable to enter a futures contract directly based on their mailbox price, they must manage their risk indirectly, using a cross hedge. Therefore, when hedging it is desirable that the farmers’ mailbox price and the price of the product traded in the futures market are closely related (Anderson and Danthine, 1981). By calculating the Pearson correlation coefficients (Table 1), it can be seen that the dairy commodity most closely correlated with the farm’s mailbox price is Class III milk, aligning with other studies (Altman, Sanders and Schneider, 2008). 

<div align="center">
  
||Class IV	|Class III|	Butter	|NFDM|
|:---:|:---:|:---:|:---:|:---:|
|Mailbox	|0.84387983	|0.962720017	|0.785990297	|0.172078104|
</div>

<div align="right">
Table 1: Pearson Correlation Coefficients
</div>
<br>
<br>
To execute a hedge using milk futures the farmers must first calculate the expected quantity of milk to be produced and the corresponding revenue. They must also estimate the period over which they want to hedge their price risk. Upon choosing the appropriate expiration month for the futures contract that aligns with the timing of their milk production and sales, the farmer must determine their hedge ratio. 

<br>
<br>
Hedge ratios play a crucial role in determining the optimal allocation of hedging instruments to effectively manage price risk in financial markets. According to Bell and Krasker (1986), hedge ratios represent the relationship between the quantity of the underlying asset being hedged and the number of hedging instruments employed. Bell and Krasker highlighted the significance of hedge ratios in enabling investors to determine the optimal quantity of futures needed to counteract potential losses resulting from adverse price movements in the underlying asset. This calculation ensures that the hedge achieves the desired level of protection while simultaneously minimising costs and optimising risk-adjusted returns. The determination of hedge ratios is influenced by various factors, including market volatility, the correlation between the underlying asset and the hedging instrument, and the time horizon of the hedge.

<br>
<br>
Upon calculating their hedge ratio, the farmers can enter the futures market by shorting the corresponding number of Class III Milk futures contracts on the exchange. It should be noted that throughout the hedge period, the farmers should monitor milk and futures prices, adjusting their hedge position should market conditions change significantly. 

<br>
<br>
Due the nature of the hedge, basis risks may arise. The basis is the difference between the cash price of milk and the futures price. Basis risk arises if the basis changes between the initiation and expiration of the hedge, impacting the effectiveness of the hedge (Working, 1953). In the context of the farmers, basis risk occurs because the farm’s mailbox price does not perfectly align with the price of Class III milk futures contracts used for hedging. This misalignment can be influenced by various factors such as local supply and demand dynamics, transportation costs, storage costs, and other market-specific conditions. Therefore, there is the risk the relationship between the cash market price and the futures market price may change unfavourably during the period of the hedge. Another risk when hedging is the potential for a margin call. Futures contracts require margin payments, and if the market moves against the hedge position, the farmer may need to deposit additional margin funds to maintain the hedge, potentially leading to liquidity challenges.
<br>
<br>


$${Y=\alpha+\betaΧ+\varepsilon}$$
<div align="right">
Fig. 1: Regression Model
</div>
<br>
<div align="center">

|||
|:---:|:---:|
|(Intercept)|-1.5571995** (0.7044506)|
|Mailbox Price|	1.1821876*** (0.0531889)|
|$`{N}`$|	41|
|$`{R^{2}}`$|	0.9268298|
\* p<.10, ** p<.05, *** p<.01
</div>
<div align="right">
Table 2: Regression Statistics 
</div>
<br>

Using a linear regression model (Fig. 1) provides the estimates in Table 2. Using the regression formula (Fig. 2), the futures price of Class III milk can be predicted to be $13.22, given a mailbox price of $12.50. 

$${\hat{Y}=-1.557+1.182(Mailbox Price)}$$

$${=-1.557+1.182(12.50)}$$

$${=13.22(2 d.p.)}$$

<div align="right">
Fig. 2: Regression Formula
</div>
<br>

Using the standard error of prediction (0.607) and the one-sided critical t value at a 95% level of confidence and 39 degrees of freedom (-1.685), the margin of error was calculated to be -1.023 (Fig. 3). Applying the margin of error to the predicted price of Class III milk futures gives the upper bound $14.24 (Fig 4). As strike prices in the milk market occur in intervals of $0.25, this figure is rounded, leading to a strike price of $14.25.


$$S.E_{{\hat{Y}}_{pred}}=s\sqrt{1+\frac{1}{n}+\frac{(x-\bar{x})^2}{{SS}_x}}$$

$$=s\sqrt{1+\frac{1}{40}+\frac{(12.50-13.127)^2}{126.763}}$$

$$=0.607$$
 
$$t_{\frac{0.05}{2},39}=-1.685$$

$$Margin\ of\ Error=t_{\frac{0.05}{2},39}*S.E_{\hat{Y}_{pred}}$$

$$=-1.023$$


<div align="right">
Fig. 3: Margin of Error Formula
</div>
<br>


$$Prediction\ Interval=\ \hat{Y}\pm Margin\ of\ Error$$


$$=(12.197,\ 14.243)$$


<div align="right">
Fig. 4: Prediction Interval Formula
</div>
<br>
  
By using the strike price $14.25, the farmers can be 95% sure that their put option will be in the money, should mailbox prices fall below $12.50. If their mailbox price falls below $12.50 at maturity, the farmers can choose to exercise their put options, meaning they can sell Class III milk futures contracts at the strike price of $14.25, even though the market price is lower. The difference between their strike price and the market price will be the farm’s payoff from the put option. Profiting from their put option will offset any loss they incur due to the reduced mailbox price, resulting in a hedging effect, thereby protecting the farm’s revenue and mitigating the effects of the price decrease. 
<br>
<br>

Reference List: 
<br>
<br>
Altman, I.J., Sanders, D. and Schneider, J. (2008). Producer-Level Hedging Effectiveness of Class III Milk Futures. Journal of American Society of Farm Managers and Rural Appraisers, 2008, pp.8–15. doi:https://doi.org/10.22004/ag.econ.189871. 
<br>
<br>
Anderson, R.W. and Danthine, J.-P. (1981). Cross Hedging. Journal of Political Economy, [online] 89(6), pp.1182–1196. Available at: https://www.jstor.org/stable/1837189. 
<br>
<br>
Bell, D.E. and Krasker, W.S. (1986). Estimating Hedge Ratios. Financial Management, 15(2), p.34. doi:https://doi.org/10.2307/3664976.
<br>
<br>
Bittman, J.B. (2013). Trading and Hedging with Agricultural Futures and Options. Columbia, Md: John Wiley & Sons, Inc. 
<br>
<br>
Hauser, R.J. and Eales, J.S. (1987). Option Hedging Strategies. North Central Journal of Agricultural Economics, 9(1), p.123. doi:https://doi.org/10.2307/1349348. 
<br>
<br>
Working, H. (1953). Futures Trading and Hedging. The American Economic Review, [online] 43(3), pp.314–343. Available at: http://www.jstor.org/stable/1811346. 
<br>
<br>
Yamey, B.S. (1971). Short Hedging and Long Hedging in Futures Markets: Symmetry and Asymmetry. The Journal of Law and Economics, 14(2), pp.413–434. doi:https://doi.org/10.1086/466716.

