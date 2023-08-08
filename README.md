# sales-predictions

Goal: Predicting and improving sales of grocery and supermarket products with different variables. Methods: Data Visualizations and Machine Learning (Decision Trees and Linear Regression)

Throughout the duration of this project, I undertook the task of data cleansing, delved into data analysis employing visualization techniques, and devised machine learning methodologies to both assess and construct predictive models for the dataset.

The culmination of the project materializes in a comprehensive slideshow presentation. This presentation effectively encapsulates the broader implications of my research, presenting a comprehensive overview of the insights derived and offering actionable recommendations for leveraging this data to bolster sales within the market. The entire content of this presentation has been thoughtfully included within this README document.

# Data Visualizations: 

![heatmap](https://github.com/carmeniturbe/sales-predictions/assets/98364829/c7250cda-1841-4742-83f8-2ca3dbe313b6)

A heatmap exploration of our dataset has highlighted a significant correlation. Notably, there exists a moderate relationship between Item_MRP (maximum retail price) and Item_Outlet_Sales (total sales for an item at an outlet). This insight underscores the potential impact of pricing strategies on sales performance.

## Grocery Stores vs. Supermarkets:

![Grocery stores vs supermarket](https://github.com/carmeniturbe/sales-predictions/assets/98364829/776e2559-c4cb-4166-8422-ee91090df084)

The dataset is characterized by a notably higher presence of supermarkets compared to grocery stores. This disparity has the potential to introduce bias to our data if left unaddressed.

## Grocery Store Sales:

![Grocery Store Sales](https://github.com/carmeniturbe/sales-predictions/assets/98364829/acb534a9-1584-4c45-8b94-f18827e48c7d)

The sales distribution leans towards the right, indicating a higher frequency of lower sales yields for a majority of items.

## Supermarket Sales:

![Supermarket Sales](https://github.com/carmeniturbe/sales-predictions/assets/98364829/0269d89d-8f89-4902-b959-2671be8986bf)

Exhibiting a greater magnitude than that of grocery stores, the data from higher-scale establishments also demonstrates a right-skewed sales distribution. This skewness signifies a prevalence of items sold at lower sales yields within this segment as well.

## Types of Items:

![Type of items](https://github.com/carmeniturbe/sales-predictions/assets/98364829/48cc82e3-9dd1-43f7-8288-3060b90f57a0)

Across diverse item categories, a balanced proportionality is observed between lower and higher outlet sales. Interestingly, the seafood category deviates from this trend, exhibiting a notably similar proportionality between the lower and higher sales brackets. This suggests that the seafood category maintains a consistent level of performance across varying sales ranges, distinguishing it as a robust performer in terms of sales.

# Machine Learning

I performed Linear Regression and Simple Trees models to see which may be best for predicting our Item_Outlet_sales.

## Linear Regression:

- R2 Score:
  
  Train: 0.5271927340568043

  Test: 0.5188218954890396
  
- RMSE:
  
  Train: 1175.5378103908606

  Test: 1176.813204725337

## Simple Decision Tree:

- R2 Score:
  
  Train: 0.6160308756204118

  Test: 0.5916472077034576
  
- RMSE:
  
  Train: 1059.3578354805206

  Test: 1084.107550470981

## Random Forest:

- R2 Score:
  
  Train: 0.6250694432556143

  Test: 0.6003007932873522
  
- RMSE:
  
  Train: 1046.8150307344442

  Test: 1072.5591384139607

## Model Evaluation and Findings:

Upon evaluating the performance of the Linear Regression model, I observed an R² score of 0.5271 for the training data and 0.5188 for the test data. Additionally, the RMSE values were calculated to be 1175.5378 for training and 1176.813 for testing. These metrics suggest that the Linear Regression model captures a certain degree of variance, albeit with moderate predictive accuracy. The test RMSE indicates the average error between the predicted and actual values.

The performance of the Decision Tree Regressor model was very similar, The R² score for the training data was 0.6160, while the test data exhibited an R² score of 0.5916. The corresponding RMSE values for training and testing were 1059.35 and 1084.10, respectively.

In contrast, the Random Forest Model yielded more promising results. The R² score for the training data was 0.6250, while the test data exhibited an R² score of 0.6003. The corresponding RMSE values for training and testing were 1046.81 and 1072.55, respectively. The Random Forest model demonstrates better predictive ability and a closer fit to the actual values in comparison to the Linear Regression and Decision Tree regressor models.

While the Random Forest model emerges as the more suitable choice based on the presented findings, it is important to note that even though it performs better, it still falls short of achieving the optimal scores. This limitation is attributed to the inherent nature of the dataset, characterized by a relatively lower degree of correlation between variables. The predictive performance of the models is influenced by this underlying aspect.

In conclusion, while Random Forest model offers improved predictive performance over the Linear Regression and  Decision Tree Regressor models, it's essential to acknowledge that all models face challenges due to the limited correlation present in the data. Despite this, the Random Forest model stands as a more viable choice for our  task, capturing underlying patterns and demonstrating a greater ability to generalize to unseen data.

# Recommendations

My findings lead me to the following conclusions and recommendations:
- Prioritize Supermarkets over Grocery Stores: Shift your attention towards supermarkets rather than grocery stores.
- Enhance Item Visibility:  Ensure optimal visibility for your items.
- Competitive Pricing and Occasional Sales:  Consider implementing competitive pricing strategies or periodic sales promotions.
- Profitable Seafood Market: The seafood segment demonstrates potential for profitability.

These insights offer strategic directions to enhance sales and optimize your market approach.
