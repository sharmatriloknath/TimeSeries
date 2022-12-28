# TimeSeries Forcasting
**Timeseries:** A time series is nothing but a sequence of various data points that occurred in a successive order for a given period of time.

#### How to Analyze the Timeseries Data
    <div alert alert-danger>
    - Collecting the data and cleaning it
    - Preparing Visualization with respect to time vs key feature
    - Observing the stationarity of the series
    - Developing charts to understand its nature.
    - Model building – AR, MA, ARMA and ARIMA
    - Extracting insights from prediction 
    </div>

### Components of Timeseries
1. **Trend:** In which there is no fixed interval and any divergence within the given dataset is a continuous timeline. The trend would be Negative or Positive or Null Trend.

2. **Seasonality:** In which regular or fixed interval shifts within the dataset in a continuous timeline. Would be bell curve or saw tooth.

3. **Cyclical:** In which there is no fixed interval, uncertainty in movement and its pattern.

4. **Irregularity** Unexpected situations/events/scenarios and spikes in a short time span.


![Image]("https://editor.analyticsvidhya.com/uploads/39815Components%20of%20Time%20Series%20Analysis.png")

### Data Types of Time Series
- There are two data types:
    - Stationary
    - Non-Stationary

1. **Stationary:** A dataset should follow the below thumb rules, without having Trend, Seasonality, Cyclical, and Irregularity component of time series.
- The MEAN value of them should be completely constant in the data during the analysis
- The VARIANCE should be constant with respect to the time-frame
- The COVARIANCE measures the relationship between two variables.

2. **Non-Stationary:** It is just opposite to Stationary.

![image]("https://editor.analyticsvidhya.com/uploads/99388Stationary%20Vs%20Non-Stationary.png")


### How to check Stationarity
During the TSA model preparation workflow, we must access if the given dataset is Stationary or NOT. Using Statistical and Plots test.

**Statistical Test:** There are two tests available to test if the dataset is Stationary or NOT.
- Augmented Dickey-Fuller (ADF) Test
- Kwiatkowski-Phillips-Schmidt-Shin (KPSS) Test
**Augmented Dickey-Fuller (ADF) Test or Unit Root Test:** The ADF test is the most popular statistical test and with the following assumptions.
**Null Hypothesis (H0):** Series is non-stationary
**Alternate Hypothesis (HA):** Series is stationary
p-value >0.05 Fail to reject (H0)
p-value <= 0.05 Accept (H1)

**Kwiatkowski–Phillips–Schmidt–Shin (KPSS):** these tests are used for testing a NULL Hypothesis (HO), that will perceive the time-series, as stationary around a deterministic trend against the alternative of a unit root. Since TSA looking for Stationary Data for its further analysis, we have to make sure that the dataset should be stationary.


### Convert Non-Stationary to Stationary
- Detrending
- Differencing
- Transformation


