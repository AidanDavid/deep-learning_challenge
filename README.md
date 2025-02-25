# deep-learning_challenge
See model1.ipynb for the original, innacurate model. See model2.ipynb for the far more accurate model.

# Analysis

The purpose of this project was to develop a deep learning model. This model would predict the success of funding applications for the Alphabet Soup charity; thus, allowing for more strategic allocation of resources.

## Results

#### Data Preprocessing

Target Variable: STATUS column, indicating the success of the funding application.

Feature Variables: All other columns, excluding EIN and NAME, were used as features.

Removed Variables: The EIN and NAME, they do not provide predictive value for the model.

#### Compiling, Training, and Evaluating the Model

##### Model Architecture:

Neurons: 128 neurons in the first layer, 64 in the second layer, and 1 in the output layer.

Layers: 3 layers, two hidden layers with ReLU activation and an output layer with a sigmoid activation function.

Activation Functions: ReLU handled non-linear relationships, while sigmoid handled binary classification.

Model Performance: The optimized model achieved an accuracy greater than the goal of 75%.

##### Performance Improvement Steps:

Feature scaling with StandardScaler.

Balanced the data using SMOTE.

Reduced overfitting with dropout layers.

Early stopping to prevent unnecessary epochs from reducing model performance.

## Summary

The model performed accurately. Alphabet Soup Charity could make use of the model as is to better their fundraising. However, an alternative approach could involve using ensemble methods such as Random Forest or XGBoost. These libraries could help with classification tasks and feature importance.
