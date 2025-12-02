# Telco Customer Churn Analysis 📉

## 📌 Project Overview
**The Business Problem:**
The telecommunications company is currently facing a **26% churn rate**, leading to significant revenue loss. Retaining existing customers is estimated to be 5-25x cheaper than acquiring new ones. The management team lacks visibility into *why* customers are leaving and needs a data-driven strategy to reduce churn.

**The Objective:**
To analyze customer demographics, services, and billing patterns to identify the key drivers of churn and provide actionable recommendations to the Sales & Customer Success teams.

## 🛠️ Tools & Technologies
* **Language:** Python 3.10
* **Libraries:** Pandas, NumPy, Seaborn, Matplotlib
* **Environment:** Google Colab 
* **Techniques:** Data Cleaning, Exploratory Data Analysis (EDA), Correlation Analysis, One-Hot Encoding.

## 📊 Key Findings & Insights
Through analysis of the dataset (7,043 customers), we identified specific "Risk Profiles":

### 1. Contract Type is the #1 Driver
Customers on **Month-to-Month contracts** churn at a rate of **42.7%**, compared to just **11%** for One-Year contracts. There is a lack of incentive for customers to commit to longer terms.

### 2. The "Fiber Optic" Trap
Surprisingly, customers with **Fiber Optic** internet (the premium service) have a higher churn rate than DSL users.
* *Hypothesis:* This indicates a potential mismatch between **Price vs. Value**, or technical reliability issues with the fiber network.

### 3. Electronic Check Payment Friction
Customers paying via **Electronic Check** have significantly higher churn compared to those using Credit Cards or Bank Transfers. This suggests the manual nature of this payment method leads to missed payments and subsequent cancellations.

![Correlation Chart]
https://github.com/prachi-majmudar/Telco_Customer_Churn/blob/main/images/correlation%20chart.png 

## 💡 Strategic Recommendations

Based on the data, I recommend the following three-pronged strategy to reduce churn by an estimated 10-15%:

| Strategy | Action Item | Target Audience |
| :--- | :--- | :--- |
| **1. The "1-Year Migration" Campaign** | Offer a **15% discount** for the first 3 months to any Month-to-Month user who upgrades to a 1-Year Contract. | Month-to-Month users with >6 months tenure. |
| **2. Fiber Optic Health Check** | Launch an automated "Service Health Check" email to Fiber users in their first 60 days to proactively address technical issues before they cancel. | New Fiber Optic subscribers. |
| **3. Payment Automation Push** | Implement a "Set it and Forget it" incentive (e.g., $5 one-time credit) for users switching from Electronic Check to Auto-Pay (Credit Card). | Users paying via Electronic Check. |

## 📂 Project Structure
* `data/`: Contains the raw CSV file (sourced from Kaggle).
* `notebooks/`: The Jupyter Notebook containing all Python code for cleaning and analysis.
* `images/`: Visualizations generated during the analysis.
* `README.md`: Project summary and findings.

## 🚀 How to Run
1. Clone this repository.
2. Open the `.ipynb` file in Google Colab or Jupyter Notebook.
3. Ensure the `WA_Fn-UseC_-Telco-Customer-Churn.csv` is in the same directory.
4. Run all cells to reproduce the analysis.
