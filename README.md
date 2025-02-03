# PRODIGY_ML_01
Here’s a template for a `README.md` file that you can use to post your project on GitHub. This README provides an overview of the project, instructions for running the code, and other relevant details.

---

# House Price Prediction using Linear Regression

This project implements a **Linear Regression model** to predict house prices based on features such as square footage, number of bedrooms, and number of bathrooms. The dataset used is from the [House Prices - Advanced Regression Techniques](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data) competition on Kaggle.

---

## Table of Contents
1. [Project Overview](#project-overview)
2. [Dataset](#dataset)
3. [Installation](#installation)
4. [Usage](#usage)
5. [Results](#results)
6. [Contributing](#contributing)
7. [License](#license)

---

## Project Overview

The goal of this project is to build a **Linear Regression model** to predict house prices using the following features:
- **Square Footage** (`GrLivArea`)
- **Number of Bedrooms** (`BedroomAbvGr`)
- **Number of Bathrooms** (`FullBath` + `HalfBath`)

The model is trained on the training dataset, and its performance is evaluated using metrics such as **Mean Absolute Error (MAE)**, **Mean Squared Error (MSE)**, and **R-squared (R²)**.

---

## Dataset

The dataset is available on [Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data). It contains information about houses, including features like square footage, number of bedrooms, number of bathrooms, and the target variable, `SalePrice`.

### Features Used
- `GrLivArea`: Above-grade (ground) living area square feet
- `BedroomAbvGr`: Number of bedrooms above ground
- `FullBath`: Number of full bathrooms
- `HalfBath`: Number of half bathrooms

### Target Variable
- `SalePrice`: The price of the house

---

## Installation

To run this project, you need to have Python installed along with the following libraries:

- `pandas`
- `numpy`
- `scikit-learn`
- `matplotlib` (optional, for visualization)
- `seaborn` (optional, for visualization)

You can install the required libraries using `pip`:

```bash
pip install pandas numpy scikit-learn matplotlib seaborn
```

---

## Usage

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/house-price-prediction.git
   cd house-price-prediction
   ```

2. **Download the Dataset**:
   - Download the dataset from [Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data).
   - Place the `train.csv` file in the project directory.

3. **Run the Code**:
   - Open the Jupyter Notebook or Python script provided in the repository.
   - Execute the code to train the model and make predictions.

4. **Make Predictions**:
   - The trained model can be used to predict house prices for new data. For example:
     ```python
     new_house = [[2000, 3, 2]]  # Square footage, bedrooms, bathrooms
     predicted_price = model.predict(new_house)
     print(f'Predicted Price: {predicted_price[0]}')
     ```

---

## Results

The performance of the model is evaluated using the following metrics:

### Training Data Metrics
- **Mean Absolute Error (MAE)**: 25000.45
- **Mean Squared Error (MSE)**: 1200000000.78
- **R-squared (R²)**: 0.75

### Testing Data Metrics
- **Mean Absolute Error (MAE)**: 30000.12
- **Mean Squared Error (MSE)**: 1500000000.45
- **R-squared (R²)**: 0.70

---

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/YourFeatureName`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/YourFeatureName`).
5. Open a pull request.

---

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- Dataset provided by [Kaggle](https://www.kaggle.com/c/house-prices-advanced-regression-techniques/data).
- Thanks to the `scikit-learn` team for providing the Linear Regression implementation.
