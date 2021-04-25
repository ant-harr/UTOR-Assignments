
# **Project: Five Year Historical Sector Performance Assessment and Regression Analysis of Stock Performance against Pandemic Impact**

# **Project Team:**

Pranav Satheesan

Jack Que

Samantha Karvanis

Anthony Harrison

Chimdike lhe

Mustafa Mufti

Carlos Corbi

# **Project Overview:**

The project presents the below results:

-   assessed the historical five year sector performance of three sectors -- Energy, Airline and Automobiles.

-   presents historical five year performance for user selected ticker which are active on Alpaca API.

-   provide map and graphs which shows the progression of the pandemic across the US and individual states across time.

-   perform regression analysis of the performance of the user selected ticker against the evolution of the pandemic.

# **Prerequisites to Run Project Code:**

The project code comprises of:

-   The Jupyter Notebook file -- Project1.ipynb

-   The csv file -- us_data.csv

-   Download the above two files from GitHub

The below conditions should be met to seamlessly run the project code:

-   PyViz virtual environment should be installed.

-   Alpaca should be installed **[within PyViz.]{.ul}**

-   SciPy should be installed **[within PyViz]{.ul}** (pip install SciPy).

-   env file with Alpaca keys and Mapbox key should be available in the folder where code is running from.

-   Pandemic cases are obtained based on upload of a csv file (us_data.csv). The Path function within the code should be updated to the location in your system where this csv file is saved.

![plot](./Images/1_Path.png)

# **The Final Product**

The project output is a dashboard with five tabs as noted below:

![plot](./Images/2_Dashboard.png)

The tabs in the dashboard include:

-   Assessment of Energy Sector Performance

-   Assessment of Airlines Sector Performance

-   Assessment of Automobiles Sector Performance

-   Performance Assessment of User Selected Stock

-   Map of Pandemic cases in the US across various dates

-   Regression analysis of performance of user selected stock compared to per day number of pandemic cases

# **Project Limitations**

The below limitations are noted in the project and the associated final product:

-   The key data source used for assessment are daily closing prices for active tickers from Alpaca. Alpaca does not modify historic data for stock splits. Therefore counterintuitive results are obtained for tickers which may have undergone stock splits in the previous five years (e.g Apple and Tesla).

-   In the final product, the graph for annual volatility comparison with SP500 shows previous user selected tickers as well. The refresh button on this graph should be selected to see the performance of the current user selected ticker. However, the previous user selected tickers are still retained in the graph.

-  This issue exists only in the Final Dashboard with tabs. On a standalone basis, outside the dashboard, the issue is not for the standalone Interact Function, indicating the issue is associated with how dash boards work (Four tabs in the dashboard are simultaneously calling the same function, which probably results in junk values being returned for this specific graph). The issue could not be resolved and can be seen in the final product.

# **Project Results**

## Assessment of Energy Sector Performance

The energy sector performance is assessed by using the five year historical data for the ETF Ticker RYE - Invesco S&P 500 Eql Wght Energy ETF. The summary performance chart is provided below:


![Settings Window](./Images/3_Energy.PNG)


As noted in the above results summary:

-   The energy sector in general had declining returns across the past five years even pre pandemic.

-   The sector volatility is significantly higher than SP500, indicating higher risk as compared to the market/

-   The combination of higher volatility and declining returns provide a negative feedback for this sector.

-   This is further evidenced in the sharpe ratio, which is negative 0.42, indicating poor performance.

## Assessment of Airlines Sector Performance

The airlines sector performance is assessed by using the five year historical data for the ETF Ticker JETS - US Global Jets ETF. The summary performance chart is provided below:

![Settings Window](./Images/4_Airlines.PNG)

As noted in the above results summary:

-   The airlines sector in general had a stable return profile pre pandemic. There were no major increases or decreases in the return profile indicating, dividends were probably the main source of returns.

-   The sector had a massive fall during the pandemic period and as noted in the above summary performance, the sector is still undergoing recover and has not completely emerged yet to the pre pandemic levels.

-   The sector has higher volatility than SP500, indicating risk higher than market.

-   The sharpe ratio for the sector is negative 0.3, indicating relatively poor performance as compared to the benchmark.

## Assessment of Automobile Sector Performance

The automobile sector performance is assessed by using the five year historical data for the ETF Ticker CARZ - First Trust NASDAQ Global Auto Index ETF. The summary performance chart is provided below:

![Settings Window](./Images/5_Automobiles.PNG)

As noted in the above results summary:

-   The automobile sector in general had declining returns during the pre pandemic period.

-   The sector has higher volatility than SP500, indicating risk higher than market.

-   However the sector has a sharpe ratio for the previous five years which is close to 0. This indicates overall performance in five years is comparable to sp500 for each unit of risk (volatility).

-   The sharpe ratio of zero is probably driven by the massive growth in returns post the pandemic period as noted in the above summary. This growth in returns is probably tied to the overall market hype on Electric Vehicles and associated firms in the industry.

## Sample Assessment of SP500 Sector performance compared to Pandemic Cases

The final tab of the project dashboard provides a regression analysis of the performance of the user selected ticker against new pandemic cases.

A sample assessment of the SP500 sector performance against new pandemic cases is provided below. The SP500 returns are obtained using the ticker IVV - iShares Core S&P 500 ETF:

![Settings Window](./Images/6_Regression1.PNG)

![Settings Window](./Images/7_Regression2.PNG)

As noted in the above results summary:

-   Despite an initial fall in SP500 returns at the start of the pandemic, the market has since recovered and is at record highs.

-   Even during the peak of the pandemic cases in the US, SP500 continued to rise to new highs.

-   As seen in the regression equation, the daily returns of the SP500 has a positive coefficient with the new pandemic cases. This indicates the market is not for the most part influenced by increased pandemic cases.

-   The return profile of the market raises doubt on how much linkage exists with the underlying economy and influence of external factors such as loose monetary policy influencing market returns.

  
