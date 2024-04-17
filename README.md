# Help Used Car Dealership Increase Profit by Analyzing and Modeling Used Car Sales Data 

## Background
A used car dealership is interested in increasing their sales by having someone take a look at a dataset containing 426,000 records of previously sold used cars. This dataset consists of many features that customers take into consideration when purchasing a new car, such as: color, type, year, model, manufacturer, milage, etc. The task is to do some initial analysis on the data, clean it up by removing any duplicates/outliers and then find the factors that a customer cares about the most. Finally, the car dealership needs to know what the results are so they are able to implement the findings into their inventory, sales and marketing plan.

Initially, by looking at just the numerical columns of the vehicles dataset, Year has a positive correlation with price- the newer the car, the more it can be sold for. The Title is also important in the sense that people would prefer to buy a vehicle iwth a clean title status. Odometer has a negative correlation meaning that people want a car that does not have as many miles on it. Interestingly, condition has a slightly negative correlation.

![corrolation](https://github.com/anjana250/price_of_car/assets/15185723/ba54d933-7920-4089-87e5-966e4cd24aae)

## Business Goals and KPI
1. Understand what characteristics customers value when purchasing a used car.
2. How can the dealership use this information to optimize pricing and improve sales?

The metrics used to analyze the models are R2 Score and Median Absolute Error (MAE). The goal is to optomize these as much as possible.

A thorough explanation of the Data Preparation,Data Understanding, and everythign else can be found by clicking on [Link to Jupyter Notebook](https://github.com/anjana250/price_of_car/blob/main/practical_application_II_starter/Price_of_Car_final.ipynb)

## Modeling
The four models used on this data set is Linear Regression, Random Forest Regression, Ridge Regression, and Lasso. Out of the four models, Ridge performed the best when comparing the metrics R2 score and Median Absolute Error(MAE). Therefore, only the results from this model will be addressed here. If there is any interest in looking at any of the other models, please refer to Jupyter notebook above.


![R2metrics](https://github.com/anjana250/price_of_car/assets/15185723/99389a78-48c3-4314-b4f8-65751f3cf8b1)

For the R2 Score metric, Ridge has a score closest to 1 without being too close to 1 (sign of overfitting).
![MAEmetrics](https://github.com/anjana250/price_of_car/assets/15185723/927b31eb-849a-448d-abe7-d8dcf476e820)

For the MAE metric, Ridge has the lowest error value.

Ridge Regression Model suggests that the factors that customers care the most about when buying a used car are:
1. Model of the vehicle 
3. Year the Vehicle was Manufactured
4. Manufacturer of the Vehicle
5. State in which the sale happened
6. Odometer value at the time of purchase

The models of cars most coveted by used car buyers are:
1. "t"                       
2. willys coupe                
3. nomad                       
4. 34 Tudor                   
5. chevelle malibu conver

The manufacturers of cars that are priced the highest are:
1. ferrari   
2. morgan          
3. aston-martin    
4. saturn
5. tesla  
6. porsche  

Used car buyers also want to buy cars that are newer, and do not have as much milage on them. The state in which the sale is made also has an impact, with Alaska, Hawaii, Idaho, Rhode Island and Connecticut having the highest prices.


