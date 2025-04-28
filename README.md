# LendingClub Loan Default Prediction 📊🚀

## Overview
LendingClub is a major US peer-to-peer lending company. This project aims to **predict** whether a borrower will **repay** a loan or **default** using historical loan data.  
We build a **binary classification model** using **Keras** and **TensorFlow**, preparing the way for real-world deployment to assess new customer applications.

## Project Goal
- Predict the probability of loan repayment based on customer and loan data.
- Help minimize financial risk by identifying high-risk borrowers.
- Evaluate model performance using classification metrics such as **accuracy**, **precision**, **recall**, **ROC-AUC**, etc.

## Dataset Information
- Data Source: LendingClub public loan dataset (Kaggle)
- Target Variable: `loan_status`
  - Typically values like `"Fully Paid"` vs `"Charged Off"`
- Features include:
  - **Loan Info:** Amount, Term, Interest Rate, Installment
  - **Borrower Info:** Employment Length, Annual Income, Home Ownership
  - **Credit Info:** DTI (Debt-to-Income Ratio), Revolving Balance, Public Records
  - **Others:** Purpose of Loan, State, Application Type

| Feature | Description |
|:---|:---|
| loan_amnt | Amount of the loan applied for |
| term | Duration of the loan (in months) |
| int_rate | Interest rate on the loan |
| installment | Monthly payment |
| grade | LendingClub assigned loan grade |
| sub_grade | LendingClub assigned loan sub-grade |
| emp_title | Borrower's job title |
| emp_length | Employment length |
| home_ownership | Home ownership status |
| annual_inc | Annual income |
| verification_status | Income verification status |
| issue_d | Loan funding month |
| loan_status | **Target variable**: Current status of the loan |
| purpose | Purpose of the loan |
| title | Loan title |
| zip_code | Borrower's ZIP code |
| addr_state | Borrower's state |
| dti | Debt-to-Income ratio |
| earliest_cr_line | Earliest credit line opening date |
| open_acc | Number of open credit lines |
| pub_rec | Number of derogatory public records |
| revol_bal | Revolving balance |
| revol_util | Revolving line utilization rate |
| total_acc | Total number of credit lines |
| initial_list_status | Initial listing status |
| application_type | Individual or joint application |
| mort_acc | Number of mortgage accounts |
| pub_rec_bankruptcies | Number of public record bankruptcies |

## 📂 Dataset Access
Due to GitHub file size restrictions, the full LendingClub dataset is not stored directly in this repository.

**Please download the dataset manually** from this Google Drive link:

👉 [Download LendingClub Dataset](https://drive.google.com/file/d/1UZ_2jdE6tX43mFAtI0BfZ-CCq1tcYz13/view?usp=drive_link)
👉 [Download LendingClub info Dataset](https://drive.google.com/file/d/19Dvya2RRY8ZVQRWnit46OXcTxdOqhClr/view?usp=drive_link)


After downloading:
- Save the `.csv` file into the project folder.
- Make sure the file path matches the code (or modify the path accordingly).

## Project Workflow
1. **Data Preprocessing** 🧹
   - Handling missing values
   - Feature engineering (e.g., encoding categorical variables)
   - Creating dummy variables (0/1)
2. **Exploratory Data Analysis (EDA)** 🔎
   - Understanding patterns and distributions
3. **Model Building** 🛠
   - Keras Sequential API
   - Dense layers + Dropout layers
   - Sigmoid activation for binary classification
4. **Model Evaluation** 🧪
   - Accuracy, Precision, Recall, Confusion Matrix
   - ROC Curve and AUC Score
5. **Prediction on New Data** 🧑‍💻
   - Model predicts whether a new applicant is likely to default.

## Technologies Used
- Python 🐍
- Pandas, NumPy
- Matplotlib, Seaborn (for visualization)
- Scikit-learn (for preprocessing and evaluation)
- TensorFlow & Keras (for model building)

## How to Run
1. Clone the repository
2. Install dependencies:
   ```bash
   pip install -r requirements.txt

3.Run the notebook or Python scripts step-by-step.

4.Predict new applicants by passing data into the trained model.

## Results
- Achieved around XX% accuracy (you can fill this in after your results).

- Model shows strong capability to distinguish between repaid and defaulted loans.

## Future Improvements
- Hyperparameter tuning with KerasTuner or RandomSearch

- Try advanced models like XGBoost, LightGBM for comparison

- Deployment with Flask API or Streamlit web app

## Acknowledgments
- LendingClub for providing the dataset

- Kaggle for hosting public datasets

- TensorFlow and Keras teams for amazing ML libraries

## 🚀 Let's reduce financial risk with data-driven lending decisions!
