# Simple Linear Regression Visualization

This repository contains Python code for implementing and visualizing a simple linear regression model. The code demonstrates how to fit a linear regression model to synthetic data, plot the regression line, and visualize the residuals.

## Table of Contents

1. [Overview](#overview)
2. [Requirements](#requirements)
3. [Installation](#installation)
4. [Usage](#usage)
5. [How It Works](#how-it-works)
6. [Examples](#examples)
7. [Results](#results)
8. [Troubleshooting](#troubleshooting)
9. [FAQs](#faqs)
10. [License](#license)
    
## Overview

This project demonstrates the application of simple linear regression using `scikit-learn`. The code generates synthetic data, fits a linear regression model, and visualizes the regression line along with the data points and residuals using `matplotlib`.

## Requirements

To run the code, you'll need to install the following Python libraries:

- `numpy`
- `matplotlib`
- `scikit-learn`

You can install these libraries using pip:

```bash
pip install numpy matplotlib scikit-learn
```

## Installation

1. **Clone the Repository**:

    ```bash
    git clone https://github.com/yourusername/simple-linear-regression-visualization.git
    ```

2. **Navigate to the Project Directory**:

    ```bash
    cd simple-linear-regression-visualization
    ```

3. **Install Required Libraries**:

    ```bash
    pip install numpy matplotlib scikit-learn
    ```

## Usage

1. **Run the Python Script**:

    Execute the Python script to train the linear regression model and generate the visualization:

    ```bash
    python linear_regression_visualization.py
    ```

2. **View the Output**:

    The script will display a plot showing:
    - The data points.
    - The regression line.
    - Residuals as dashed lines.

## How It Works

### Data Generation

- **Features (`X`)**: X is a feature matrix with 100 data points, generated randomly.
- **Targets (`y`)**: y is the target variable with a linear relationship plus some random noise.
  
### Model Training

- **Model**: A linear regression model is created using `scikit-learn` and trained with the synthetic data.

### Prediction

- **New Data Points**: Generated to plot the regression line over a range of values. Predictions are made on new data points (X_new) to plot the regression line.

### Visualization

- **Scatter Plot**: Displays the original data points.
- **Regression Line**: Plotted in red to show the model’s predictions.
- **Residuals**: Green dashed lines indicate the vertical distance between each data point and the regression line.

### Metrics

Mean Squared Error (MSE) and R^2 Score are calculated to evaluate model performance.

- **Mean Squared Error (MSE)**: Measures the average squared difference between observed and predicted values.
- **R^2 Score**: Indicates the proportion of variance in the dependent variable that is predictable from the independent variable.

## Examples

### Basic Execution

Run the provided script to visualize the linear regression model:

```bash
python linear_regression_visualization.py
```

### Customization

You can modify the following parameters in the script to experiment with different scenarios:

- **Noise Level**: Adjust the noise added to the target variable.
- **Feature Range**: Change the range of `X_new` to visualize the regression line over different feature values.

## Results

The script generates a plot with:
- **Data Points**: Blue dots representing the original data.
- **Regression Line**: Red line showing the fitted model.
- **Residuals**: Green dashed lines indicating the errors for each data point.

Additionally, the Mean Squared Error and R^2 Score are printed to the console to evaluate model performance.

## Output

![Output1](https://github.com/AartiDashore/SimpleLinearRegressionVisualization/blob/main/Output1.png)

## Troubleshooting

### Common Issues

1. **Module Not Found Error**:
    - Ensure all required libraries are installed correctly.
    - Verify your Python environment.

2. **Plot Not Displaying**:
    - Ensure that `matplotlib` is installed and properly configured.
    - Try running the script in an environment that supports plotting, such as Jupyter Notebook or a local IDE.

## FAQs

### What is Linear Regression?

Linear regression is a statistical method used to model the relationship between a dependent variable and one or more independent variables by fitting a linear equation to observed data.

### What are Residuals?

Residuals are the differences between the observed values and the values predicted by the model. They represent the error or deviation of the predictions from the actual data.

### How do I interpret the R^2 Score?

The R^2 Score represents the proportion of variance in the dependent variable that is predictable from the independent variable. A higher R^2 Score indicates a better fit of the model to the data.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
