# Fuel Efficiency Prediction

This project predicts the fuel efficiency (MPG) of a car based on its features like cylinders, horsepower, weight, etc. It uses a Linear Regression model to make the predictions.

## Dataset

The project uses the [Auto MPG dataset](https://archive.ics.uci.edu/ml/datasets/auto-mpg) from the UCI Machine Learning Repository. The dataset contains information about cars from the 1970s and 1980s.

The features used for prediction are:
- Cylinders
- Displacement
- Horsepower
- Weight
- Acceleration
- Model Year
- Origin (USA, Europe, Japan)

## Requirements

To run this project, you need Python and the following libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- jupyter

You can install the required libraries using pip:
```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

## Usage

1. Clone this repository or download the files.
2. Make sure you have the `auto-mpg.data` file in the same directory.
3. Open the `fuel_efficiency_model.ipynb` file in a Jupyter Notebook environment.
4. Run the cells in the notebook sequentially.

## Model

The project uses a `LinearRegression` model from the `scikit-learn` library. The model is trained on 80% of the data and tested on the remaining 20%.

## Evaluation

The model's performance is evaluated using two metrics:
- **Mean Squared Error (MSE):** Measures the average squared difference between the actual and predicted values.
- **R2 Score:** Represents the proportion of the variance in the dependent variable that is predictable from the independent variables.

The notebook also includes a classification report and a confusion matrix by converting the continuous MPG prediction into three discrete categories:
- **Low:** MPG < 17
- **Medium:** 17 <= MPG < 29
- **High:** MPG >= 29

## Interactive Prediction

The final cell in the notebook is an interactive form where you can input the features of a car to get a real-time MPG prediction.
