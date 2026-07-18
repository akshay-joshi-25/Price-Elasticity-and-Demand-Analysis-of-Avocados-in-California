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

The dataset used for this report was publicly made available by the Hass Avocado Board (HAB), an industry-funded agriculture promotion group established in 2002 to increase the consumption and value of Hass avocados in the United States. You can access the dataset by clicking [here](https://www.kaggle.com/datasets/timmate/avocado-prices-2020?resource=download)

This report focuses on analyzing avocado pricing data for the year 2020.

# 🔧 **Tools Used**

- **Python** was used for data analysis and implementing the appropriate machine learning model.
- **Excel** was used for data wrangling.

# 🧮 Relationship between Average Price and Total Volume of Avocados sold by Market

In the charts below, the correlation coefficient (r) quantifies the strength and direction of the relationship between Average Price and Total Volume.

## Conventional Avocados

<img width="1072" height="638" alt="image" src="https://github.com/user-attachments/assets/bb868c4a-80cb-4479-b91e-2b723e58a920" />

### Las Vegas

* Shows a **weak negative relationship** between price and volume sold.
* Sales generally decrease as prices increase, but the trend is scattered with a few outliers.

**Business interpretation:** Demand is **relatively price-insensitive**, suggesting that factors other than price also influence sales.

### Los Angeles

* Displays a **moderate negative relationship**.
* Higher prices are generally associated with lower sales volumes.

**Business interpretation:** Consumers are **moderately price-sensitive**, so price increases are likely to reduce demand.

### Sacramento

* Shows a **strong negative relationship**.
* Sales volume decreases consistently as prices increase.

**Business interpretation:** This market is **highly price-sensitive**, making competitive pricing essential.

### San Diego

* Exhibits a **moderate negative relationship** with noticeable variation.
* Some scatter indicates that other factors also affect demand.

**Business interpretation:** Price influences demand, but promotions and market conditions likely play an important role.

### San Francisco

* Shows a **moderately strong negative relationship**.
* Higher prices generally correspond to lower sales volumes.

**Business interpretation:** Consumers are **fairly responsive to price changes**, so competitive pricing can help maintain sales.

### Overall Interpretation

All five graphs show a **negative relationship** between price and volume sold, indicating that demand generally decreases as prices increase. Price sensitivity is weakest in **Las Vegas**, strongest in **Sacramento**, and moderate in **Los Angeles, San Diego, and San Francisco**, suggesting that pricing strategies should be adjusted according to each market's responsiveness to price changes.

## Organic Avocados

<img width="1072" height="638" alt="image" src="https://github.com/user-attachments/assets/bf2e0730-d084-4ada-a14d-beeb69f3cafc" />

### Las Vegas

* Shows a **weak negative relationship** between price and volume sold.
* Sales tend to decrease slightly as prices increase, but the trend is scattered.

**Business interpretation:** Demand is **relatively price-insensitive**, suggesting that non-price factors also influence sales.

### Los Angeles

* Displays a **weak negative relationship** with considerable variation.
* The data points are widely dispersed, indicating an inconsistent trend.

**Business interpretation:** Price has a **limited impact** on demand, with other factors likely playing a larger role.

### Sacramento

* Shows a **strong negative relationship** between price and volume sold.
* Sales decline sharply as prices increase, with a few noticeable outliers.

**Business interpretation:** Consumers are **highly price-sensitive**, making competitive pricing important for maintaining demand.

### San Diego

* Exhibits a **weak negative relationship** with a broad spread of data points.
* The relationship between price and sales is not very pronounced.

**Business interpretation:** Demand is **only slightly affected by price**, indicating that other market factors influence purchasing decisions.

### San Francisco

* Shows a **moderate negative relationship**.
* Higher prices generally correspond to lower sales volumes, although a few outliers are present.

**Business interpretation:** Consumers are **moderately price-sensitive**, so pricing decisions are likely to influence sales.

### Overall Interpretation

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

# 🧠 Evaluating How Change in the Average Price will affect Demand.

## Conventional Avocados

<img width="786" height="246" alt="image" src="https://github.com/user-attachments/assets/325cb525-3f40-44d8-a785-05de575384f2" />

