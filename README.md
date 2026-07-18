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
## Conventional Avocados

<img width="1072" height="638" alt="image" src="https://github.com/user-attachments/assets/bb868c4a-80cb-4479-b91e-2b723e58a920" />

### Graph 1 (Top Left)

* Shows a **weak negative relationship** between price and volume sold.
* Sales generally decrease as prices increase, but the trend is scattered with a few outliers.

**Business interpretation:** Demand is **relatively price-insensitive**, suggesting that factors other than price also influence sales.

### Graph 2 (Top Middle)

* Displays a **moderate negative relationship**.
* Higher prices are generally associated with lower sales volumes.

**Business interpretation:** Consumers are **moderately price-sensitive**, so price increases are likely to reduce demand.

### Graph 3 (Top Right)

* Shows a **strong negative relationship**.
* Sales volume decreases consistently as prices increase.

**Business interpretation:** This market is **highly price-sensitive**, making competitive pricing essential.

### Graph 4 (Bottom Left)

* Exhibits a **moderate negative relationship** with noticeable variation.
* Some scatter indicates that other factors also affect demand.

**Business interpretation:** Price influences demand, but promotions and market conditions likely play an important role.

### Graph 5 (Bottom Middle)

* Shows a **moderately strong negative relationship**.
* Higher prices generally correspond to lower sales volumes.

**Business interpretation:** Consumers are **fairly responsive to price changes**, so competitive pricing can help maintain sales.

### Overall Interpretation

All five graphs show a **negative relationship** between price and volume sold, indicating that demand generally decreases as prices increase. Price sensitivity is weakest in **Graph 1**, strongest in **Graph 3**, and moderate in **Graphs 2, 4, and 5**, suggesting that pricing strategies should be adjusted according to each market's responsiveness to price changes.
