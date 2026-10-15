# 📈 Time Series Analysis in Python

Companion repository for the **4-part YouTube video series** on time series analysis:
from the theory of stochastic processes to forecasting with ARIMA models, with the Box-Jenkins workflow applied to a real dataset.

> 🎥 **YouTube playlist:** www.youtube.com/@EpsilonDeltaItalia

## 🗂️ Episodes

| # | Episode | Topics | Notebook | Colab |
|---|---------|--------|----------|-------|
| 1 | Fundamentals and Decomposition | Stochastic processes, time series vs cross-section, trend / seasonality / residual, moving averages, multiplicative `seasonal_decompose` | [`01_fundamentals_decomposition.ipynb`](notebooks/01_fundamentals_decomposition.ipynb) | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/USERNAME/time-series-analysis-python/blob/main/notebooks/01_fundamentals_decomposition.ipynb) |
| 2 | Stationarity, ACF and PACF | Strict vs weak stationarity, ergodicity, White Noise vs Random Walk, correlograms | [`02_stationarity_acf_pacf.ipynb`](notebooks/02_stationarity_acf_pacf.ipynb) | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/USERNAME/time-series-analysis-python/blob/main/notebooks/02_stationarity_acf_pacf.ipynb) |
| 3 | Differencing and Tests | Lag and difference operators, ADF unit-root test, log + seasonal differencing, Turning Point Test | [`03_differencing_adf_turning_point.ipynb`](notebooks/03_differencing_adf_turning_point.ipynb) | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/USERNAME/time-series-analysis-python/blob/main/notebooks/03_differencing_adf_turning_point.ipynb) |
| 4 | ARIMA Models and Forecasting | ARMA/ARIMA, Box-Jenkins workflow, residual diagnostics, `auto_arima`, forecasts with confidence intervals | [`04_arima_box_jenkins.ipynb`](notebooks/04_arima_box_jenkins.ipynb) | [![Open in Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/USERNAME/time-series-analysis-python/blob/main/notebooks/04_arima_box_jenkins.ipynb) |

> Replace `USERNAME` in the Colab links with your GitHub username.

## 🚀 Getting Started

```bash
git clone https://github.com/USERNAME/time-series-analysis-python.git
cd time-series-analysis-python

python -m venv .venv
source .venv/bin/activate        # Windows: .venv\Scripts\activate
pip install -r requirements.txt

jupyter notebook notebooks/
```

Or open the notebooks directly in Google Colab using the badges above.

## 🧰 Stack

`numpy` · `pandas` · `matplotlib` · `seaborn` · `scipy` · `statsmodels` · `scikit-learn` · `pmdarima`

## 📚 Datasets

All notebooks use data that is either downloaded automatically or simulated:

- **AirPassengers** (monthly airline passengers 1949–1960), loaded with `statsmodels.datasets.get_rdataset` (episodes 1 and 4; requires an internet connection).
- **Simulated series** (White Noise, Random Walk, synthetic series with trend and seasonality) with a fixed seed for reproducibility (episodes 2 and 3).

## 🧭 Suggested Path

```
Decomposition → Stationarity & ACF/PACF → Differencing & tests → ARIMA & forecasting
    (Ep. 1)            (Ep. 2)                  (Ep. 3)               (Ep. 4)
```

## 📄 License

Released under the [MIT License](LICENSE).
