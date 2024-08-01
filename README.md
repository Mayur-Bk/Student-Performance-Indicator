# Student Performance Indicator

The purpose of this project is to analyze and determine if any factors are affecting students' test performance scores. By utilizing machine learning, the model predicts the score of a student after computing various factors involved in test performance.

## Features

- **Score Prediction**: The ML model predicts a student's test score based on various factors.
- **Deployment**: The model is deployed using Flask and AWS Elastic Beanstalk, making it accessible via a web interface.

## Deployment

The application is deployed using Flask and AWS Elastic Beanstalk and can be accessed locally at `http://127.0.0.1:5000/`.

![Webpage gif](https://github.com/user-attachments/assets/3bfb4cc9-6055-48b3-8e63-6eda010e4848)

## Setup Instructions

To set up the project locally, follow these steps:

1. **Clone the repository:**
    ```bash
    git clone https://github.com/Mayur-Bk/Student-Performance-Indicator.git
    cd Student-Performance-Indicator
    ```

2. **Create a virtual environment:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. **Install the dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4. **Run the application:**
    ```bash
    flask run
    ```
   The application will be available at `http://127.0.0.1:5000/`.

## Exploratory Data Analysis (EDA)

The EDA process helps in understanding the data, identifying patterns, and uncovering insights. The detailed EDA for this project can be found in the [EDA Student Performance Indicator](https://github.com/Mayur-Bk/Student-Performance-Indicator/blob/main/notebook/data/EDA%20Student%20Performance%20Indicator.ipynb) notebook.

### Key Insights and Visualizations

1. **Distribution of Scores**:
   ![Distribution of Scores](path/to/distribution_of_scores.png)
   - This graph shows the overall distribution of student test scores.

2. **Correlation Heatmap**:
   ![Correlation Heatmap](path/to/correlation_heatmap.png)
   - This heatmap visualizes the correlations between different features and the test scores, highlighting which factors have the strongest relationships.

3. **Feature Impact**:
   ![Feature Impact](path/to/feature_impact.png)
   - This bar chart displays the importance of each feature in predicting the student's test score.

4. **Scores by Gender**:
   ![Scores by Gender](path/to/scores_by_gender.png)
   - This visualization compares the test scores between male and female students.

5. **Scores by Parental Education Level**:
   ![Scores by Parental Education Level](path/to/scores_by_parental_education.png)
   - This graph shows the impact of parental education level on student test scores.

For more detailed visualizations and insights, please refer to the [EDA Student Performance Indicator](https://github.com/Mayur-Bk/Student-Performance-Indicator/blob/main/notebook/data/EDA%20Student%20Performance%20Indicator.ipynb) notebook.

## Model Training

The model training process involves the following steps:

1. **Data Preprocessing**: Handling missing values, encoding categorical variables, and feature scaling.
2. **Feature Selection**: Identifying important features that impact student performance.
3. **Model Selection**: Training various models (Linear Regression, Ridge, Lasso, K-Neighour Regressor, Decision Trees, Random Forest Regressor, XGB Regressor, CatBoost Regressor, AdaBoost Regressor) and selecting the best-performing (Linear Regression) model based on metrics such as MAE, R^2 and RMSE.
4. **Model Evaluation**: Evaluating the model using test data and cross-validation techniques to ensure generalization.

For detailed steps, please refer to the [Model_training.ipynb](https://github.com/Mayur-Bk/Student-Performance-Indicator/blob/main/notebook/data/Model_training.ipynb) notebook.

## Usage

1. Open your web browser and navigate to `http://127.0.0.1:5000/`.
2. Enter the required details to get a prediction of the student's test score.

## Dependencies

The project requires the following Python libraries:

- Flask
- scikit-learn
- Pandas
- NumPy

Make sure to install all dependencies listed in `requirements.txt`.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Contact

For any questions or feedback, please contact Mayur Bk at mayurbelgaumkar03@gmail.com.
