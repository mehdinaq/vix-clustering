# vix-clustering
### [Application of K-Means Clustering to VIX data](https://github.com/mehdinaq/vix-clustering/blob/main/vix_clustering.ipynb)

#### Overview
The VIX is known to be the fear gauge of the stock market, where high spikes in VIX coincide with high volatility and large percent drawdowns in the broader stock market (SPY benchmark).
The goal of this analysis is to use K-Means clustering to determine ranges of VIX values to be used as potential cut-off points for markers of market volatility.

#### Data Source
Use the yfinance library to get VIX and SPY values from 1995 - 2021. Adjusted Close values for SPY are used to exclude the impact of dividends and other external actions unrelated to market performance

![spy vix history](https://user-images.githubusercontent.com/8281173/130368308-053ca3d1-9174-48e1-8b6c-517ea5dee11f.png)

#### Analysis
- Use K-Means clustering for different number of clusters, and use Elbow method to subset final choices of clusters based on Sum of Sqaured Deviations
- Plot VIX data based on the final choices of cluster labels to visualize bands of VIX values
- Determine final choice of clusters by using box plots for the percent change in SPY based on cluster labels; the rationale behind the approach is to choose the number of clusters that provides clear separation in the SPY percent change and variations across clusters

[Detailed Analysis here](https://github.com/mehdinaq/vix-clustering/blob/main/vix_clustering.ipynb)

![Clustered VIX values](https://user-images.githubusercontent.com/8281173/130368840-e2795c7d-a318-4f64-a65c-928897812700.png)


  
