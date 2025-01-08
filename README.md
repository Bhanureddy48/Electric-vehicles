# Electric-vehicles

A summary of the project:
An essential component of the shift to environmentally friendly transportation is electric automobiles. But "range anxiety"—the worry that the battery will die before getting to a charging station—remains a major obstacle to their widespread use. In order to address this problem, our project uses machine learning to develop prediction models that, utilizing historical data and different vehicle attributes, produce precise battery range estimates.

Important objectives include:

1.creating a trustworthy model for predicting battery range.
2.determining the main elements influencing EV battery performance.
3.evaluating the effectiveness of several regression techniques, including XGBoost, KNN, and Decision Tree.
4.giving manufacturers and EV users useful information.


The dataset:
The "Cheapest Electric Cars 2023" dataset, which is openly accessible on Kaggle, was used for this project (Dataset Link).

Features:
Vehicle price
Battery capacity (kWh)
Driving range (miles)
Charging time (hours)
Energy efficiency (miles per kWh)
Vehicle make and model

The dataset contains exploratory data analysis (EDA) for improved comprehension and has been preprocessed to guarantee data integrity. The static dataset is supplemented with additional simulated scenarios for dynamic driving circumstances.


Models and Techniques:

Three regression models are investigated in this study to predict battery range:
1.Regressor for Decision Trees
Advantages: Easy to understand, captures non-linear interactions, and is straightforward.
Cons: More likely to overfit.
2.KNN Regressor (K-Nearest Neighbors)
Advantages include instance-based learning and effectiveness with smaller datasets.
Cons: Sensitive to feature scaling; computationally costly for huge datasets.
3.XGBoost Regressor
Advantages: Reduces overfitting by regularization, manages intricate relationships, and is incredibly precise.
Cons: Requires a lot of computation.

Matrices for evaluation:

To evaluate the models, the following metrics were used:
Mean Absolute Error (MAE)
Mean Squared Error (MSE)
Root Mean Squared Error (RMSE)
R-Squared (R²)

XGBoost outperformed other models, achieving:
MAE: 53.29
MSE: 12201.0
RMSE: 110.45
R²: 0.4194

Findings:
-The most accurate model was the XGBoost Regressor, which explained input-feature variability and captured intricate interconnections.

Important revelations include:
1.A longer driving range is correlated with a larger battery capacity.
2.EVs with all-wheel drive and rear-wheel drive typically use more energy.
3.In general, cheaper EVs sacrifice driving range in exchange for reduced costs.

Future Extent:
Future enhancements can consist of:
1.Incorporating current environmental information, such as road conditions and weather.
2.employing sophisticated deep learning models for sequential data analysis, such as RNNs or transformers.
3.maximizing computational effectiveness for EV systems' real-time applications.
