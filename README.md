# Linear Regression From Scratch

This project implements a simple linear regression model from scratch using Python, NumPy, and Pandas. The goal is to predict a dependent variable based on an independent variable by fitting a linear equation to the observed data.

## Notebook: `main.ipynb`

The Jupyter Notebook, [`main.ipynb`](main.ipynb), contains the complete implementation and is structured as follows:

1.  **Data Loading and Preprocessing**: The notebook starts by loading the dataset using Pandas and separating it into independent (`X`) and dependent (`y`) variables.
2.  **Model Implementation**:
    *   **Cost Function**: It defines a function to calculate the Mean Squared Error (MSE), which measures the average squared difference between the estimated values and the actual value.
    *   **Gradient Descent**: The core of the learning algorithm. This function iteratively adjusts the model's parameters (slope and intercept) to minimize the cost function.
3.  **Training**: The model is trained on the dataset for a specified number of iterations with a defined learning rate. The process of minimizing the cost is visualized to ensure convergence.
4.  **Prediction**: Once trained, the model can be used to make predictions on new data.
5.  **Visualization**: The final step is to visualize the results. The notebook plots the original data points as a scatter plot and overlays the linear regression line that best fits the data. This graph is saved as [`output.png`](output.png).

## Dataset

The model is trained on the California Housing dataset. The goal is to predict the median house value for California districts based on various features from the 1990 census. You can find the dataset used in this project here:

[California Housing Dataset](https://github.com/ageron/handson-ml2/tree/master/datasets/housing)

The raw CSV file can be downloaded directly from:
`https://raw.githubusercontent.com/ageron/handson-ml2/master/datasets/housing/housing.csv`

## Output

The following graph shows the original data points and the regression line learned by the model.

![Linear Regression Model Output](output.png)