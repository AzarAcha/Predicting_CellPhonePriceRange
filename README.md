# Predicting_CellPhonePriceRange

# Requirement

Task 1:-Prepare a complete data analysis report on the given data.

Task 2:-On the basis of the mobile Specification like Battery power, 3G enabled , wifi ,Bluetooth, Ram etc predict the Price range of the mobile.

Task 3:- Prepare the analysis report stating how model will help expanding the business by stating several factors including feature importance.


# Problem Statement

Bob has started his own mobile company. He wants to give a tough fight to big companies like Apple, Samsung etc.
He does not know how to estimate the price of mobiles his company creates. In this competitive mobile phone market, you cannot simply assume things. To solve this problem he collects sales data of mobile phones of various companies.
Bob wants to find out some relation between features of a mobile phone(eg:- RAM, Internal Memory etc) and its selling price. But he is not so good at Machine Learning. So he needs your help to solve this problem.
In this problem you do not have to predict the actual price but a price range indicating how high the price is


# Feature of the dataset

●	battery_power - Total energy a battery can store in one time measured in mAh\
●	blue - Has bluetooth or not\
●	clock_speed - speed at which microprocessor executes instructions\
●	dual_sim - Has dual sim support or not\
●	fc - Front Camera mega pixels\
●	four_g - Has 4G or not\
●	int_memory - Internal Memory in Gigabytes\
●	m_dep - Mobile Depth in cm\
●	mobile_wt - Weight of mobile phone\
●	n_cores - Number of cores of processor\
●	pc - Primary Camera mega pixels\
●	px_height - Pixel Resolution Height\
●	px_width - Pixel Resolution Width\
●	ram - Random Access Memory in Megabytes\
●	sc_h - Screen Height of mobile in cm\
●	sc_w - Screen Width of mobile in cm\
●	talk_time - longest time that a single battery charge will last when you are\
●	three_g - Has 3G or not\
●	touch_screen - Has touch screen or not\
●	wifi - Has wifi or not\
●	price_range - This is the target variable with value of 0(low cost), 1(medium cost), 2(high cost) and 3(very high cost).\



# Conclusion
Logistic Regression : This model shows strong performance with few misclassifications but cv score is much lesser 64% only. This is due to overfitting on the training data and failing on unseen data.
Gradient Boosting : This model also shows strong performance with high accuracy score, precision and f1 score and Cv is also above 90%. But itt misclassifies some medium and high category mobile models.
Random Forest Classifier : The training accuracy is 100% but test accuracy drops to 89% showing overfitting. Also, it misclassifies lot of medium and high class mobile models.
XGBoost Classifier : This model also shows overfitting but slightly less than Random Forest.
SVC : This model almost as same as XGBoost but with low recall score.
Decision Tree : It shows high overfitting, misclassification.
KNN : It is the least effective model for this project with low accuracy and other scores. Also, it misclassifies every segment.
ANN : Performs well and in par with Logistic Regression.


# Suggestion to the Bob
With the report of confusion matirx and test result, Bob has to implement Gradient Boosting Classifier to effectively price his mobile models.
He should also train the model with some additional data which may increase the accuracy level which in turn helps in to price his products.

