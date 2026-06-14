# Housing-Price-Prediction-Using-ML-Neural-Networks

## Project Overview
Pricing real estate is a high-stakes challenge often influenced by human bias, shifting economies, and localized market volatility. Traditional methods can easily miss broader market patterns, leading to unstable valuations. 

This project seeks to replace human guesswork with a resilient, data-driven mathematical framework. By analyzing the **Ames Housing Dataset**—a highly detailed residential ledger tracking 79 distinct property characteristics—this project builds, optimizes, and stress-tests machine learning models to accurately predict housing prices. 

## Summary of Findings
Through rigorous Exploratory Data Analysis (EDA) and machine learning implementation, several key insights were uncovered:

* **Quality Outweighs Quantity:** While raw square footage establishes a baseline minimum value for a property, subjective overall quality acts as a massive financial multiplier. 
* **Neural Network Superiority:** A baseline Multiple Linear Regression model struggled to capture complex market patterns ($R^2$ = 0.10). By implementing a Feed-Forward Neural Network, the Mean Squared Error (MSE) was reduced by billions, and the $R^2$ score improved to 0.44, proving the neural network's ability to map non-linear housing trends.
* **Scenario Analysis (Market Stress Testing):** Simulated market shifts proved that in an economic squeeze, dropping a home's quality severely damages its valuation. Conversely, upgrading a home's quality completely offsets the financial penalty of shrinking its square footage.
* **Actionable Recommendation:** Sellers and flippers should prioritize capital investments in cosmetic and systemic quality repairs rather than costly structural additions to protect equity.

## Project Structure
* **Data Preprocessing:** Handled missing values (median/mode imputation), engineered combined features (Total Square Footage), applied one-hot encoding for categorical variables, and standardized features using `StandardScaler`.
* **Baseline Modeling:** Implemented a Multiple Linear Regression model to establish a performance benchmark.
* **Advanced Modeling:** Designed and optimized a Feed-Forward Neural Network (64-to-32 neuron architecture) using TensorFlow/Keras with Early Stopping regularization.
* **Scenario Simulation:** Stress-tested the optimized neural network against 3 hypothetical market shifts (Remote Work Expansion, Economic Squeeze, Eco-Minimalist Trend).
* **Interactive Dashboard:** Built a dynamic Power BI dashboard featuring market distribution histograms, interactive scatter plots, and KPI tracking to visualize model performance and market truths.

## Dependencies and Technologies Used
To run this project locally, you will need the following tools and Python libraries:

* **Environment:** Jupyter Notebook / JupyterLab
* **Language:** Python 3.x
* **Core Libraries:**
  * `pandas` (Data manipulation)
  * `numpy` (Numerical operations)
  * `matplotlib` & `seaborn` (Data visualization)
  * `scikit-learn` (Preprocessing, splitting, and baseline modeling)
  * `tensorflow` / `keras` (Neural network architecture and training)
  * `openpyxl` (Exporting metrics to Excel)
* **Visualization Software:** Microsoft Power BI Desktop (for the `.pbix` dashboard file)

## How to Run the Project
1. Clone this repository to your local machine.
2. Ensure you have the required dependencies installed. You can install them via pip:
   ```bash
   pip install pandas numpy matplotlib seaborn scikit-learn tensorflow openpyxl
