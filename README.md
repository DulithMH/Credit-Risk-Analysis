📊 Key Insights from EDA


Detailed Exploratory Data Analysis was performed using Plotly to visualize risk factors:

Wealth Levels: Analysis of Checking and Saving accounts revealed that individuals with "Little" wealth carry a statistically higher risk of default.

Loan Purpose: Using Radar (Polar) Charts, we identified that loans for Education and Business often have different risk profiles compared to Radio/TV or Cars.

Demographics: Age and Housing status (Own vs. Rent) were identified as strong indicators of stability.

🛠️ Technical Implementation
1. Modern Data Pipeline
I implemented a modular Scikit-Learn Pipeline using ColumnTransformer to ensure clean, reproducible data transformations:

Numerical Features: Imputed missing values with the median and applied StandardScaler.

Categorical Features: Handled missing categories as "Unknown" and applied OneHotEncoder.

Compatibility: The code is optimized for NumPy 1.24+, fixing legacy AttributeError issues related to deprecated np.object types.

2. Handling Class Imbalance
The dataset is naturally imbalanced (more "Good" risks than "Bad"). To prevent model bias, the project incorporates:

SMOTE (Synthetic Minority Over-sampling Technique) to balance the training set.

Evaluation Metrics: Shifting focus from simple Accuracy to Recall and F1-Score.

🚀 How to Run
Clone the Repo:

Bash

git clone https://github.com/YourUsername/Credit-Risk-Analysis.git
Install Dependencies:

Bash

pip install pandas numpy scikit-learn plotly
Run the Notebook: Open the .ipynb file in Google Colab or Jupyter Lab.

📈 Future Work
[ ] Implement XGBoost and LightGBM for improved gradient boosting performance.

[ ] Fine-tune hyperparameters using GridSearchCV.

[ ] Deploy the model as a web API using Flask or FastAPI.

Contact
Your Name - [DulithMH](https://www.linkedin.com/in/dulith-m-h-172709256?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app)

Project Link: https://github.com/YourUsername/Credit-Risk-Analysis
