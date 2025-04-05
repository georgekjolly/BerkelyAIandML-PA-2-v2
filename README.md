**Required Assignment 11.1: What Drives the Price of a Car?**

Jupyter Note Book link : https://github.com/georgekjolly/BerkelyAIandML-PA-2/blob/main/prompt_II.ipynb

**Introduction**

This report presents the results from our analysis and modeling efforts aimed at predicting used car prices. By leveraging various machine learning models, we have provided insights into the key factors influencing car prices and developed predictive models that can be used by used car dealers to fine-tune their inventory decisions. The models and findings are aimed at optimizing pricing strategies and maximizing profitability in the used car market.

**Primary Findings**

From the data analysis, several factors were identified as significant drivers of the used car prices:

**Odometer (Mileage)**: Cars with lower mileage tend to have higher prices due to better condition and longevity.

**Vehicle Type:** The type of vehicle (e.g., sedan, SUV, truck) affects pricing due to differences in consumer demand and market trends.

**Model:** Specific vehicle models can have significantly different price trends based on brand reputation, reliability, performance, and consumer preference. Popular or well-rated models tend to retain value better.

**Manufacturer:** The brand of the car plays a key role in pricing, as some manufacturers are known for reliability, luxury, or performance. Well-established brands with strong resale value typically command higher prices.

**Year of Manufacture**: Newer vehicles are typically priced higher due to more advanced features, improved condition, and longer remaining lifespan.

**Drive Type**: Cars with all-wheel drive (AWD), four-wheel drive (4WD), or front-wheel drive (FWD) may be priced differently depending on their utility in specific environments.

**Fuel Type:** Cars powered by gasoline or diesel exhibit different price trends based on fuel efficiency, environmental factors, and demand for certain types of fuel.

**Transmission Type:** Manual and automatic transmissions can influence price, with automatic generally commanding a premium in many markets.
Region: The geographical location of the car plays a significant role in pricing, as demand can vary by area.

**Model Overview**

Two key models were employed to predict used car prices:

**Ridge Regression:** This model performed well in predicting the price, utilizing polynomial transformations of the features to capture non-linear relationships in the data. The optimal Ridge model had a polynomial degree of 5 and an alpha of 1000.

**Linear Regression:** A simpler approach was also employed, using linear regression with the same polynomial degree and yielding similar results to Ridge regression. This suggests that a linear model is sufficiently capturing the relationship between the features and price, but regularization in Ridge helped avoid overfitting.

Both models performed reasonably well, with the Ridge regression providing a slightly more robust solution due to its regularization, which prevented overfitting in higher-degree polynomials.

**Performance Evaluation**

**Best Model:** The Ridge Regression model with a polynomial degree of 5 and an alpha of 1000 provided the most accurate predictions for both the training and test datasets.

**Key Performance Metrics:**

R² (Train): 0.7131

R² (Test): 0.6575

Train MSE: 66,797,167

Test MSE: 83,609,049

These metrics indicate a good balance between model complexity and performance, with a decent fit on both training and testing data.

**Feature Importance**

Through the use of polynomial features, we identified the following features as being significant in predicting car prices:

Odometer (Mileage),
Vehicle Type,
Year of Manufacture,
Manufacturer,
Model,
Drive Type,
Fuel Type,
Transmission Type,
Region

These features are crucial in understanding the price variations in used cars and can guide pricing strategies for dealers. A more detailed feature analysis, including feature selection and interaction terms, could further optimize model performance.

**Recommendations for Dealers**

Based on the findings, we recommend the following actions for used car dealers:

**Pricing Strategy:** Prioritize vehicles with lower mileage, newer models, and popular types (e.g., SUVs) to command higher prices.
Market Segmentation: Adjust prices based on regional demand. Cars with certain features like 4WD or AWD may perform better in specific regions.
Inventory Optimization: Invest in vehicles that are expected to retain higher resale value, such as those with specific fuel types or transmissions in demand.
Opportunities for Further Improvement

While the models provide strong insights, further refinements could enhance predictive accuracy:

**Feature Engineering:** Additional transformations or interaction terms might capture more complex relationships between features.
Data Enrichment: Incorporating external data, such as current market trends or competitor pricing, could provide more contextual information for pricing.
Advanced Modeling: Exploring more complex algorithms, like Random Forests or Gradient Boosting, could offer additional improvements, especially in capturing non-linear patterns.
Conclusion

This analysis provides a robust foundation for understanding the key factors that influence used car prices and offers actionable insights that can help used car dealers fine-tune their inventory and pricing strategies. By leveraging the models and insights presented, dealers can make data-driven decisions to optimize their offerings and maximize their profit margins.

Moving forward, continuous monitoring and fine-tuning of the model, as well as the exploration of new features, will further enhance the accuracy and relevance of predictions for future market conditions.
