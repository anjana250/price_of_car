# Increase Used Car Dealership's Profit by Analyzing and Modeling Used Car Sales Data 

[Link to Jupyter Notebook](https://github.com/anjana250/price_of_car/blob/main/practical_application_II_starter/Price_of_Car_final.ipynb)
## Background:
A used car dealership is interested in increasing their sales by having someone take a look at a dataset containing 426,000 records of previously sold used cars. This dataset consists of many features that customers take into consideration when purchasing a new car, such as: color, type, year, model, manufacturer, milage, etc. The task is to do some initial analysis on the data, clean it up by removing any duplicates/outliers and then find the factors that a customer cares about the most. Finally, the car dealership needs to know what the results are so they are able to implement the findings into their inventory, sales and marketing plan.

Initially, by looking at just the numerical columns of the vehicles dataset, Year has a positive correlation with price- the newer the car, the more it can be sold for. The Title is also important in the sense that people would prefer to buy a vehicle iwth a clean title status. Odometer has a negative correlation meaning that people want a car that does not have as many miles on it. Interestingly, condition has a slightly negative correlation.

![corrolation](https://github.com/anjana250/price_of_car/assets/15185723/ba54d933-7920-4089-87e5-966e4cd24aae)

## Business Goals and KPI:
#### 1. Understand what characteristics customers value when purchasing a used car.
#### 2. How can the dealership use this information to optimize pricing and improve sales?

The metrics used to analyze the models are R<sup>2</sup> Score and Median Absolute Error (MAE). The goal is to optimize these as much as possible.

A thorough explanation of the Data Preparation,Data Understanding, and everythign else can be found by clicking on [Link to Jupyter Notebook](https://github.com/anjana250/price_of_car/blob/main/practical_application_II_starter/Price_of_Car_final.ipynb)

## Modeling:
The four models used on this data set is Linear Regression, Random Forest Regression, Ridge Regression, and Lasso. Out of the four models, Ridge performed the best when comparing the metrics R<sup>2</sup> score and Median Absolute Error(MAE). Therefore, only the results from this model will be addressed here. If there is any interest in looking at any of the other models, please refer to Jupyter notebook above.


**Evaluation Metric R<sup>2</sup> Score Comparison Between Models**
![R2metrics](https://github.com/anjana250/price_of_car/assets/15185723/32139aec-76bd-4922-a53c-1e42a3f3f006)

For the R<sup>2</sup> Score metric, Ridge has a score closest to 1 without being too close to 1 (sign of overfitting). Random Forest and Lasso had the worst outcomes for this metric.

**Evaluation Metric Median Absolute Error(MAE) Comparison Between Models**
![MAEmetrics](https://github.com/anjana250/price_of_car/assets/15185723/b58eb7fc-b548-4aa5-8932-abfbbc177a7c)

For the MAE metric, Ridge has the lowest error value. Linear and Random Forest are a little bit worse than Ridge while Lasso has the worst outcome.

## Findings from the Models:
After thorough model training and analysis of the most influential coefficients, several crucial factors have emerged:

#### 1. Model and Manufacturer of the Vehicle:
Certain models and manufacturers are highly sought after by used car buyers, such as "t", Willys Coupe, Nomad, 34 Tudor, and Chevelle Malibu Conver. Likewise, Ferrari, Morgan, Aston-Martin, Saturn, Tesla, and Porsche are among the most expensive manufacturers for used cars. While it may not be practical to exclusively stock these vehicles, it is advisable for the client to prioritize adding them to their inventory whenever possible.

#### 2. Year of Manufacture:
Newer vehicles tend to attract more buyer interest compared to older models that may come with higher maintenance requirements.

#### 3. Odometer Value at Purchase:
Buyers prefer vehicles with lower mileage, seeking cars that have been driven less.

#### 4. Impact of Sales State:
Certain states, such as Alaska, Hawaii, Idaho, Rhode Island, and Connecticut, have shown to have higher average prices. However, influencing this variable may be challenging for the dealership.

#### 5. Other Influential Factors:
Buyers also show a preference for diesel-fueled vehicles and convertibles. Additionally, the condition of the vehicle plays a role in influencing buyer decisions, albeit to a lesser extent.

## Recommendations:
1. Consider implementing inventory strategies that align with our key findings. Prioritize the acquisition of newer vehicles with lower mileage, as well as models and manufacturers that are in high demand. Diesel fuel vehicles or convertibles are also a good addition to the inventory. It is also a good idea to consider the condition of the vehicle obtained.
2. Ensure that vehicles with a history of commanding higher prices are priced appropriately to maximize profitability.
3. Maintain vigilance over market trends and customer preferences. Regularly reassess the relevance and applicability of our models' findings, making adjustments as needed to stay responsive to market dynamics.

## Next Steps:
It will be very helpful to continue to receive data about used car sales from the client so that we can further train the models to see which model performs better with more data. There is also a possiblity that findings might change and these changes need to be communicated with the client.

Different models can also be trained to see if there are any that perform better than Ridge Regression.

## Conclusion:
Based on the analysis of the car sales data, several key recommendations and next steps have been identified. Implementing inventory strategies that prioritize newer vehicles with lower mileage, as well as cars from the most sought-after models and manufacturers, can lead to increased sales and profitability. Additionally, ensuring that historically higher-selling cars are priced correctly is crucial.
Continuously monitoring market trends and customer preferences is essential to adapt strategies accordingly. It is also recommended to regularly reevaluate the model's findings and update them as necessary.
Moving forward, it would be beneficial to receive more data on used car sales to further train the models and potentially explore other models besides Ridge Regression to see if any perform better. Communication with the client regarding any changes in findings or strategies is key to maintaining a successful partnership and maximizing results.
