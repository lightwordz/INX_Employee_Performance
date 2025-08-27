# INX Future Inc.

## Requirements

INX Future Inc, is one of the leading data analytics and automation solutions provider with over 15 years of global business presence.  INX is consistently rated as top 20 best employers past 5 years. In recent years, the employee performance indexes are not healthy and this has become a growing concern among the top management. The CEO Mr. Brain, decided to initiate a data science project, which analyzes the current employee data and find the core underlying causes of the employee performance issues. He also expects a clear indicators of non-performing employees, so that any penalization of non-performing employee, if required, may not significantly affect other employee morals.

The following insights are expected from this project:

* Department wise performances.
* Top 3 Important Factors effecting employee performance.
* A trained model which can predict the employee performance based on factors as inputs.
* Recommendations to improve the employee performance based on insights from analysis.

### Final Project File

You can view the main project file here: [INX Employee Performance Ratings](Employee_Performance_Analysis/processed/INX_EmployeePerformanceRatings.ipynb)

---

## Analysis

* The data is supervised and categorical. The predictor variables are ordinal and a few among them are nominal. The target variable 'PerformanceRating' is ordinal.

* To analyze the data, various data processing techniques like **Label Encoding** and **Standardization** is used. **Correlation Coeffecient** is used to interpret the relationship between variables. The most important features selected are **Department, Job Role, Environment Satisfaction, Last Salary Hike Percent, Work Life Balance, Experience Years At This Company, Experience Years In Current Role, Years Since Last Promotion, Years With Current Manager**.

* For training the data and predicting the target, algorithms used are **Logistic Regression, Support Vector Machine, Decision Tree, Random Forest Classifier, K-Nearest Neighbor, Gradient Boosting Classifier** and **ANN (Multi-layer Perceptron Classifier)**. A separate analysis of Department wise Performance is carried out.

---

## Summary

The project was done with the purpose of finding out factors affecting the performance of the employees, training a model which accurately predicts the performance rating of the employee, analyzing the data to provide recommendations to improve the performance and gain insights from the analysis. The following steps were carried out:

* Import the data provided, find out the predictor & target variables and look for missing values.
* Analysis of Department wise performance as asked.
* Label Encoding the ordinal columns.
* Calculate correlation coeffecient to find out the relationship between variables and then select the important features for analysis.
* Standardizing the data and splitting it into test and train.
* Training the data using algorithms like Logistic Regression, Support Vector Machine, Decision Tree, Random Forest, K-Nearest Neighbor, Gradient Boosting Classifier and Artificial Neural Network and checking the accuracy to find out which algorithm is the best.
* Exporting the model with highest accuracy.

---

## Results

* Random Forest with GridSearchCV gives **96.82%% accuracy**. The features that positively correlated are Environment Satisfaction, Last Salary Hike Percent & Worklife Balance. This means that if these factors increases, Performance Rating will increase. On the other hand, the features that are negatively correlated are **Years Since Last Promotion, Experience Years at this Company, Experience years in Current Role & Years with Current Manager. This means that if these factors increases, Performance Rating will go down.

* The top 3 features effecting employee performances are:

1. Employee Environment Satisfaction (**39.5%**)
2. Employee Last Salary Hike Percent (**33.3%**)
3. Work Life Balance (**12%**)

---

## Analysis and Insights

* It was observed that the maximum accuracy was obtained when we used **Random Forest with GridSearchCV** which was **96.82%**.

* The important features that are positively correlated are **Environment Satisfaction, Last Salary Hike Percent & Worklife Balance**. This means that if these factors increases, Performance Rating will increase. On the other hand, the features that are negatively correlated are **Years Since Last Promotion, Experience Years at this Company, Experience years in current role & Years with Current Manager**. This means that if these factors increases, Performance Rating will go down.

* We can conclude that the company should provide a better environment as it increases the performance drastically. The company should increase the salary of the employee from time to time and help them maintain a worklife balance. On the other hand, shuffling the manager from time to time will also affect performance.

---

## Recommendation

we can conclude from our analysis the following which can help with improvement in the employee performance ratings:

- Tailored Training: Create personalized training based on experience and background.
- Competitive Pay: Ensure salaries are competitive, especially for top talent.
- Faster Promotions: Facilitate quicker promotions for high-achievers (within 4 years).
- Flexible Work: Offer flexible arrangements to improve work-life balance.
- Address Performance Gaps: Target and fix performance issues in Sales and R&D.
- Promote Well-being: Cultivate a culture of strong work-life balance.

