# 📊 Price Elasticity and Demand Analysis of Avocados in California

This report served two objectives:
- Assess the price elasticity of conventional and organic avocados across seven markets: California, Las Vegas, Los Angeles, Sacramento, San Diego, San Francisco, and one additional market.
- Evaluate how changes in price affect the demand for conventional and organic avocados in each of these seven markets.

# 📌 **Overview**

This report covers the following:
- Plot and interpret the relationship between the prices of conventional and organic avocados and their corresponding sales volumes in each market.
- Fit an appropriate machine learning model to capture the relationship between price and sales volume.
- Interpret the fitted model to determine the price elasticity of demand and evaluate how changes in price affect the demand for conventional and organic avocados.

# 📂 **Datasets**

The dataset used for this report was publicly made available by the Hass Avocado Board (HAB), an industry-funded agriculture promotion group established in 2002 to increase the consumption and value of Hass avocados in the United States. It functions under the supervision of the United States Department of Agriculture (USDA).

This report focuses on analyzing avocado pricing data for the year 2020. You can access the dataset by clicking [here](https://www.kaggle.com/datasets/timmate/avocado-prices-2020?resource=download)

# 🔧 **Tools Used**

- **Python** was used for data analysis and implementing the appropriate machine learning model.
- **Excel** was used for data wrangling.

# 🧮 Relationship between Average Price and Total Volume of Avocados sold by Market

In the charts below, the correlation coefficient (r) quantifies the strength and direction of the relationship between Average Price and Total Volume.

## Conventional Avocados

<img width="1072" height="638" alt="image" src="https://github.com/user-attachments/assets/bb868c4a-80cb-4479-b91e-2b723e58a920" />

All five graphs show a **negative relationship** between price and volume sold, indicating that demand generally decreases as prices increase. Price sensitivity is weakest in **Las Vegas**, strongest in **Sacramento**, and moderate in **Los Angeles, San Diego, and San Francisco**, suggesting that pricing strategies should be adjusted according to each market's responsiveness to price changes.

## Organic Avocados

<img width="1072" height="638" alt="image" src="https://github.com/user-attachments/assets/bf2e0730-d084-4ada-a14d-beeb69f3cafc" />

All five graphs show a **negative relationship** between price and volume sold, indicating that demand generally decreases as prices increase. The relationship is **strongest in Sacramento**, **moderate in San Francisco**, and **weak in Las Vegas, Los Angeles, and San Diego**, suggesting that price sensitivity varies across the different markets.

# 📈 Fitting an appropriate ML model to capture the relationship between Average Price and Total Volume

## Conventional Avocados

<img width="1180" height="638" alt="image" src="https://github.com/user-attachments/assets/c78371e4-2d79-40ae-831f-aa3e33dca9cc" />

### Las Vegas

* Shows a **weak negative relationship** between price and volume sold.
* The GAM curve declines gradually, indicating only a slight reduction in demand as prices increase.

**Business interpretation:** This market exhibits **price inelasticity**, as demand changes relatively little in response to price increases.

### Los Angeles

* Displays a **moderate negative relationship** with a steeper decline at higher prices.
* The GAM curve suggests demand falls more rapidly as prices rise.

**Business interpretation:** This market exhibits **moderate price elasticity**, with consumers becoming more responsive to higher prices.

### Sacramento

* Shows a **strong nonlinear negative relationship**.
* The GAM curve remains fairly flat at lower prices before dropping sharply at higher prices.

**Business interpretation:** This market exhibits **price elasticity**, particularly at higher price levels, where demand decreases substantially with price increases.

### San Diego

* Exhibits a **moderately strong negative relationship**.
* The GAM curve shows a consistent decline in sales as prices increase.

**Business interpretation:** This market is **price elastic**, indicating that consumers respond noticeably to price changes.

### San Francisco

* Shows the **strongest negative relationship** among the five graphs.
* The GAM curve declines sharply, especially at higher prices.

**Business interpretation:** This market is **highly price elastic**, with demand decreasing significantly as prices rise.

### Overall Interpretation

All five graphs indicate a negative relationship between price and volume sold. However, the degree of price responsiveness differs across markets:

* **Price Inelastic:** **Las Vegas**, where demand changes only slightly with price.
* **Moderately Price Elastic:** **Los Angeles**, where demand becomes more responsive as prices increase.
* **Price Elastic:** **Sacramento, San Diego, and San Francisco**, with **San Francisco** showing the highest price elasticity, indicating that consumers are highly sensitive to price increases.

## Organic Avocados

<img width="1180" height="638" alt="image" src="https://github.com/user-attachments/assets/1817bb8f-675a-4c1c-bacd-e96119a175a9" />

### Las Vegas

* Shows a **nonlinear relationship** between price and volume sold.
* Sales decline as prices increase initially, then stabilise and recover slightly at higher prices.

**Business interpretation:** This market exhibits **mixed price responsiveness**. Demand is **price elastic at lower prices** but becomes **more inelastic at higher prices**, suggesting that consumers remaining at higher prices are less sensitive to further price increases.

### Los Angeles

* Displays a **weak negative relationship**.
* The GAM curve is nearly flat, indicating only a slight decline in sales as prices increase.

**Business interpretation:** This market exhibits **price inelasticity**, with demand changing very little in response to price changes.

### Sacramento

* Shows a **highly nonlinear relationship** with large fluctuations.
* The wide confidence interval at higher prices indicates substantial uncertainty due to limited observations.

**Business interpretation:** Price elasticity is **difficult to determine reliably**. While demand appears highly responsive at certain price ranges, the high uncertainty means no strong conclusion can be drawn.

### San Diego

* Exhibits a **weak nonlinear negative relationship**.
* Sales generally decline as prices increase, with a slight flattening in the middle of the price range.

**Business interpretation:** This market is **mostly price inelastic**, with only modest changes in demand following price increases.

### San Francisco

* Shows a **highly nonlinear relationship** with considerable uncertainty at higher prices.
* The GAM curve fluctuates substantially, and the confidence interval widens considerably.

**Business interpretation:** The relationship between price and demand is **uncertain**. Although demand appears responsive at some price levels, there is insufficient evidence to confidently classify the market as price elastic or inelastic.

### Overall Interpretation

The markets exhibit varying degrees of price responsiveness:

* **Price Inelastic:** **Los Angeles and San Diego**, where demand changes only slightly as prices increase.
* **Mixed Elasticity:** **Las Vegas**, where demand is more elastic at lower prices but becomes less responsive at higher prices.
* **Uncertain:** **Sacramento and San Francisco**, where highly nonlinear trends and wide confidence intervals suggest insufficient evidence to reliably determine price elasticity.

# 🧠 Evaluating How Change in the Average Price will affect Demand and Revenue.

## Conventional Avocados

Notes:
- Las Vegas observed price range is [0.73, 1.14] - total volume for prices [1.2, 1.3] were not extrapolated as a result.
- Sacramento observed price range is [0.97, 1.54] - total volume for prices [0.8, 0.9] were not extrapolated as a result.
- San Francisco observed price range is [0.99, 1.67] - total volume for prices [0.8, 0.9] were not extrapolated as a result.

<img width="757" height="245" alt="image" src="https://github.com/user-attachments/assets/81e0c205-732d-4449-829c-ea1c0bc0c347" />

Since some values are missing, the percentage changes can only be calculated where consecutive data points are available.

* **If the average price increases from $0.80 to $0.90**, the total volume would
  * **increase by 14.41%** in **Las Vegas**, but
  * **decrease by 15.92%** in **Los Angeles** and **7.78%** in **San Diego**.

* **If the average price increases from $0.90 to $1.00**, the total volume would
  * **increase by 0.13%** in **Las Vegas**, but
  * **decrease by 12.30%** in **Los Angeles** and **7.86%** in **San Diego**.

* **If the average price increases from $1.00 to $1.10**, the total volume would
  * **decrease by 28.13%** in **Las Vegas**, **4.37%** in **Los Angeles**, **24.69%** in **Sacramento**, **7.52%** in **San Diego**, and **8.30%** in **San Francisco**.

* **If the average price increases from $1.10 to $1.20**, the total volume would
  * **decrease by 1.18%** in **Los Angeles**, **6.81%** in **San Diego** and **8.32%** in **San Francisco**, but
  * **increase by 3.94%** in **Sacramento**

* **If the average price increases from $1.20 to $1.30**, the total volume would
  * **decrease by 5.90%** in **Los Angeles**, **13.03%** in **Sacramento**, **6.73%** in **San Diego**, and **6.31%** in **San Francisco**.

<img width="671" height="246" alt="image" src="https://github.com/user-attachments/assets/233167e3-a8f0-4061-b03d-b9c5b88f3917" />

Based on the calculations form the above table, I would recommend conventional avocados to be sold at the followin prices to generate maximum revenue:
* **$1** in **Las Vegas**, and **Sacramento**
* **$1.3** in **Los Angeles**, **San Diego**, and **San Francisco**

## Organic Avocados

Notes:
- Las Vegas observed price range is [1.30, 1.65] - total volume for prices [1.7, 1.8] were not extrapolated as a result.
- Los Angeles observed price range is [1.44, 2.10] - total volume for prices [1.3, 1.4] were not extrapolated as a result.
- San Diego observed price range is [1.33, 2.34] - total volume for prices [1.3] were not extrapolated as a result.
- San Francisco observed price range is [1.36, 2.26] - total volume for prices [1.3] were not extrapolated as a result.

<img width="671" height="246" alt="image" src="https://github.com/user-attachments/assets/63317b2c-08b8-415c-b31a-119ce744abd5" />

Since some values are missing, the percentage changes can only be calculated where consecutive data points are available.

* **If the average price increases from $1.30 to $1.40**, the total volume would
  * **increase by 12.63%** in **Las Vegas**, but
  * **decrease by 14.96%** in **Sacramento**.

* **If the average price increases from $1.40 to $1.50**, the total volume would
  * **decrease by 8.44%** in **Las Vegas**, **0.83%** in **San Diego** and **19.51%** in **San Francisco**, but
  * **increase by 4.89%** in **Sacramento**

* **If the average price increases from $1.50 to $1.60**, the total volume would
  * **decrease by 30.19%** in **Las Vegas**, **1.82%** in **Los Angeles**, **7.78%** in **Sacramento**, **0.87%** in **San Diego**, and **20.20%** in **San Francisco**.

* **If the average price increases from $1.60 to $1.70**, the total volume would
  * **decrease by 1.91%** in **Los Angeles**, **18.66%** in **Sacramento**, **0.93%** in **San Diego**, and **17.32%** in **San Francisco**.

* **If the average price increases from $1.70 to $1.80**, the total volume would
  * **decrease by 2.05%** in **Los Angeles**, **1.02%** in **San Diego** and **9.97%** in **San Francisco** but
  * **increase by 2.90%** in **Sacramento**

You can access the Python code used to conduct the price elasticity & demand analysis by clicking [here.](https://github.com/akshay-joshi-25/Price-Elasticity-and-Demand-Analysis-of-Avocados-in-California/blob/main/Price%20Elasticity%20and%20Demand%20Analysis.ipynb)
