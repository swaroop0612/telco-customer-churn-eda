📌 Telco Customer Churn – Exploratory Data Analysis (EDA)

This project performs in-depth Exploratory Data Analysis (EDA) on the Telco Customer Churn dataset.
The goal is to understand customer behavior, identify key drivers of churn, and prepare the data for further modeling.

🔍 Project Objectives :

--> Understand dataset structure

--> Handle missing values

--> Create new features (tenure groups)

--> Explore distributions of predictors

--> Analyze churn patterns

--> Visualize relationships between variables

📁 Dataset :

File: WA_Fn-UseC_-Telco-Customer-Churn.csv
Contains 7,043 customer records with 21 features, including:

--> Demographics

--> Services subscribed

--> Account information

--> Billing patterns

--> Churn status

🛠️ Technologies Used :

--> Python

--> Pandas

--> NumPy

--> Matplotlib

--> Seaborn

--> Jupyter Notebook

⚙️ Installation :

--> Clone the repo:

git clone https://github.com/<your-username>/<your-repo-name>.git


Install dependencies:

pip install -r requirements.txt


Run Jupyter Notebook:

jupyter notebook

📊 Key EDA Steps Performed
1. Data Summary :

.info() to check datatypes

.describe() for numeric stats

Identify incorrect dtypes (TotalCharges as object)

2. Missing Value Treatment :

Calculated missing %

Only 0.15% values missing in TotalCharges

Dropped missing records (safe due to small impact)

3. Feature Engineering :

Created tenure groups (1–12 months, 13–24, …, 61–72):

telco_data['tenure_group'] = pd.cut(...)

4. Univariate & Bivariate Analysis :

--> Countplots of categorical variables

--> Churn distribution by predictors

--> Tenure vs Churn

--> Contract vs Churn

--> Internet Service vs Churn

-->Histograms and barplots

📈 Insights :

--> Month-to-month contract customers churn the most

--> Long-tenure customers have low churn

--> Fiber optic users show higher churn

--> Automatic payment methods reduce churn

--> Senior Citizen and gender show weaker correlation
