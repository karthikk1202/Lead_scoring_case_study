# Lead Scoring Case Study  

This project was conducted for X Education, an online course provider, to optimize their sales process by assigning scores to leads. The aim was to identify high-potential leads, improve conversion rates, and make the sales process more efficient.  

## Problem Statement  
X Education receives thousands of leads daily through website forms, referrals, and marketing campaigns. However, only about 30% of these leads typically convert. The objective is to build a predictive model that assigns a Lead Score to each lead, indicating the probability of conversion, so that the sales team can focus on the most promising ones.

## Dataset and Preprocessing  
- Dataset: 9,240 leads with 37 features (numerical and categorical).  
- Missing values: Columns with excessive missing values dropped; others imputed using mode.  
- Encoding: Converted categorical features into numeric variables.  
- Feature Scaling: Standardized numerical features.  
- Train-test split: 70% training, 30% testing.

## Approach  
1. Explored data to identify key behavioral and demographic patterns.  
2. Built Logistic Regression as the primary model (Decision Trees were tested but found to overfit).  
3. Validated the model using accuracy, ROC-AUC, and precision-recall tradeoffs.  
4. Selected an optimal probability threshold of 0.42 to balance precision and recall.
## Model Performance  
- Accuracy: ~91% on test data  
- ROC-AUC Score: 0.96 (indicating strong predictive power)  
- Precision and Recall balanced at chosen threshold.
## Key Findings  
Top Numerical Features:
- Total Time Spent on Website → higher time = higher conversion chance  
- Lead Origin → API and Landing Page Submission leads convert better  
- Last Activity → engagement via emails/SMS boosts conversion.

Top Categorical Features: 
- Lead Source → Organic Search, Direct Traffic, and Google generate more converting leads  
- Lead Quality → "High" and "Might Be" are more promising  
- Specialization → Finance and Banking fields have higher conversions.

## Strategic Recommendations  
- Aggressive Conversion (intern hiring period): Lower lead score threshold to 30–40, prioritize high-engagement leads, and apply multi-touch campaigns (calls + emails + SMS).  
- Efficiency Mode (after targets met): Raise threshold to 80+, prioritize referral leads, and automate follow-ups before assigning sales calls.

## Conclusion  
- Data quality is critical; preprocessing was key to model reliability.  
- User behavior (time spent, activity) plays a major role in lead conversion.  
- Logistic Regression was chosen for its simplicity, interpretability, and strong performance.  
- By implementing this model, X Education can potentially increase conversions by 10–20% while reducing wasted sales efforts.  

## Tech Stack  
- Python (Pandas, NumPy, Scikit-learn, Matplotlib, Seaborn)  
- Jupyter Notebook for model building  
- PDF reports and PPT presentations for documentation  

## Applications  
- Helps sales teams prioritize leads effectively  
- Improves conversion rates while reducing wasted calls  
- Supports marketing in targeting high-quality sources  
- Provides actionable insights for resource allocation and business growth  
