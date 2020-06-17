# Finviz Analytics
What is Finviz?¶
FinViz aims to make market information accessible and provides a lot of data in visual snapshots, allowing traders and investors to quickly find the stock, future or forex pair they are looking for. The site provides advanced screeners, market maps, analysis, comparative tools and charts.

# Why?
Leverage the unofficial python API for FinViz to create custom stock screeners to identify value with volatile market conditions.

# How? 
Download current international stock stats.  Load & perform lightweight staging via finviz-analytics notebook.
https://github.com/sahudsonleck/finviz-analytics/blob/master/finviz.ipynb.  
Associated analytics is located in Tableau public gallery 
https://public.tableau.com/profile/stephanie.hudson4873#!/vizhome/USValueStocks/finviz
Review the associated data model and pandas-profile reports for data domain details. 

# Data Sets 
* Overview
* Technical 
* Financial
* Custom
* Performance
* Ownership
* Valuation
* Overview 

# Data Set Detail
#  stock_screener_financial.csv
## Columns
No.
Ticker
Market Cap
Dividend
ROA
ROE
ROI
Curr R
Quick R
LTDebt/Eq
Debt/Eq
Gross M
Oper M
Profit M
Earnings
Price
Change
Volume
## Summary Stats
       Ticker Market Cap Dividend   ROA   ROE   ROI Curr R Quick R LTDebt/Eq  \
count    7522       7522     7522  7522  7522  7522   7522    7522      7522   
unique   7522       4165     1098   998  1560  1129    224     222       557   
top       NJR          -        -     -     -     -      -       -         -   
freq        1       2254     3314  3366  3404  3352   3913    3973      3300   

       Debt/Eq Gross M Oper M Profit M Earnings Change Volume  
count     7522    7522   7522     7522     7522   7522   7522  
unique     596     974   1113      967      216   1407   7135  
top          -       -      -        -        -  0.00%      0  
freq      3300    4136   4011     4010     3653    218    100  


#  stock_screener_overview.csv
## Columns
No.
Ticker
Company
Sector
Industry
Country
Market Cap
P/E
Price
Change
Volume
## Summary Stats
       Ticker   Company     Sector              Industry Country Market Cap  \
count    7522      7522       7522                  7522    7522       7522   
unique   7522      7487         11                   149      49       4165   
top       NJR  CHS Inc.  Financial  Exchange Traded Fund     USA          -   
freq        1         5       3500                  2226    6568       2254   

         P/E Change Volume  
count   7522   7522   7522  
unique  2186   1407   7135  
top        -  0.00%      0  
freq    4598    218    100  


#  stock_screener_technical.csv
## Columns
No.
Ticker
Beta
ATR
SMA20
SMA50
SMA200
52W High
52W Low
RSI
Price
Change
from Open
Gap
Volume
## Summary Stats
       Ticker  Beta  SMA20  SMA50 SMA200 52W High 52W Low   RSI Change  \
count    7522  7522   7522   7522   7522     7522    7522  7522   7522   
unique   7522   416   2454   3519   4671     4582    5907  2754   1407   
top       NJR     -  2.08%  0.77%  1.78%  -10.00%  48.94%     -  0.00%   
freq        1  3664     20     11      8        8       6    53    218   

       from Open    Gap Volume  
count       7522   7522   7522  
unique      1310    879   7135  
top        0.00%  0.00%      0  
freq         524    550    100  


#  stock_screener_custom.csv
## Columns
No.
Ticker
Company
Sector
Industry
Country
Market Cap
P/E
Price
Change
Volume
## Summary Stats
       Ticker   Company     Sector              Industry Country Market Cap  \
count    7522      7522       7522                  7522    7522       7522   
unique   7522      7487         11                   149      49       4165   
top       NJR  CHS Inc.  Financial  Exchange Traded Fund     USA          -   
freq        1         5       3500                  2226    6568       2254   

         P/E Change Volume  
count   7522   7522   7522  
unique  2186   1407   7135  
top        -  0.00%      0  
freq    4598    218    100  


#  stock_screener_performance.csv
## Columns
No.
Ticker
Perf Week
Perf Month
Perf Quart
Perf Half
Perf Year
Perf YTD
Volatility W
Volatility M
Recom
Avg Volume
Rel Volume
Price
Change
Volume
## Summary Stats
       Ticker Perf Week Perf Month Perf Quart Perf Half Perf Year Perf YTD  \
count    7522      7522       7522       7522      7522      7522     7522   
unique   7522      2423       4141       5366      4960      5202     5034   
top       NJR     0.00%          -          -         -         -    0.00%   
freq        1        51         32         79       188       452       10   

       Volatility W Volatility M Recom Avg Volume Change Volume  
count          7522         7522  7522       7522   7522   7522  
unique         1717         1517    34       5823   1407   7135  
top           6.35%            -     -      1.10M  0.00%      0  
freq             16           32  3551         20    218    100  


#  stock_screener_ownership.csv
## Columns
No.
Ticker
Market Cap
Outstanding
Float
Insider Own
Insider Trans
Inst Own
Inst Trans
Float Short
Short Ratio
Avg Volume
Price
Change
Volume
## Summary Stats
       Ticker Market Cap Outstanding Float Insider Own Insider Trans Inst Own  \
count    7522       7522        7522  7522        7522          7522     7522   
unique   7522       4165        4354  3946        1086          2055     1649   
top       NJR          -           -     -           -             -        -   
freq        1       2254        2254  2781        2728          3081     2625   

       Inst Trans Float Short Short Ratio Avg Volume Change Volume  
count        7522        7522        7522       7522   7522   7522  
unique       2152        1450        1077       5823   1407   7135  
top             -           -           -      1.10M  0.00%      0  
freq         3074        2802        1909         20    218    100  


#  stock_screener_valuation.csv
## Columns
No.
Ticker
Market Cap
P/E
Fwd P/E
PEG
P/S
P/B
P/C
P/FCF
EPS this Y
EPS next Y
EPS past 5Y
EPS next 5Y
Sales past 5Y
Price
Change
Volume
## Summary Stats
       Ticker Market Cap   P/E Fwd P/E   PEG   P/S   P/B   P/C P/FCF  \
count    7522       7522  7522    7522  7522  7522  7522  7522  7522   
unique   7522       4165  2186    2036   827  1547  1178  2245  1906   
top       NJR          -     -       -     -     -     -     -     -   
freq        1       2254  4598    4640  5735  2772  2740  3276  5197   

       EPS this Y EPS next Y EPS past 5Y EPS next 5Y Sales past 5Y Change  \
count        7522       7522        7522        7522          7522   7522   
unique       2428       3071        1262        1172           832   1407   
top             -          -           -           -             -  0.00%   
freq         2927       3611        3531        4473          3806    218   

       Volume  
count    7522  
unique   7135  
top         0  
freq      100  


#  stock_screener_overview.csv
## Columns
No.
Ticker
Company
Sector
Industry
Country
Market Cap
P/E
Price
Change
Volume
## Summary Stats
       Ticker   Company     Sector              Industry Country Market Cap  \
count    7522      7522       7522                  7522    7522       7522   
unique   7522      7487         11                   149      49       4165   
top       NJR  CHS Inc.  Financial  Exchange Traded Fund     USA          -   
freq        1         5       3500                  2226    6568       2254   

         P/E Change Volume  
count   7522   7522   7522  
unique  2186   1407   7135  
top        -  0.00%      0  
freq    4598    218    100  






