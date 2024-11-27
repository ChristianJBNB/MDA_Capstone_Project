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
Last

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











