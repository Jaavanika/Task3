# Task3
1. These are Python libraries.

pandas → for handling data (tables, CSV).

numpy → for math (not heavily used here).

matplotlib.pyplot → for drawing graphs.

2. Some columns are text like "yes", "no", "furnished", "semi-furnished" etc.

Machine learning needs numbers, not text.

So, LabelEncoder converts them into numbers (like yes → 1, no → 0).

We loop over all columns and convert any object type column.

sklearn → for machine learning models and evaluation.

3. X = all columns except 'furnishingstatus' (these are the input features).

y = the 'furnishingstatus' column (this is the value we want to predict).

4. 80% of data goes into training (X_train, y_train).

20% goes into testing (X_test, y_test).

random_state=42 means it splits the same way every time (for reproducibility).

5. Makes a Linear Regression model.

.fit(X_train, y_train) → The model learns from the training data.

6. Model uses X_test and predicts what y (furnishingstatus) would be.

These are the predicted outputs.

7. MAE (Mean Absolute Error): How far off predictions are on average.

MSE (Mean Squared Error): Penalizes big errors even more.

R² Score: How well the model fits the data (closer to 1 is better).

8. Draws a scatter plot between actual values (real furnishingstatus) and predicted values.

Helps you visualize how well predictions match reality.
