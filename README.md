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
