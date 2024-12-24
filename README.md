# Predicted Price for Used Cars

## Project Overview
This project uses the **CRISP-DM (Cross-Industry Standard Process for Data Mining)** methodology to predict the selling price of used cars in India. It addresses a common challenge faced by individuals: determining the right selling price for their vehicles. 

The dataset was scraped from **Cars24.com** in March 2021. Due to its real-time nature, the data required significant cleaning and preprocessing to prepare it for analysis and modeling.

---

## Problem Statement
Many car owners in India struggle to determine the appropriate selling price for their vehicles. This project aims to predict the price of a used car based on several key attributes.  

**Objective**: Build a regression model that achieves an **R² score of 0.85 or higher** on test data.  
**Task**: Split the dataset into an 80-20 train-test ratio and apply various regression techniques to predict the car prices.

---

## Data Sources
The dataset was sourced from:
- [Cars24.com](https://www.cars24.com/faq/)
- Comparable platforms like [CarWale](https://www.carwale.com/) and [CarDekho](https://www.cardekho.com/).

---

## Dataset Features
The dataset contains the following attributes:

### Independent Variables
1. **Name**: Model name and year of the car.
2. **Rating**: Condition rating given during inspection.
3. **City**: Location where the car is advertised.
4. **Kilometers**: Total distance driven by the car.
5. **Year of Purchase**: Original purchase date of the car.
6. **Owner**: Number of previous owners.
7. **Fuel Type**: Type of fuel the car uses (e.g., Petrol, Diesel).
8. **Transmission**: Gear type (e.g., Manual, Automatic).
9. **RTO**: Regional Transport Office where the car is registered.
10. **Insurance**: Expiry date of the insurance.
11. **Insurance Type**: Type of insurance coverage (e.g., Comprehensive, Expired).

### Target Variable
- **Price**: Selling price of the used car.

---

## Methodology
The project follows the **CRISP-DM** process:
1. **Business Understanding**: Identify the problem and define the objectives.
2. **Data Understanding**: Collect and explore the data.
3. **Data Preparation**: Clean and preprocess the dataset for modeling.
4. **Modeling**: Apply various regression models.
5. **Evaluation**: Assess model performance using R² scores.
6. **Deployment**: Prepare the final model for use in production.

---

## Data Preprocessing
### Steps Involved:
1. **Cleaning**:
   - Removed special characters and strings from columns like `Price`, `Rating`, `Kilometers`, `Year of Purchase`, `Insurance`, etc.
   - Extracted year and month from the `Year of Purchase` column.
   - Encoded categorical variables like `Transmission` and `Insurance Type` into numerical format.

2. **Feature Engineering**:
   - Split the `Name` column into meaningful parts (e.g., Brand, Model, Year).
   - Dropped redundant columns like `Year of Purchase` after extracting relevant information.

3. **Handling Missing Values**:
   - Filled or removed null values in columns like `Transmission` and `Insurance`.

---

## Models Implemented
The following regression techniques were used to predict car prices:
1. **Polynomial Regression**
2. **Linear Regression**
3. **Decision Tree Regression**
4. **Random Forest Regression**
5. **AdaBoost Forest Regression**
6. **XGBoost Regression**

---

## Results
- **Evaluation Metric**: R² Score
- Target R² score: **≥ 0.85**
- Best-performing model: Xtream Gradirnt Boost Train
-                       r2_score 0.96237283187598

---

## Tools and Libraries Used
- **Programming Language**: Python
- **Libraries**:
  - Data Manipulation: `Pandas`, `NumPy`
  - Data Visualization: `Matplotlib`, `Seaborn`
  - Machine Learning: `Scikit-learn`, `XGBoost`
- **Environment**: Jupyter Notebook

---

## How to Run the Project
1. Clone the repository:
   ```bash
   git clone <repository-link>
   ```
2. Navigate to the project directory:
   ```bash
   cd Predicted-Price-For-Used-Cars
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Run the notebook:
   ```bash
   jupyter notebook
   ```
5. Load and execute `Predict_Used_Car_Price.ipynb`.

---

## Future Scope
- Expand the dataset with more features like car brand popularity and market trends.
- Deploy the model as a web app for user interaction.
- Integrate additional models like Gradient Boosting for enhanced performance.

---

## References
- Dataset scraped from [Cars24.com](https://www.cars24.com/).
- Additional resources: [CarWale](https://www.carwale.com/) and [CarDekho](https://www.cardekho.com/).

---

