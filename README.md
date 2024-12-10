# Income, Race, and Education Analysis: A Comprehensive Machine Learning Study

## Project Overview
This data science project employs advanced machine learning techniques to analyze a detailed census dataset, exploring the intricate relationships between socioeconomic factors, income, and demographic characteristics.

## Dataset Characteristics
- **Total Samples**: 32,537 (after removing duplicates)
- **Features**: 15 columns including age, workclass, education, race, sex, income, and more

## Key Visualizations and Insights

### Demographic Composition
- **Race Distribution**: 
  - White: 85.4%
  - Black: 9.6%
  - Asian-Pacific Islander: 3.2%
  - Other races: 2.8%
- **Gender Distribution**: 
  - Male: 67.0%
  - Female: 33.0%

### Financial Dynamics
#### Capital Gains and Losses
- **Capital Gains by Gender**:
  - Males: Average of $1,330.29
  - Females: Average of $568.89
  - Significant gender-based disparity in financial investments

#### Income by Life Stage
- **Middle-Aged Income Distribution**:
  - Males: 70.6%
  - Females: 29.4%
- **Retiree Income Distribution**:
  - Males: 66.8%
  - Females: 33.2%

#### Income by Marital Status
- **Earning Over $50k**:
  1. Married-Civil Spouse: 6,690
  2. Never Married: 491
  3. Divorced: 463
- **Earning $50k or Less**:
  1. Never Married: 10,176
  2. Married-Civil Spouse: 8,280
  3. Divorced: 3,978

### Educational Landscape
- **Top 5 Education Levels**:
  1. High School Graduate
  2. Some College
  3. Bachelors
  4. Masters
  5. Vocational Associate Degree

### Occupation and Work Insights
- **Top Occupations**:
  1. Professional Specialty
  2. Craft Repair
  3. Executive/Managerial
  4. Administrative Clerical
  5. Sales
- **Average Work Hours by Race**:
  1. White: 40.69 hours/week
  2. Asian-Pacific Islander: 40.13 hours/week
  3. American Indian/Eskimo: 40.05 hours/week
  4. Other: 39.47 hours/week
  5. Black: 38.43 hours/week

## Machine Learning Methodology

### Data Preprocessing
1. **Feature Encoding**:
   - Transformed categorical variables to numerical format using LabelEncoder
   - Ensured machine learning algorithm compatibility

2. **Feature Selection**:
   - Applied Chi-square test to identify most relevant features
   - Selected 9 key features: age, workclass, education, marital status, occupation, relationship, race, sex, and hours per week

3. **Data Preparation**:
   - Split data into 80% training and 20% testing sets
   - Used consistent random state for reproducibility

### Model Performance Comparison

#### 1. Logistic Regression
- **Accuracy**: 77.01%
- **Precision**: 50.83%
- **F1 Score**: 26.88%

#### 2. K-Nearest Neighbors (KNN)
- **Best Parameters**: 
  - Neighbors: 6
  - Weights: None
- **Performance**:
  - Accuracy: 82.01%
  - Precision: 65.18%
  - F1 Score: 55.05%

#### 3. Support Vector Classifier (SVC)
- **Best Parameters**:
  - Regularization (C): 4
  - Kernel: Radial Basis Function (RBF)
- **Performance**:
  - Accuracy: 81.59%
  - Precision: 61.55%
  - F1 Score: 57.73%

#### 4. Random Forest Classifier
- **Best Parameters**:
  - Estimators: 200
  - Max Depth: 12
  - Min Samples Split: 8
- **Top Performer**:
  - Accuracy: 84.34%
  - Precision: 69.44%
  - F1 Score: 63.01%

#### 5. CatBoost Classifier
- **Best Parameters**:
  - Depth: 4
  - Learning Rate: 0.1
  - Estimators: 250
- **Performance**: Similar to Random Forest

#### 6. XGBoost Classifier
- **Best Parameters**:
  - Learning Rate: 0.07
  - Estimators: 150
- **Performance**: Comparable to Random Forest

### ROC Curve Analysis
The Receiver Operating Characteristic (ROC) curve revealed:
- Random Forest: Best Area Under Curve (AUC)
- XGBoost: Highly competitive performance
- K-Nearest Neighbors: Solid predictive power
- Logistic Regression: Most limited performance

## Technologies and Libraries
- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Seaborn
- XGBoost
- CatBoost

## Key Observations
1. Significant gender disparities in income and capital gains
2. Strong correlation between marital status and income levels
3. Complex interactions between race, education, and economic opportunities

## Research Limitations
- Represents a specific demographic sample
- Data from a particular time period
- Broad categorical classifications may oversimplify individual experiences

## Potential Future Research
- Detailed income inequality analysis
- Intersectional studies of race, gender, and economic outcomes
- Long-term trends in educational and professional attainment
- Comprehensive factors influencing capital gains

## Recommendations
1. Utilize Random Forest for income prediction tasks
2. Prioritize ensemble machine learning methods
3. Invest in sophisticated feature engineering
4. Consider broader, more nuanced demographic categories

## Conclusion
This project demonstrates the power of data science and machine learning in unraveling complex socioeconomic patterns. By combining advanced statistical techniques with comprehensive data analysis, we've gained profound insights into the multifaceted nature of income, education, and demographic interactions.

