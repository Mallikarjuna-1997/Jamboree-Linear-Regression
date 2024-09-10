# Jamboree Linear Regression Project

## Project Overview

This project focuses on predicting the probability of a student getting admitted to an Ivy League college based on multiple factors such as GRE scores, TOEFL scores, CGPA, research experience, and more. The project utilizes **linear regression** models to understand which variables most significantly impact the admission chances and how they interact with one another.

The analysis was conducted using a dataset from Jamboree, which contains information about students' profiles and their admission probabilities. The results of the regression analysis will assist Jamboree in providing better guidance to prospective students.

## Dataset

The dataset contains the following variables:
- **GRE Score**: Graduate Record Examination score.
- **TOEFL Score**: Test of English as a Foreign Language score.
- **University Rating**: A rating of the university (on a scale of 1 to 5).
- **SOP**: Statement of Purpose strength (on a scale of 1 to 5).
- **LOR**: Letter of Recommendation strength (on a scale of 1 to 5).
- **CGPA**: Cumulative Grade Point Average.
- **Research**: A binary variable indicating whether the student has research experience (1 for Yes, 0 for No).
- **Chance of Admit**: The probability of admission (a value between 0 and 1).

## Project Structure

- **Jamboree_LinearRegression.ipynb**: This Jupyter Notebook contains the full data analysis and modeling process.
- **data/Jamboree_Admission.csv**: The dataset used for this analysis.
- **models/**: Saved models from the linear regression analysis.
- **visualizations/**: Plots and visualizations generated from the data analysis.

## Key Steps

1. **Data Preprocessing**:
   - Loaded the dataset and performed initial cleaning (removal of duplicates and outliers).
   - Checked for missing values and handled them accordingly.

2. **Exploratory Data Analysis**:
   - Visualized the distribution of each feature using histograms and boxplots.
   - Created a correlation heatmap to understand relationships between variables.

3. **Modeling**:
   - Implemented **Ordinary Least Squares (OLS)** regression to predict the `Chance of Admit`.
   - Evaluated model performance using metrics such as **R-squared**, **Mean Absolute Error (MAE)**, and **Root Mean Squared Error (RMSE)**.
   - Compared the performance of **Ridge**, **Lasso**, and **ElasticNet** regression models to address multicollinearity.

4. **Insights**:
   - CGPA is the most significant predictor of admission chances.
   - GRE and TOEFL scores positively influence admission chances.
   - Research experience also plays an important role in determining admission probability.
   - University Rating and SOP have relatively weaker effects.

## Installation and Requirements

To run this project, you will need the following Python libraries:
- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`
- `statsmodels`
- `scikit-learn`

You can install the dependencies using the following command:
```bash
pip install -r requirements.txt
```

## Usage

To run the analysis, open the **Jamboree_LinearRegression.ipynb** notebook in Jupyter or Google Colab. Ensure that the dataset is placed in the correct directory, and the necessary dependencies are installed.

## Results

- The OLS regression model achieved an **R-squared** value of 0.826, explaining 82.6% of the variance in the `Chance of Admit`.
- The model confirms that academic performance (CGPA, GRE, TOEFL) and research experience are key predictors of admission chances.

## Future Improvements

- Consider adding more features to improve the prediction accuracy.
- Explore non-linear models to capture more complex relationships between variables.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
