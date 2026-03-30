# Database evaluation table

## Key:

#### Quick Check 
- Has 500+ rows (ideally 1000+)
- Has 5+ columns
- Data is downloadable as CSV / Excel

#### Hypothesis Check
The main statement: “Analysing [dataset] can help [organisation] improve [something valuable].”


You need to give three clear problems that are descision driven not descriptive
- Specific
- Solvable with data
- Link to business value


The three problems:
1. Prediction Problem
2. Factor Problem
3. Strategic/Policy Problem


#### Target Variable Check
Does your dataset have a column that reflects the result of predictions: Yes/No, Numeric data, grouping data etc 

#### Cleaning Potential
This project requires at least 10% cleaning to pass the assignment 

#### Variable Quality
Are all columns meaningful? Do they relate to each other logically and can I explain them all?

#### Dataset Method Match
For this project to work it's important to understand what type of data you're dealing with so the right analysis can be used. Be aware of the following methods covered in class:

- Classification → KNN / Naïve Bayes
- Prediction (numbers) → Regression
- Grouping → Clustering
- Patterns → Association rules

#### Business Value Test
Ask yourself who would use this? What decisions does it support? Can you link the methods to business value?
| Name | Link | Quick Check | Hypothesis Check | Target Variable Check | Cleaning Potential | Variable Quality | Dataset-Method Match | Business Value Test |
|----------|------|-------------|------------------|-----------------------|--------------------|------------------|----------------------|---------------------|
|Global Commodity Prices 2000-2026 | (https://www.kaggle.com/datasets/ibrahimqasimi/global-commodity-prices-2000-2026/data) |  ✅ 38,002 rows, ✅ 8 columns ✅ CSV file | MS: Analysing global commodity price data can help the UK government understand inflationary pressures and support more effective economic policy decisions. PP: How have global commodity prices changed over time, and which commodities show the most significant price fluctuations? FP: Which commodities contribute most to price volatility and are therefore likely to drive inflationary pressures? SP: Can commodities be grouped based on similar price behaviour to help prioritise areas for government monitoring or intervention? | ✅ The target Variable = Close column | ✅ Great Cleaning potential. There are missing values, 2,935 rows have Volume = 0 this is not accurate as trading days rarely have zero volume, There is inconsistent Numeric Precision, Negative / Impossible Values which is impossible for commodity prices, Redundant columns with ticker and commodity, The date column can be brushed up on, there are flat price rows which are low quality data, there are also outliers with volume| ✅ Yes all the columns are meaningful: Date (Trading date), Open (Price at market open), High (Highest price of the day), Low (Lowest price of the day), Close (Price at market close), Volume(Number of trades/contracts, Ticker (The market symbol), Commodity (The type of commodity it is), These columns link to each other logically becausde they describe the same thing at different times  | ✅ For this dataset the methods align with each question for PP: Regression and time series to analyse trends over time, for FP: Statistical analysis (within regression) to measure volatility numerically and SP: Clustering to look at group similar behaviour, the MS will then be using justiciation and linking to real-world use with the findings | ✅ The real UK organisations that would use this is the HM Treasury which is in charge of economic policy decision or Bank of England for inflation control, really just UK Government, the decisions that can be made using my analysis include: Inflation control, Energy policy, Budget Planning and risk monitoring, the methods I can use in relation to business value: Regression, this can predict future price trends → inflation forecasting, Volatility analysis, this can identify unstable commodities → risk management and lastly Clustering, Group similar commodities → policy prioritisation  |

