### **Objective**
The goal is to build a logistic regression model that assigns a lead score between 0 and 100 to leads based on their likelihood of conversion. This will help X Education's sales team focus their efforts on high-potential leads, thereby improving the overall lead conversion rate.

---

### **Steps Followed**

#### 1. **Reading Data**
   - **Dataset:** Load `Leads.csv` to analyze the lead attributes and conversion labels.
   - **Data Dictionary:** Refer to `Leads Data Dictionary.xlsx` to understand the meaning of each attribute and its data type.

#### 2. **Data Cleaning**
   - Handle missing values using appropriate imputation techniques (e.g., mean/median for numerical data, mode/constant for categorical data).
   - Remove redundant or irrelevant columns, such as those with a high percentage of missing values or low variance.
   - Standardize column names for consistency.

#### 3. **Exploratory Data Analysis (EDA)**
   - Analyze key attributes influencing lead conversion rates (e.g., traffic sources, time spent on the website).
   - Use visualization tools like bar plots, histograms, and correlation matrices to uncover patterns and trends.
   - Identify any class imbalance in the target variable (`Converted`).

#### 4. **Creating Dummy Variables**
   - Convert categorical variables into numerical format using one-hot encoding or label encoding.
   - Ensure the dummy variables align with logistic regression requirements.

#### 5. **Splitting Data into Training and Testing Sets**
   - Split the dataset into a training set (70-80%) and a test set (20-30%) to evaluate model performance.
   - Use stratified sampling to maintain the target class ratio in both subsets.

#### 6. **Building the Logistic Regression Model**
   - Implement logistic regression with regularization (e.g., L1/L2 penalty) to prevent overfitting.
   - Select relevant features using statistical tests or automated feature selection techniques (e.g., Recursive Feature Elimination).

#### 7. **Making Predictions**
   - Use the model to calculate lead scores (probabilities of conversion) for each lead.
   - Scale probabilities to a score range of 0-100.

#### 8. **Model Evaluation**
   - Evaluate the model using metrics like:
     - **Accuracy**: Overall correctness.
     - **Precision**: Proportion of true positives among predicted positives.
     - **Recall**: Proportion of true positives identified.
     - **F1-Score**: Harmonic mean of precision and recall.
   - Use a **confusion matrix** to assess model performance.

#### 9. **ROC Curve**
   - Plot the Receiver Operating Characteristic (ROC) curve to evaluate the tradeoff between true positive rate and false positive rate.
   - Calculate the Area Under the Curve (AUC) to assess model discriminative ability.

#### 10. **Prediction on Test Set**
   - Use the test dataset to predict lead scores and evaluate the model’s ability to generalize.

#### 11. **Precision-Recall Curve**
   - Plot the Precision-Recall curve to focus on the performance for the minority class (converted leads).

---

### **Details of Files**
- **Lead Score Case Study.ipynb:** Python file containing code and analysis.
- **Assignment Subjective Questions.pdf:** Answers to subjective questions, including methodology and insights.
- **Lead Score Case Study PPT.pdf:** Presentation slides summarizing findings and recommendations.
- **Summary.pdf:** Concise documentation of the work done.
