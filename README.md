# Machine Learning Analysis to Predict Used Automobile Prices

### Author: Christian Carson Jackson
Northwest Missouri State University, Maryville MO 64468, USA  
Email: [cjackson430@yahoo.com](mailto:cjackson430@yahoo.com)

## Description
This project aims to create a model that can accurately predict used car prices. It uses a [Used Car Sales Dataset](https://www.kaggle.com/datasets/satvshr/top-4-used-car-sales-datasets-combined) obtained from Kaggle, which contains many different attributes that can be used in machine learning algorithms to predict car prices. Finding an algorithm that can accurately predict used car prices would be helpful with potentially helping value cars in order to find if a car is overpriced or underpriced.

## Project Start
1. Start a new Repository and select a default README.md
2. Clone the Repository to your local environment.
3. Open the project, and create\activate the virtual environment.
```bash
python -m venv .venv
source .venv\Scripts\Activate
```
4. Install required libraries/dependencies into the virtual environment.
```bash
pip install -r requirements.txt
```

## Abstract
This project investigates the application of different machine learning algorithms to predict used car prices. The Car Price data set used was taken from Kaggle and provides a foundation for training various regression models, including Linear Regression, Random Forest, Decision Tree, and Support Vector. The Data set contains 19 thousand plus entities with features such as mileage, model, year, etc. After preprocessing and cleaning the data, key attributes were identified to be used in the predictive analysis. The primary objective of the project was to evaluate the performance of the different models when predicting the price of cars with a particular focus on metrics such as RMSE (Root Mean Squared Error) and R². The findings indicate that the Decision Tree model had the best overall performance in terms of fitting the data during training, though there were signs of overfitting with a lower R² score. The Random Forest Regressor also provided strong results but was less effective on unseen data compared to the Decision Tree model.
<br/>
Keywords: Machine Learning · Used Car Prices · Predictive Modeling· Regression Models · Encoding · Model Evaluation

## Introduciton
Automobiles are an essential aspect of everyday life. They make it possible to get from point A to point B on time. Automobiles are a luxury though because of the price it is not a luxury that everyone can enjoy. Many different aspects have led to the increase in the price of automobiles over the years. At the beginning of the decade, average car prices increased less than 3 percent annually until COVID-19 happened in which prices rose by 5 percent. The reason for this increase was the chip shortage that was experienced due to COVID-19. Modern cars are much more technologically advanced than previous generations of vehicles. This means that for all of that entertainment, safety, and performance tech you want in your automobile, you’re going to need quite a few car chips. This price increase has led to people not being able to buy cars at an affordable. The average car price did begin to dip slightly in 2022 after COVID-19 was coming to an end. With all of this in mind, trying to predict the price of cars can be accomplished by using machine learning.
<br/>
  In this project, using the Car Prices Dataset, machine learning algorithms were trained to predict the potential prices of used automobiles. The algorithms that are going to be featured will include linear regression, random forest regressor, decision tree regressor, and support vector regression (SVR) to find the most fitting model for the predictive analysis.

## Goals of Research
This project focuses on using different machine-learning models to find the most effective way to predict used car prices. By using data provided by the online dataset, the project hopes to create an effective and efficient way of predicting used car prices depending on many different factors.

- **Primary Goal**: Develop different machine-learning models to find the model that can predict most accurately automobile prices based on many different factors.
- **Secondary Goal**: Use visualizations to identify the most important factors that lead to the pricing of used cars.
- **Predicted Outcome**: Creation of an effective and efficient machine learning model that will predict car prices.

## Relevant Links
- [Car Price Prediction GitHub](https://github.com/ChristianJBNB/MDA_Capstone_Project)
- [Car Price Prediction Overleaf File](https://www.overleaf.com/read/ppjrmjkgwgcs#ce2a20)
- [Used Car Sales Dataset](https://www.kaggle.com/datasets/satvshr/top-4-used-car-sales-datasets-combined)

## Dataset 
The dataset used in this project will be the Car Prices Dataset. This dataset was obtained from Kaggle and it contains information about used car prices along with other attributes such as the make, model, and mileage of the cars. This dataset was last updated in 2021 and contains 19237 rows and 18 columns.

## Data Collection and Use
The data was collected from Kaggle. The data was contained in a CSV file which made it easy to implement into the project repository. Once the file was added to the repository, the CSV file was read into the main Python file using the Pandas extension. Pandas is a fast, powerful, flexible, and easy-to-use open-source data analysis and manipulation tool, built on top of the Python programming language. Putting the data into a data frame allowed for easy data analysis and cleaning. 

## Data Attributes
|Column Name|Description|Data Type|
|---|---|---|
|ID|Unique number to identify each data entry|Integer|
|Price|The amount of money in USD that was paid for the particular car|Integer|
|Levy|The tax cost that was associated with the sale|Object|
|Manufacturer|The company that made the car|Object|
|Model|The specific design of the car|Object|
|Prod. Year|The year that the car was made|Integer|
|Category|The style of car|Object|
|Leather Interior|Whether the car has a leather interior or not|Object|
|Fuel Type|What kind of fuel the car takes|Object|
|Engine Volume|The total volume of all the cylinders in a car's engine|Object|
|Mileage|The number of miles that were on the car at the time of sale|Object|
|Cylinders|The number of cylinders that are in the car|Float|
|Gear Box Type|The type of gearbox that is in the car|Object|
|Drive Wheels|What wheels are the drive wheels on the car|Object|
|Doors|The number of doors on the car|Object|
|Wheel|What side of the car the wheel is on|Object|
|Color|The color of the car|Object|
|Airbags|The number of airbags in the car|Integer|

## Main Attributes
While the dataset has a lot of attributes to choose from, not every aspect is that important when it comes to the price of the car. The main attributes that were used in the project were price, model, prod. year, fuel type, mileage, cylinders, and gearbox type. These are the most important attributes that determine the price of a car and lead to an accurate prediction of the price for other cars.

## Data Limitations
While the dataset has a lot of useful information, it is also missing information that would lead to more in-depth. The dataset only includes data from 2021 and no other historical data that could help with predicting price changes over time. It also doesn't have location data of where the cars were sold, which could help explain why certain cars may be more expensive than one another if they are the same make and model. These limitations could lead to less accurate predictions of the prices of used cars.

## Data Cleaning
For this project, the dataset selected had a lot of unnecessary information for predicting car prices. From the dataset, the columns that were removed were levy, leather interior, drive wheels, doors, color, and airbags. Most of these do not have a strong correlation to the price attribute and thus were not considered necessary in the analysis.

## Data Attributes after Cleaning
|Column Name|Description|Data Type|
|---|---|---|
|ID|Unique number to identify each data entry|Integer|
|Price|The amount of money in USD that was paid for the particular car|Integer|
|Manufacturer|The company that made the car|Object|
|Model|The specific design of the car|Object|
|Prod. Year|The year that the car was made|Integer|
|Category|The style of car|Object|
|Fuel Type|What kind of fuel the car takes|Object|
|Engine Volume|The total volume of all the cylinders in a car's engine|Object|
|Mileage|The number of miles that were on the car at the time of sale|Object|
|Cylinders|The number of cylinders that are in the car|Float|
|Gear Box Type|The type of gearbox that is in the car|Object|

## Cleaning Tools/Technique
The cleaning process was done using the Pandas library. First, the CSV file containing the dataset was put into a data frame using the Pandas library. Once the data frame had the dataset’s data, it was as simple as one line of Python code.

```bash
train_full.drop(['Leather interior', 'Drive wheels', 'Doors','Wheel', 'Color', 'Airbags', 'Levy'], axis=1, inplace=True)
```
This line of code uses the data frame ”train full” which holds all of the data from the dataset. The Pandas library has a method called ”.drop” which drops all of the columns that are listed inside the data frame. After this line of Python was executed the data was removed and it left only the data that was necessary to price prediction.

## Missing Data Handling
In the event of missing data from the dataset, the record would be removed but that did not end up being necessary because every record contained all the information that was needed. This resulted in there being 19238 rows with 11 columns in the cleaned dataset.

## Exploratory Data Analysis
Before starting the machine learning analysis, Exploratory Data Analysis (EDA) must be completed. The main purpose of EDA as defined by IBM, the main purpose of EDA is to help look at data before making any assumptions. It can help identify obvious errors, as well as better understand patterns within the data, detect outliers or anomalous events, and find interesting relations among the variables. For this project, the main focus of Exploratory Data Analysis was finding connections between the different chosen attributes and visualizing them. The Exploratory Data Analysis for this project began by first cleaning the
data and handling missing data. While doing this, data types were converted to more useful types that could be used for descriptive statistics. The key descriptive statistics that were computed were the count, mean, standard deviation, minimum, and maximum, along with the 25th, 50th, and 75th percentile from the Car Prices Dataset. After finding descriptive statistics, the next process was creating visualizations. The key visualizations that were used during the visualization process were histograms, pie charts, and scatter plots. These visualizations will be explained in depth as to what they are showing and why it is
relevant to the overall goal of predicting car prices. Relevant code and visualizations can be located in the Exploratory Data Analysis Notebook found in the Car Price Prediction GitHub repository. Below
are said visualizations and explanations.

## Descriptive Statistics 
||ID|Price|Prod. Year|Mileage|Cylinders|
|---|---|---|---|---|---|
|Count|19237.0|19237.0|19237.0|19237.0|19237.0|
|Mean|45576535.9|18555.9|2010.9|1532235.7|4.6|
|STD|936591.4|190581.3|5.7|48403869.4|1.2|
|Min|20746880|1|1939|0|1|
|25%|45698374|5331|2009|70139|4|
|50%|45772308|13172|2012|126000|4|
|75%|45802036|22075|2015|188888|4|
|Max|45816654|26307500|2020|2147483647|16|

## Visual Analysis
![image info](/visualizations/distributionofcars.png)
![image info](/visualizations/distributionofcarsfuel.png)
![image info](/visualizations/meancarprices.png)
![image info](/visualizations/priceandmileagegb.png)
![image info](/visualizations/pricecylinders.png)
![image info](/visualizations/manufacturer.png)
![image info](/visualizations/models.png)

## Conclusion of EDA
From looking at all the different visualizations it is clear that most of the attributes are important when predicting the price of a car. With this knowledge, the selected attributes will be the ones used in the machine learning analysis.

## Implementing Machine Leaning Analysis
The implementation of machine learning for this project will involve using different machine learning algorithms on the Car Price Dataset involving the previously stated features and new features created for better accuracy. The most accurate algorithm will be selected and used to predict car prices after the algorithm is given different attributes.

## Data Preprocessing
Before applying the different algorithms to the data, first, the data must be cleaned and focused to create stronger correlations between attributes. This was done in three different ways, label encoding, target encoding, and outlier removal. Label encoding is a technique that is used to convert categorical columns into numerical ones so that they can be fitted by machine learning models that only take numerical data. It is an important pre-processing step in a machine-learning project. \cite{LabelEncoding} The label encoder was applied to the object and float attributes in the cleaned data to make them usable in the different algorithms. Then the data was target encoded. Target encoding makes each category encoded based on a shrunk estimate of the average target values for observations belonging to the category. The encoding scheme mixes the global target mean with the target mean conditioned on the value of the category. \cite{TargetEncoding} Lastly the data removed outliers to remove the noise that they can cause when run through the algorithms. This lowered the entries from around 19000 to 5736. After this the Prod. Year column was altered from the year the car was created into the attribute, Vehicle Age, which was calculated by taking the current year and subtracting it by the Prod. Year. Once all of this was completed, feature selection was used to choose the attributes that had a strong correlation to get accurate predictive analysis by the different algorithms. The selected features were Model, Vehicle Age, Fuel type, Mileage, Category, and Price with the Price being the target value. 

## Model Training and Testing 
The main goal of model training in this project is to predict car prices using the selected features stated earlier. The algorithms that were used during this process were Linear Regression, Random Forest Regressor, Decision Tree Regressor, and Support Vector Regression. Each model was trained on selected features and the target value. The dataset was broken down into an 80/20 split of training and testing to make sure the model had sufficient data for learning. The metrics that are being used to determine the sufficient algorithm is the Root Mean Square Error (RMSE), which measures the average difference between the predicted and actual values of a model, and the R2 Score, which is a statistical metric used to evaluate how well a regression model fits the data, essentially indicating the proportion of variance in the dependent variable that can be explained by the independent variables. With these two metrics, selecting the correct algorithm will be simple.

## Model Comparison
||RMSE Train|RMSE Test|R2 Train|R2 Test|
|---|---|---|---|---|
|Linear Regression Model|92.05|92.55|0.18|0.22|
|Random Forest Regressor|51.56|82.05|0.92|0.52|
|Decision Tree Regressor|31.76|91.66|0.99|0.25|
|Support Vector Regression|95.81|97.04|0.44|0.36|

![image info](/visualizations/Comparionofmodels.png)

## Model Selection
Based on the numbers, it would appear that the best model to use for predicting car prices would be the Decision Tree Regressor. This is because the lower RMSE score indicates a better model performance and the high R2 score for training fits the data extremely well. The lower test R2 is concerning because it could indicate overfitting. Random Forest Regressor was a strong contender but the RMSE score indicates it doesn't perform well on unseen data.

## Conclusion
The objective of this project was to develop a predictive model that is able to estimate the price of a car by using different attributes such as mileage, age, and fuel type to name a few. Through exploratory data analysis and model training, the Decision Tree model became the most reliable model. The model is able to predict car prices based on already available data accurately but struggles when given unknown data. 

![image info](/visualizations/DecsionTree.png)

## Key Findings
The model suggests that attributes like mileage and vehicle age are the two most important aspects when determining the price of a car. From further testing, it became apparent that the model is not able to easily determine the price of cars when given factors that would make the price an outlier. The model looks at older cars and determines that because they are much older they should be extremely cheap. This is not always the case and this leads to inaccurate price prediction. The model does thrive when given the attributes of actual cars. When given actual car data from the dataset, the model can get almost the exact price of the car. The model can make meaningful trends but should be treated with caution when being used for practical applications.

![image info](/visualizations/BoxAndWhisker.png)

From looking a the box and whisker plot, it is apparent that the decision tree model was the correct model to use because of how accurate the predicted prices are compared to the actual. This also shows the outliers that are apparent in the data and why the model is not always the most accurate.

## Limitations
The data ended up being more limited than originally anticipated. This occurred when removing the outliers from the upper and lower quartiles leaving only around 6000 entities left before analysis. The data is also limited in the number of years of the car sales. All of the data was collected from 2021 which means there was less of a trend that could be seen over the years. The scope was also limited only focusing on finding the price of cars using only a few attributes to predict the price. If more attributes were used, then the model may have been more accurate.

## Future Work
This project is the initial work of developing a model that can accurately predict the prices of cars. Further work on the model would lead to more accurate predictions and continuous alteration of the data would create more correlations between the target value and attributes. Adding a location value could lead to seeing trends in prices in different states and countries. Lastly, trying different model algorithms could lead to finding a more applicable model.

In summary, the Decision Tree model provides useful data that can be used in predicting the prices of used cars. With further improvement, the model can become more accurate and provide better predictions. 

## References
1. Auctions, A.: Does mileage or age matter more to used car buyers?, https://www.
acvauctions.com/blog/used-car-age-vs-mileage
2. Chugh, A.: Ml — label encoding of datasets in python, https://www.geeksforgeeks.
org/ml-label-encoding-of-datasets-in-python/
3. IBM: What is exploratory data analysis? — ibm, https://www.ibm.com/topics/
exploratory-data-analysis
4. Mohanty, S.K.: Car prices dataset, https://www.kaggle.com/datasets/sidharth178/
car-prices-dataset
5. of North Charlotte, T.: The car chip shortage, explained, https://www.
toyotaofnorthcharlotte.com/research/the-car-chip-shortage-explained/
6. Pandas: Pandas, https://pandas.pydata.org/
7. Scikit: Targetencoder, https://scikit-learn.org/1.5/modules/generated/sklearn.
preprocessing.TargetEncoder.html
8. Susan Meyer, B.S.: Average car price is at an all-time high of 47,000 going into
2022, https://www.thezebra.com/resources/driving/average-car-price/



















