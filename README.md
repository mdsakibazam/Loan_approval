# Credit Wise: Loan Approval Prediction System

## 📌 Project Overview
**Credit Wise** is a machine learning-based classification project designed to predict the likelihood of loan approval for applicants. Financial institutions can use this tool to automate initial screenings, reduce manual processing time, and improve decision-making accuracy by leveraging historical data and applicant profiles.

The project implements an end-to-end data science pipeline, including data cleaning, exploratory analysis, feature scaling, and a comparative study of multiple classification algorithms.

---

## 📊 Dataset Description
The model is trained on a dataset containing **1,000 applicant records** with **20 distinct features**. The data captures a comprehensive view of an applicant's financial health and demographic background.

### Key Features:
* **Demographics**: Age, Gender, Marital Status, Education Level, and Dependents.
* **Employment**: Employment Status (Salaried/Self-employed) and Employer Category (Private/Government).
* **Financial Metrics**: Applicant Income, Co-applicant Income, Savings, and existing Credit Score.
* **Loan Details**: Loan Amount, Loan Term, Loan Purpose, and Collateral Value.
* **Target Variable**: `Loan_Approved` (Yes/No).

---

## 🛠️ Data Preprocessing & Feature Engineering
To ensure high model performance, the following preprocessing steps were conducted:
1.  **Handling Missing Values**: 
    * Numerical columns were imputed using the **Mean** strategy.
    * Categorical columns were handled using the **Most Frequent** (Mode) strategy.
2.  **Categorical Encoding**: Non-numeric data (like Employment Status and Gender) was converted into a machine-readable format using Label Encoding.
3.  **Feature Scaling**: Standard scaling was applied to numerical features to ensure that variables with larger ranges (like Income or Loan Amount) do not dominate the models.
4.  **Data Splitting**: The dataset was split into training and testing sets to evaluate model generalization on unseen data.

---

## 🤖 Machine Learning Models
The project explores a variety of supervised learning algorithms to find the most effective predictor:

* **Logistic Regression**: A baseline linear model for binary classification.
* **Decision Tree & Random Forest**: Tree-based methods to capture non-linear relationships and interactions between features.
* **Support Vector Machines (SVM)**: Used to find the optimal hyperplane for separation.
* **Naive Bayes**: A probabilistic classifier that performed exceptionally well on this specific dataset.
* **K-Nearest Neighbors (KNN)**: An instance-based learning algorithm.

---

## 📈 Results and Evaluation
The models were evaluated using a comprehensive suite of metrics: **Accuracy, Precision, Recall, and F1-Score**. 

### Performance Comparison:
| Model | Accuracy | Precision | Recall | F1-Score |
| :--- | :--- | :--- | :--- | :--- |
| **Naive Bayes** | **86.5%** | **78.3%** | **77.0%** | **0.777** |
| **Logistic Regression** | 85.0% | 83.3% | 65.6% | 0.734 |
| **Random Forest** | 83.5% | 75.4% | 70.5% | 0.729 |

*Note: The **Naive Bayes** model emerged as the most balanced and accurate predictor for this dataset.*

---

## 💻 Tech Stack
* **Language**: Python 3.x
* **Libraries**: 
    * `pandas` & `numpy`: Data manipulation
    * `seaborn` & `matplotlib`: Data visualization
    * `scikit-learn`: Machine learning and preprocessing

---

## 🚦 How to Run the Project
1.  **Clone the Repo**:
    ```bash
    git clone [https://github.com/yourusername/credit-wise.git](https://github.com/yourusername/credit-wise.git)
    ```
2.  **Install Requirements**:
    ```bash
    pip install pandas numpy seaborn matplotlib scikit-learn
    ```
3.  **Launch the Notebook**:
    Open `credit_wise.ipynb` in Jupyter Notebook or VS Code and run all cells sequentially.

---

## 📄 License
This project is licensed under the MIT License - see the LICENSE file for details.
