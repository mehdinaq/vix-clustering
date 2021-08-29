# vix-clustering
### [Application of K-Means Clustering to VIX data](https://github.com/mehdinaq/vix-clustering/blob/main/vix_clustering.ipynb)

### Overview
The VIX is known to be the fear gauge of the stock market, where high spikes in VIX coincide with high volatility and large percent drawdowns in the broader stock market (SPY benchmark).
The goal of this analysis is to use K-Means clustering to determine ranges of VIX values to be used as potential markers of market volatility.<br /><br />

### Data Source
Use the yfinance library to get VIX and SPY values from 1995 - 2021. Adjusted Close values for SPY are used to exclude the impact of dividends and other external actions unrelated to market performance

![spy vix history](https://user-images.githubusercontent.com/8281173/130368308-053ca3d1-9174-48e1-8b6c-517ea5dee11f.png)<br /><br />

### Analysis
- Use K-Means clustering for different number of clusters, and use Elbow method to subset final choices of clusters based on Sum of Squared Deviations
- Plot VIX data based on the final choices of cluster labels to visualize bands of VIX values
- Determine final choice of clusters by using box plots for the percent change in SPY based on cluster labels; the rationale behind the approach is to choose the number of clusters that provides clear separation in the SPY percent change and variations across clusters<br /><br />

[Detailed Analysis here](https://github.com/mehdinaq/vix-clustering/blob/main/vix_clustering.ipynb)<br /><br />

![vix clusters](https://user-images.githubusercontent.com/8281173/131237853-f133065b-1444-4468-9d9a-6440ecb73eab.png)<br /><br />

![spy pct change by clusters](https://user-images.githubusercontent.com/8281173/131237859-1c1e4998-9d1b-44c6-979c-5f19ed59cd23.png)



  
