<div align="center">

<h1>Fraud Detection for Financial Transactions</h1>

</div>

<hr>

<h2>Overview</h2>

<p>
This project focuses on detecting fraudulent financial transactions using
machine learning techniques. Fraud detection is challenging due to extreme
class imbalance and high business cost of missed fraud.
</p>

<p>
The goal is to build an interpretable and effective fraud detection system
while preserving real-world transaction behavior.
</p>

<hr>

<h2>Dataset</h2>

<p>
<strong>Fraudulent Transactions Dataset (Kaggle)</strong><br>
https://www.kaggle.com/datasets/chitwanmanchanda/fraudulent-transactions-data
</p>

<ul>
  <li>Total transactions: ~6 million</li>
  <li>Target variable: <code>isFraud</code></li>
</ul>

<hr>

<h2>Data Preparation</h2>

<ul>
  <li>Removed identifier columns (<code>nameOrig</code>, <code>nameDest</code>)</li>
  <li>Label encoded transaction type</li>
  <li>Outliers retained due to relevance in fraud detection</li>
  <li>Time-based train-test split to prevent data leakage</li>
</ul>

<hr>

<h2>Handling Class Imbalance</h2>

<p>
Instead of resampling, class weighting and probability threshold tuning were
used to handle class imbalance while preserving real-world data distribution.
</p>

<hr>

<h2>Models Used</h2>

<ul>
  <li>Logistic Regression (baseline)</li>
  <li>Random Forest Classifier (final model)</li>
</ul>

<hr>

<h2>Model Evaluation</h2>

<ul>
  <li>Precision, Recall, F1-score</li>
  <li>ROC-AUC</li>
  <li>Confusion Matrix</li>
</ul>

<p>
Thresholds (0.1–0.3) were evaluated to balance fraud detection and false positives.
</p>

<hr>

<h2>Key Fraud Indicators</h2>

<ul>
  <li>TRANSFER and CASH_OUT transaction types</li>
  <li>High transaction amounts</li>
  <li>Abnormal balance changes</li>
</ul>

<hr>

<h2>Technologies Used</h2>

<ul>
  <li>Python</li>
  <li>Pandas, NumPy</li>
  <li>Scikit-learn</li>
  <li>Matplotlib, Seaborn</li>
</ul>

<hr>

<h2>Author</h2>

<p>
<strong>Mohammed Maaz Ali</strong><br>
B.Tech Computer Science Engineering<br>
IIIT Kottayam
</p>
