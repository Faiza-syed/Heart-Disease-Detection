## Overview
This project predicts the likelihood of heart disease using machine learning models and provides a user-friendly interface built with Django. The application processes health-related data to determine the presence or absence of heart disease based on input features such as BMI and sleep time.

## Dataset
The dataset used for this project, `heart_2020_1.csv`, includes information on various health and lifestyle factors. It contains 18 variables that are used to predict the likelihood of heart disease. Key features include BMI, PhysicalHealth, MentalHealth, SleepTime, and more.

## Data Preprocessing
- **Steps:**
  - Categorical columns are encoded using `LabelEncoder`.
  - Numerical features (e.g., BMI, PhysicalHealth, SleepTime) are standardized using `StandardScaler`.
  - Missing values are removed to ensure clean data for model training.

## Feature Selection
- The Decision Tree Classifier is used to identify the most relevant features for prediction.
- Features surpassing a set importance threshold are selected for training the final model.
- Visualizations (e.g., bar charts) illustrate the importance of selected features.

## Classification
- **Logistic Regression Classifier**: A model is trained using the selected features and tested for its performance.
- Predictions are based on input features, such as BMI and sleep time, to indicate the likelihood of heart disease.

## Performance Metrics
- **Confusion Matrix**: This evaluates the model’s performance by analyzing true positives, true negatives, false positives, and false negatives.

## Web Interface
The application features a Django-based web interface:
- **Technologies Used:**
  - Python, Django Framework
  - HTML, CSS (with responsive design)
- **Key Files:**
  - `settings.py`: Contains project configuration details.
  - `models.py`: Defines the data models for preprocessing, feature selection, and evaluation.
  - `forms.py`: Captures user input for predictions.
  - `views.py`: Processes user input, runs the prediction model, and renders results.
  - `base.html`: Provides the main user interface.
  - `urls.py`: Manages URL routing within the application.

## Predicate Logic
The project incorporates predicate logic for rule-based analysis. For example:
- **Rule 1**: Individuals with low sleep time and high BMI are more likely to have heart disease.
- **Rule 2**: Individuals with sufficient sleep time and normal BMI are less likely to have heart disease.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/Faiza-syed/Heart-Disease-Detection.git
   ```
2. Navigate to the project directory:
   ```bash
   cd Heart-Disease-Detection
   ```
3. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the Django development server:
   ```bash
   python manage.py runserver
   ```
5. Access the web interface at `http://127.0.0.1:8000/`.

## Usage
1. Upload your health data in the required format.
2. Enter relevant details (e.g., BMI, sleep time) in the provided form.
3. View the prediction results and associated metrics.

## Acknowledgments
- **Libraries Used:** scikit-learn, NumPy, pandas, Django
- **Inspiration:** Health-focused machine learning applications.

---
For more details, check out the project documentation and source code.

