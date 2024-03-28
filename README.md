# Credit Risk Analysis
### Summary
Credit Risk Model is constructed by Financial Institutions to determine the likelihood of default(not able to make timely payments).

<img src=/Images/credit_risk.png width=80% height=80%>

The target of this model is to assess the likelihood of loan default and decide whether to extend the loan to borrowers. Common features include lender's credit history(e.g., credit score and utilization rate), borrower's personal information(e.g., income level and home ownership), and loan characteristics(e.g., loan amount and interest rate).

### Dataset
LendingClub is an American peer-to-peer lending company, headquartered in San Francisco, California. It is the world's largest peer-to-peer lending platform.

**Sample Dataset**

<img src=/Images/dataset.png width=80% height=80%>

### Loan Portfolio Dashboard
Loan Portfolio Dashboard monitors and assesses bank lending activities by visulizing aggregated statistics and patterns.

**SQL Code Calculating Annual Return Rate**

<img src=/Images/sql.png width=80% height=80%>

<img src=/Images/dashboard.png>

<img src=/Images/burrower.png>

<img src=/Images/risk.png>

### Model Evaluation
Because there are more loans that are paid off compared to the ones that default, class imbalance becomes a concern in credit models. Therefore, it is crucial to employ metrics that are sensitive to imbalanced labels, such as precision, recall, and F1 score. Since it's important to measure the model's ability to identify loans likely to default and to correctly allocate funds to loans expected to be repaid, the recall for the default class and the precision for the non-default class emerge as pivotal metrics in this context.

Two classfiers are constructed, Random Forest Classifier and Logistic Regression Classifier. 

**Ramdom Forest Classifier Evaluation Metrics**

<img src=/Images/random_evaluation.png width=40% height=40%>

**Logistic Regression Evaluation Metrics**

<img src=/Images/logistic_evaluation.png width=40% height=40%>

**Number of Loans Approved**

<img src=/Images/random_num.png width=80% height=80%>
<img src=/Images/logistic_num.png width=80% height=80%>

Even though Logistic Regression has a higher recall for the default class and a higher precision for the non-default class, it has significantly less number of approved loans compared to the actual number of loans that are repaid. Therefore, it might have a less amount of total return.



