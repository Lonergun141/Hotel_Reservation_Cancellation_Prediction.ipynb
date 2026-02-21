# Hotel Reservation Cancellation Prediction

## Background
With the rise of online hotel reservation platforms, the way customers book hotels has evolved significantly. These platforms offer greater flexibility, enabling customers to make or cancel reservations with ease. However, this convenience comes with challenges for hotels, particularly when reservations are canceled or guests do not show up as planned. This behavior has implications on hotel revenue management and operational planning.

## Importance
A considerable number of hotel reservations are either canceled or result in no-shows, which can impact hotel profitability. Guests often cancel for various reasons such as changes in plans or scheduling conflicts, and they are frequently encouraged by flexible cancellation policies. While this is beneficial for customers, it introduces uncertainties for hotel operators who may lose revenue or face difficulty in managing resources efficiently.

## Objective
The objective of analyzing this dataset is to predict whether a customer will honor their hotel reservation or cancel it. Accurately predicting cancellations can help hotels implement better strategies for minimizing revenue loss and improving resource allocation by anticipating customer behavior more effectively.

## Technologies & Libraries Used
- **Python**
- **Pandas** (Data manipulation and analysis)
- **Matplotlib & Seaborn** (Data visualization)
- **Scikit-learn** (Machine learning modeling & evaluation)

## Methodology
1. **Data Loading:** The dataset is loaded from a CSV file.
2. **Data Preprocessing:** Categorical features (`type_of_meal_plan`, `room_type_reserved`, `market_segment_type`, `booking_status`) are numerically encoded automatically using `LabelEncoder`.
3. **Exploratory Data Analysis (EDA):** Analyzing the distribution between canceled (0) and not canceled (1) bookings.
4. **Model Development:** The dataset is split into an 80% training set and a 20% testing set. Three classification models are deployed:
   - Support Vector Machine (SVM)
   - K-Nearest Neighbors (KNN)
   - Logistic Regression
5. **Model Evaluation:** Models are evaluated and compared using specific performance metrics, including Accuracy, Precision, Recall, Sensitivity, Specificity, and F1 Score, along with visual Confusion Matrices.

## Conclusion
Based on the analysis performed, **Logistic Regression** emerged as the most effective model for predicting hotel reservation cancellations in this context. It demonstrated the highest accuracy, precision, recall, and F1-score compared to SVM and KNN.

The findings suggest that Logistic Regression is a highly suitable model for predicting hotel reservation cancellations based on the given features. Hotels can leverage this model to implement proactive strategies to minimize revenue loss and optimize resource operations.