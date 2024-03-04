# Projects Portfolio
This Portfolio contains multiple machine learning projects that I have worked on to explore data and create models for predictions
**Each project includes:**
  * A detailed explanation of the project requirements
  * Detailed Exploratory Data Analysis for exposing hidden insights
  * Multiple Machine learning models, selecting the best performing model for deployment.

The Project Portfolio includes Classification, Advanced Regression Techniques, Deep Learning, and Recommendation Systems algorithms.

## :thumbsup: Projects

**Energy Prices Prediction in the United Kingdom**:

Due to inflation, the energy price has increased in the United Kingdom. The government wants to determine the families and individuals who cannot meet this price increase. There are many factors (features) here to determine or predict the inability to meet up with energy prices. These features are categorized into four (4):
  - Temperature: The weather of a day could have a significant effect on the energy consumption by consumers. In winter, the temperature is cold, and to keep warm, energy is consumed through the heating system. During summer, the temperature rises and as such, the use of the heating system is at its minimum or not in use at all. But due to high temperatures, there is a need to drop the temperature by air-conditioning. Both situations may lead to an increase in energy consumption.
 - Appliances: Another category that influences energy consumption is appliances. The features to consider here may include the type of appliances such as Televisions, washing machines, dryers, microwaves, and electric kettles. Another feature here is the number of each appliance and the frequency of their uses. Other features may include age and the appliances’ energy rating, which can significantly affect electricity consumption. The lower the age of an appliance, the less consumption of energy. Due to technological advancements, newer appliances tend to consume less energy. The lower number of electrical appliances and decreases in usage may reduce energy consumption and vice versa, influencing the increase or decrease of electricity cost.
- Consumer habit: This feature can either increase or decrease users' electricity consumption. Little changes made to these features which may include ensuring electrical appliances are switched off when not used, turning off light bulbs and heaters, reducing the temperature of the water heater, and switching off all devices before sleeping or when not in the home can help reduce consumer’s electricity consumption and as a result decrease in electricity cost. The vice versa can lead to an increase in electricity cost.
- Demography: There are quite a few features to consider here. The characteristics of the consumer which may include age, gender, income, education, home ownership, sexual orientation, marital status, family size, health, and disability status can influence energy consumption and the ability to pay increasing electricity costs. If the family size is large, there is a tendency for an increase in electricity consumption and an overall increase in electricity cost. With a high level of education and good income, the obligation to pay the increasing electricity cost may not be difficult for the consume
About 26 features are categorized into the 4 groups above, which are explored and analyzed.

The project is divided into two:

**Classification Problem**: With these features, we are to determine if a consumer is having difficulties with increasing energy prices or not. The target variable and prediction is the True (1) value if the customer is having difficulties with the increasing energy prices and False (0) if vice versa.

The following processes were considered:

- **Data ingestion/Loading of Data**
- **Data Cleaning and preprocessing**
- **Feature Engineering**
- **Model Development and Prediction**
  
  - The data was split into train and test set
  - The whole data was used for cross-validation with CV = 5. This means that the model will split the data into 5, using 4 folds of the data as training data to train the model and 1 fold as test data to test the model. This will be done five times with different folds as test data. At any point, the test data are different. They help to validate the model and see if the model is generalized and not overfitting or underfitting when unknown (unseen data) is used to test the model.
  - Nine (9) models were developed which include LGBM, XGB, GradientBoost, Random Forest, Quadratic Discriminant, Linear Discriminant, Logistic Regression, and GaussianNB. 
  - The model performance was determined with the following metrics:
    - Accuracy
    - Precision
    - Recall
    - Confusion Matrix
    - Classification Report

  The table below displays the performance of each trained model on test data.
  
  ![image](https://github.com/dabson2020/Projects-Portfolio/assets/45830157/d1792e76-7645-4b35-a0a9-7a5dade84075)
  
  Here is a visual representation of the model performance
  
  ![image](https://github.com/dabson2020/Projects-Portfolio/assets/45830157/d657646c-9e04-4ac9-b390-b2f8cb11304d)


  With the accuracy of 89%, 89% on cross-validation score on test data, and 90.1% accuracy on unknown data, the model with the best performance is the **XGB Classifier**


**Regression Problem**:

The energy company desires to predict the variation in the annual expenditure that a customer is going to have due to the increase in the energy cost. If the customer is going to spend more in the coming year, the price is positive, but if the customer is spending less, then the value will be
negative. With the provision of historical data, a prediction of the expenditure is carried out using machine learning techniques. This predicted value on the historical data is compared with the actual value and the technique/model with the lowest mean squared error (the metric utilized to determine the performance of the model) is utilized for the prediction of the expenditure over unknown or future data. The machine learning Regressors are utilized to create the model. We use Regression techniques because the predicted target values are numeric.

The following processes were considered:

- **Data ingestion/Loading of Data**
- **Data Cleaning and preprocessing**
- **Feature Engineering**
- **Model Development and Prediction**
  - Six Regression models were developed which include: Linear regression, LassoLarsCV, Ridge, Decision Tree, Random Forest, and Gradient gradient-boosting regressors
  The computed metrics for model performance are the R2 score and Mean Squared Error (MSE). 

  The table for the models' performance is shown below.
  
  ![image](https://github.com/dabson2020/Projects-Portfolio/assets/45830157/ef97836b-5950-4308-8cdd-52ce0e189a75)


  Gradient Boost outperformed other regressors with an R2 score of 0.80 with a visual representation shown below:
  ![image](https://github.com/dabson2020/Projects-Portfolio/assets/45830157/8477e28c-d142-402a-84f0-32ac62969917)



