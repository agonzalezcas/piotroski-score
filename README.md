# Piotroski F-Score for Stock Selection

## Summary
This notebook calculates the Piotroski F-Score of all companies in the CSI 300 (沪深300) Index. The score is a number between 0 and 9. Assessing the financial strength of the companies for identifying value stocks.

## Data
This analysis was first created and written on [JoinQuant](https://www.joinquant.com/) research platform.  Data were gathered using [JQData API](https://www.joinquant.com/data).

## Calculation
Add 1 to the score if any of the below statements is true

*Profitability (公司盈利项)* - **Is the company making money?**

- Return of Asset is positive (资产收益率是否为正?)
- Operating Cash Flow is positive (经营现金流是否为正?)
- Change in ROA is positive (去年的资产回报率是否增长了?)
- OCF/TA is larger than ROA (产生的现金流量比利润好吗?)

*Leverage and Source of Funds (债务项)* - **How much of the funds are from debt?**

- Change in Leverage Ratio (Long-Term Debt) is negative (过去一年杠杆率下降了吗?)
- Change in Current Ratio is positive (过去一年资产负债的流动比率是否有所提高(即手上持有的现金是否更多)?)
- No increase in number of existing shares (公司有发行股票吗?)

*Operating Efficiency* - **Is the company generating profits from its assets efficiently?**

- Change in Gross Margin is positive (过去一年的毛利率增长了吗?)
- Change in Asset Turnover is positive (去年的资产周转率是否增长了?)

## References
1. https://www.zhitongcaijing.com/content/detail/316953.html (华文)
2. https://codingandfun.com/piotroski-f-score/
3. https://en.wikipedia.org/wiki/Piotroski_F-score
