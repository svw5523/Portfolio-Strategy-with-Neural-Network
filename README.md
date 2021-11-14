# Explore the portfolio strategy with ML technique in Pharmaceuticals industry

### Introduction

Machine Learning has been a hot topic over the years and was mainly used in technology industry. However, nowadays people in financial industry also start to explore the application of Machine Learning in investment management area. Inspired by Prof. Aldridge’s book [“Big Data Science in Finance”](https://www.bdfbook.com/), our team hope to explore the usage of ML into portfolio construction, specifically to capture the noisy trading signal in daily basis. To better interpret the contribution of the ML technique into constructing the portfolio, we check the portfolio performance with out-of-sample portfolio profit PNL plot.

In this project, we define the target variable as the one-day ahead return and construct the trading signal by the sign of the predicted return value. If positive, then it shows "buy" signal as 1 and negative shows "sell" signal as -1 in daily basis.

### Background and Data Input
Under the pandemic, pharmaceuticals industry companies played a key role in developing the vaccine and providing medical care program to the society. Our team hopes to take a step into exploring their stock performance and related portfolio construction.

Our team selected the following 10 companies from [iShares U.S. Pharmaceuticals ETF (IHE) index](https://www.ishares.com/us/products/239519/ishares-us-pharmaceuticals-etf) and obtained their stock price information from Yahoo! Finance [linked here](https://finance.yahoo.com/). 

| Company | Ticker |
| ------------- | ------------- |
| JOHNSON & JOHNSON | JNJ |
| PFIZER INC | PFE |
| MERCK & CO INC | MRK |
| ZOETIS INC CLASS A | ZTS |
| ELI LILLY | LLY |
| CATALENT INC | CTLT |
| VIATRIS INC | VTRS |
| BRISTOL MYERS SQUIBB | BMY |
| JAZZ PHARMACEUTICALS | JAZZ |
| PERRIGO PLC | PRGO |

The portfolio optimization in-sample training period was performed from 01/01/2018 to 12/31/2019.

### Conclusion
The result is quite clear that the optimal portfolio selected by Neural Network model strictly outperforms that from the linear regression model or Random Forest Tree model. Backtested the optimized portfolio in out-of-sample period from 01/01/2020 to 10/29/2021 and the portfolio return out-of-sample is around 58.28% from the self-defined initial capital $1,000,000.

Our team hopes this project will give a simple idea and insight for the application of ML techniques in portfolio construction and as the baseline, our team may take a further step into introducing unsupervised learning technique, such as PCA approach in features selection and variance reduction.  

- Here, the Python code accounts for porfolio optimization with neural network model part.
